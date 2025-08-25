Proyecto IoT: Sistema Inteligente de Detección de Fugas de Agua con Arduino + ESP
    Contexto – ODS 6
El Objetivo de Desarrollo Sostenible (ODS) 6 busca garantizar la disponibilidad y gestión sostenible del agua para todos.
Uno de los grandes problemas es la pérdida de agua potable por fugas invisibles en viviendas y redes, lo que genera:
Desperdicio de agua potable.
Elevación en los costos del servicio.
Daños en infraestructuras por filtraciones y humedad.
Este proyecto plantea un sistema inteligente de bajo costo basado en Arduino + ESP8266/ESP32, capaz de detectar fugas en tiempo real y notificar al usuario vía WiFi.

    Objetivos del Proyecto
Detectar fugas de agua mediante sensores de flujo y humedad.
Notificar en tiempo real a través de WiFi (dashboard web o app móvil).
Automatizar el cierre del agua con una válvula solenoide en caso de fuga.
Visualizar el consumo en pantalla LCD y registrar históricos en la nube.

    Componentes principales
Arduino UNO / Nano – microcontrolador base.
ESP8266 (NodeMCU) o ESP32 – módulo para conexión WiFi.
Sensor de flujo YF-S201 – mide caudal y litros consumidos.
Sensor de humedad FC-28 – detecta fugas en el suelo.
Pantalla LCD 16x2 + I2C – muestra datos y alertas locales.
LEDs (rojo/verde/azul) – indicadores de estado.
Buzzer – alarma sonora de fuga.
Relé + válvula solenoide – corte automático del agua.
Protoboard, jumpers y resistencias – para el montaje.
Fuente de alimentación 5V–12V – según válvula y sensores.

    Flujo de trabajo del sistema
El sensor de flujo mide el caudal y los litros consumidos.
El sensor de humedad detecta presencia de agua en caso de fuga.
El Arduino procesa la información y:
Muestra datos en la pantalla LCD.
Activa LEDs y buzzer para alertas locales.
Envía la señal al ESP8266/ESP32 para reportarlo vía WiFi.
(Opcional) activa el relé para cerrar la válvula solenoide.
El ESP sube los datos a un dashboard web o aplicación móvil para notificar al usuario.

    Plataformas recomendadas para WiFi
ThingSpeak → visualización en tiempo real con gráficas.
Blynk IoT → app móvil lista para controlar y monitorear.
MQTT + Node-RED → control avanzado desde servidor local o nube.
Firebase → notificaciones push y base de datos en tiempo real.

    Posibles mejoras futuras
Control desde asistentes de voz (Google Home / Alexa).
Alimentación con energía solar para hacerlo autónomo.
Integración de más sensores: pH, turbidez, temperatura para evaluar calidad del agua.
Creación de una interfaz web personalizada con reportes de consumo históricos.

    Impacto
Este sistema ayuda a:
Reducir el desperdicio de agua en hogares y comunidades.
Ahorrar costos por facturación y mantenimiento.
Concienciar sobre el uso responsable del agua.
Contribuir directamente al ODS 6: Agua limpia y saneamiento.

    Idea del proyecto:
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/da78cc03-fea2-42d7-ae73-adeb65107bcb" />
