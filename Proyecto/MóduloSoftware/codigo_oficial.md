#include \<WiFi.h\> #include \<WebServer.h\> #include \<Wire.h\>
#include \<OneWire.h\> #include \<DallasTemperature.h\> #include
\<LiquidCrystal_I2C.h\> #include \<HTTPClient.h\> #include
\<ArduinoJson.h\>

// \-\-\-- Configuración de sensores \-\-\-- #define ONE_WIRE_BUS 32
OneWire oneWire(ONE_WIRE_BUS); DallasTemperature sensors(&oneWire);

// Sensor de color TCS230 #define S0 4 #define S1 5 #define S2 18
#define S3 19 #define OUT 33

// Pines LED const int LED_GREEN = 23; const int LED_RED = 27; const int
LED_COMMON = 14;

// WiFi const char\* ssid = \"GalaxyA04s\"; const char\* password =
\"12345678\";

// Sensor de voltaje/pH #define VOLTAGE_PIN 34

// Servidor Web WebServer server(80);

// LCD LiquidCrystal_I2C lcd(0x27, 20, 4);

// Variables globales bool isSendingData = true; unsigned long lastSend
= 0;

// \-\-\-- Funciones \-\-\--

// Leer color void setupColorSensor() { pinMode(S0, OUTPUT); pinMode(S1,
OUTPUT); pinMode(S2, OUTPUT); pinMode(S3, OUTPUT); pinMode(OUT, INPUT);
digitalWrite(S0, HIGH); digitalWrite(S1, LOW); }

int readColor(String color) { if (color == \"red\") { digitalWrite(S2,
LOW); digitalWrite(S3, LOW); } else if (color == \"green\") {
digitalWrite(S2, HIGH); digitalWrite(S3, HIGH); } else if (color ==
\"blue\") { digitalWrite(S2, LOW); digitalWrite(S3, HIGH); } return
pulseIn(OUT, LOW); }

// Calcular pH float calculatepH(float voltage) { return (-4.0 / 25.0)
\* voltage + 4.6052; }

// Enviar datos al servidor PHP void sendDataToServer(float temperature,
float pH, float voltage) { if (WiFi.status() == WL_CONNECTED) {
HTTPClient http;
http.begin(\"http://10.93.200.219/urequestESP32/urequestPHP.php\");
http.addHeader(\"Content-Type\", \"application/json\");

DynamicJsonDocument doc(1024); doc\[\"temperature\"\] = temperature;
doc\[\"pH\"\] = pH; doc\[\"voltage\"\] = voltage;

String jsonData; serializeJson(doc, jsonData);

int httpResponseCode = http.POST(jsonData);

if (httpResponseCode \> 0) { String response = http.getString();
Serial.println(\"Datos enviados correctamente:\");
Serial.println(response); } else { Serial.println(\"Error al enviar
datos: \" + String(httpResponseCode)); }

http.end(); } else { Serial.println(\"Error: Wi-Fi no conectado\"); } }

// Página principal void handleRoot() { String html = \"\<h2\>ESP32
WebServer\</h2\>\"; html += \"\<a href=\\\"/led1/on\\\"\>LED1 ON\</a\>
\| \"; html += \"\<a href=\\\"/led1/off\\\"\>LED1
OFF\</a\>\<br\>\<br\>\";

html += \"\<h3\>Control de envío de datos\</h3\>\"; if (isSendingData)
html += \"\<a href=\\\"/stop\\\"\>Detener envío\</a\>\<br\>\<br\>\";
else html += \"\<a href=\\\"/start\\\"\>Iniciar
envío\</a\>\<br\>\<br\>\";

sensors.requestTemperatures(); float temp = sensors.getTempCByIndex(0);
if (temp == DEVICE_DISCONNECTED_C) temp = 0;

int sensorValue = analogRead(VOLTAGE_PIN); float voltage = (sensorValue
/ 4095.0) \* 3.3; float pH = calculatepH(voltage);

int red = readColor(\"red\"); int green = readColor(\"green\"); int blue
= readColor(\"blue\");

html += \"\<p\>Temperatura: \" + String(temp) + \" °C\</p\>\"; html +=
\"\<p\>Voltaje: \" + String(voltage, 2) + \" V\</p\>\"; html +=
\"\<p\>pH: \" + String(pH, 2) + \"\</p\>\"; html += \"\<p\>Rojo: \" +
String(red) + \" \| Verde: \" + String(green) + \" \| Azul: \" +
String(blue) + \"\</p\>\";

server.send(200, \"text/html\", html);

// Parpadeo del LED común digitalWrite(LED_COMMON, HIGH); delay(80);
digitalWrite(LED_COMMON, LOW); }

void handleAction() { String action = server.arg(\"action\"); if (action
== \"ON\") { Serial.println(\"Encendiendo el ESP32\...\"); } else if
(action == \"OFF\") { Serial.println(\"Reiniciando el ESP32\...\");
ESP.restart(); } server.sendHeader(\"Location\", \"/\");
server.send(303); }

// \-\-\-- SETUP \-\-\-- void setup() { pinMode(LED_GREEN, OUTPUT);
pinMode(LED_RED, OUTPUT); pinMode(LED_COMMON, OUTPUT);

digitalWrite(LED_GREEN, LOW); digitalWrite(LED_RED, LOW);
digitalWrite(LED_COMMON, LOW);

Serial.begin(115200); Serial.print(\"Conectando a Wi-Fi\...\");
WiFi.begin(ssid, password); while (WiFi.status() != WL_CONNECTED) {
delay(500); Serial.print(\".\"); }

Serial.println(\"\\nConectado a Wi-Fi\"); Serial.print(\"IP: \");
Serial.println(WiFi.localIP());

digitalWrite(LED_GREEN, HIGH);

sensors.begin(); setupColorSensor();

server.on(\"/\", handleRoot);

server.on(\"/led1/on\", \[\]() { digitalWrite(LED_GREEN, HIGH);
server.sendHeader(\"Location\", \"/\"); server.send(303); });

server.on(\"/led1/off\", \[\]() { digitalWrite(LED_GREEN, LOW);
server.sendHeader(\"Location\", \"/\"); server.send(303); });

server.on(\"/start\", \[\]() { isSendingData = true;
server.sendHeader(\"Location\", \"/\"); server.send(303); });

server.on(\"/stop\", \[\]() { isSendingData = false;
server.sendHeader(\"Location\", \"/\"); server.send(303); });

server.on(\"/action\", handleAction); server.begin();

lcd.begin(); lcd.backlight(); lcd.setCursor(0, 0); lcd.print(\"Conectado
WiFi\"); delay(2000); lcd.clear(); }

// \-\-\-- LOOP \-\-\-- void loop() {

if (WiFi.status() == WL_CONNECTED) digitalWrite(LED_GREEN, HIGH); else
digitalWrite(LED_GREEN, LOW);

server.handleClient();

digitalWrite(LED_COMMON, HIGH);

sensors.requestTemperatures(); float temp = sensors.getTempCByIndex(0);
if (temp == DEVICE_DISCONNECTED_C) temp = 0;

int sensorValue = analogRead(VOLTAGE_PIN); float voltage = (sensorValue
/ 4095.0) \* 3.3; float pH = calculatepH(voltage);

digitalWrite(LED_COMMON, LOW);

// 🔴 LED ROJO SOLO cuando pH \> 7 if (pH \> 7) { digitalWrite(LED_RED,
HIGH); } else { digitalWrite(LED_RED, LOW); }

lcd.setCursor(0, 0); lcd.print(\"Temp: \"); lcd.print(temp, 1);
lcd.print(\"C \");

lcd.setCursor(0, 1); lcd.print(\"Volt: \"); lcd.print(voltage, 2);
lcd.print(\"V \");

lcd.setCursor(0, 2); lcd.print(\"pH: \"); lcd.print(pH, 2); lcd.print(\"
\");

if (isSendingData && (millis() - lastSend \> 10000)) {
sendDataToServer(temp, pH, voltage); lastSend = millis(); } }
