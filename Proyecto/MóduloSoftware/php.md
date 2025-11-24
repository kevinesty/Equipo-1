\<?php header(\"Content-Type: application/json; charset=UTF-8\");

// Conexión a la base de datos try { \$conexion = new
PDO(\'mysql:host=localhost;dbname=test\', \'root\', \'\');
\$conexion-\>exec(\"set names utf8\"); } catch (PDOException \$e) { echo
json_encode(\[\"status\" =\> \"error\", \"message\" =\> \"Error de
conexión: \" . \$e-\>getMessage()\]); exit; }

// Leer el cuerpo JSON \$json = file_get_contents(\'php://input\');
\$data = json_decode(\$json);

if (\$data === null) { echo json_encode(\[\"status\" =\> \"error\",
\"message\" =\> \"JSON inválido o vacío\", \"json_recibido\" =\>
\$json\]); exit; }

if (isset(\$data-\>temperature) && isset(\$data-\>pH) &&
isset(\$data-\>voltage)) { \$temperature =
floatval(\$data-\>temperature); \$pH = floatval(\$data-\>pH); \$voltage
= floatval(\$data-\>voltage);

try { \$sql = \"INSERT INTO sensor_data (temperature, pH, voltage,
timestamp) VALUES (:temperature, :pH, :voltage, NOW())\"; \$stmt =
\$conexion-\>prepare(\$sql); \$stmt-\>bindParam(\':temperature\',
\$temperature); \$stmt-\>bindParam(\':pH\', \$pH);
\$stmt-\>bindParam(\':voltage\', \$voltage);

if (\$stmt-\>execute()) { echo json_encode(\[\"status\" =\> \"success\",
\"message\" =\> \"Datos insertados correctamente\"\]); } else { echo
json_encode(\[\"status\" =\> \"error\", \"message\" =\> \"No se pudieron
insertar los datos\"\]); } } catch (PDOException \$e) { echo
json_encode(\[\"status\" =\> \"error\", \"message\" =\> \"Error al
insertar: \" . \$e-\>getMessage()\]); } } else { echo
json_encode(\[\"status\" =\> \"error\", \"message\" =\> \"Datos
incompletos\", \"json_recibido\" =\> \$json\]); } ?\>
