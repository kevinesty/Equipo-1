"Año de la recuperación y consolidación de la economía peruana"

# Informe técnico y lista de exigencias

Curso: Fundamentos de Diseño

**Docentes:**

JHOMER RODRIGO CONTRERAS PAUCCA

RENZO JOSE CHAN RIOS

HARRY ANDERSON RIVERA TITO

UMBERT LEWIS DE LA CRUZ RODRIGUEZ

Integrantes:

Areche Espeza Bryan Angello 

Carvallo Neciosup Kevin Esty  

Gygax Malca  Ivana Francesca

Sihuincha Palacin Shedira Lumeris

 

25 de Septiembre  del 2025 

Arquitectura Metodológica para el Desarrollo de un Modelo de Piel Sintética Bioimpresa con Sensor Integrado de pH para la Detección en Tiempo Real de pH

Shin, J., et al. (2022). "3D Bioprinting of a Thick and Perfusable Skin Patch for Non-Invasive Sensing of Molecular Biomarkers". Advanced Science.

Este proyecto replica y amplía la metodología establecida por Shin et al. (2022) para desarrollar un modelo de piel bioimpresa que integra un sensor de pH en su matriz. La acidificación del microambiente tisular, producto del incremento del metabolismo glucolítico (Efecto Warburg) durante la activación inmune, sirve como indicador temprano de sensibilización cutánea. Utilizando una bio-tinta a base de Gelatina Metacrilada (GelMA) y un indicador colorimétrico de pH (Rojo de Fenol), se fabricará un constructo epidérmico estratificado. La respuesta del sensor se correlacionará con ensayos inmunológicos standard (ELISA de IL-1α) siguiendo la directriz OECD 442E, validando esta plataforma de detección óptica no invasiva para pruebas de alergia.

**1\. Introducción y motivación** 

La industria cosmética y farmacéutica enfrenta un desafío crítico, donde la creciente demanda de productos seguros contrasta directamente con las limitaciones de los métodos actuales para evaluar alergias cutáneas. Si bien los modelos de piel sintética convencionales son aceptados regulatoriamente, estos dependen fundamentalmente de análisis destructivos que impiden la monitorización en tiempo real y generan una alta variabilidad en los resultados. Esta problemática motiva el presente proyecto debido a tres necesidades urgentes e interconectadas: en primer lugar, una necesidad ética y regulatoria, dado que más de 40 países han prohibido las pruebas en animales, creando así una demanda insatisfecha de alternativas avanzadas; en segundo término, una necesidad científica, ya que la comunidad especializada requiere métodos que capturen la cinética completa de las respuestas biológicas; y finalmente, una clara oportunidad de mercado, puesto que se proyecta que el sector de toxicología in vitro superará los $12 mil millones para 2027, sin que actualmente existen productos comerciales con capacidades de sensado integrado.

**Objetivo** 

El presente informe técnico tiene como objetivo principal demostrar la viabilidad técnica y comercial de un modelo de piel bio impresa con sensores integrados para la detección en tiempo real de reacciones alérgicas. Para alcanzar este propósito general, se han establecido los siguientes objetivos específicos interrelacionados:

En primer lugar, se busca validar la superioridad técnica del modelo propuesto mediante un análisis comparativo exhaustivo frente a las soluciones existentes en el mercado, con el fin de cuantificar sus ventajas en términos de precisión y eficiencia. Paralelamente, se pretende identificar la ruta de desarrollo más adecuada a través del análisis de patentes clave y componentes comerciales disponibles, lo que permitirá definir una estrategia de implementación efectiva. Asimismo, es fundamental establecer especificaciones técnicas detalladas que prioricen tanto la usabilidad como la escalabilidad industrial del producto, asegurando su adaptación a los entornos productivos reales. Finalmente, el informe busca definir criterios de éxito medibles que integren aspectos tecnológicos y comerciales, con el propósito de garantizar no solo la funcionalidad del dispositivo sino también su viabilidad económica y su potencial de adopción en el mercado.

**2.-Revisión de la Literatura**

La siguiente revisión sintetiza los avances científicos clave que sustentan el desarrollo de modelos de piel bioimpresa con capacidades de sensado integrado. La literatura se ha organizado en cuatro pilares fundamentales que convergen hacia la viabilidad técnica del sistema propuesto

## **Módulos Tecnológicos Esenciales**

### **1\. Módulo de Biofabricación Avanzada**

**Artículo real de respaldo:** *“Multiscale bioprinting of vascularized models”* (2018). 

* **Evidencia científica:**

  * Uso de bioimpresión con tintas sacrificiales para producir canales vasculares dentro de hidrogeles.   
  * Estructuras vasculares impresas con escalas desde \~100 µm hasta \~1 mm, logrando jerarquía de vasos.

  * Soporte para cultivo celular prolongado con perfusión de medios a través de estas redes vasculares.   
* **Métricas de desempeño:**

  * Alta viabilidad celular, sobre \~85-95 % después de imprimir y durante cultivo.

  * Canales interconectados con diámetros jerárquicos (50-250 µm) manteniendo integridad estructural.

**2\. Módulo de Sensado Óptico**

**Artículo real de respaldo:** *“Optical Sensor for Real-Time pH Monitoring in Human Tissue”* (PubMed)

* **Evidencia científica:**

  * Sensor óptico basado en fibra flexible con material híbrido sol-gel sensible al pH, para monitoreo continuo.

  * Resolución de detección muy fina (\~0.0013 unidades de pH) entre condiciones fisiológicas.

  * Tiempo de respuesta rápido: menos de 2 minutos.

* **Métricas de desempeño:**

  * Excelente reproducibilidad entre sensores diferentes.

  * Drift (desviación) bajo (\~0.003 pH unidades en \~22 h) en condiciones de laboratorio. 

### **3\. Plataforma de Biofabricación / Impresión multimaterial & vascularización**

**Artículo real de respaldo:** *“Embedded multimaterial bioprinting platform for biofabrication of biomimetic vascular structures”* (Journal of Materials Research, 2021\) 

* **Evidencia científica:**

  * Plataforma de bioimpresión multimaterial con cabezal de impresión microfluídico para fabricar estructuras vasculares semejantes a las naturales.

  * Alta precisión, reproducibilidad estructural, y uso de múltiples materiales para mimetizar distintas funciones vasculares.

* **Métricas de desempeño:**

  * Dimensiones de canales y geometría jerárquica logradas con fidelidad.   
  * Viabilidad celular aceptable, integración de diferentes tipos celulares (endoteliales, estromales) en la estructura.

### **4\. Módulo de Transductores Wearables / Sensores de pH con microneedles**

**Artículo real de respaldo:** *“Wearable microneedle array-based sensor for transdermal monitoring of pH levels in interstitial fluid”* (2022) 

* **Evidencia científica:**

  * Parche con microneedles poliméricos (≈ 10,000 punzones/cm²) recubiertos con polianilina para detección potenciométrica de pH en fluido intersticial.

  * Rango de operación de pH 4.0 a 8.6, buena precisión (\~±0.036 unidades pH).

  * Lecturas en tiempo real, respuesta estable.

* **Métricas de desempeño:**

  * Sensibilidad \~62.9 mV por unidad de pH (valor típico de potenciometría).

  * Precisión ±0.036 unidades pH. 

### **5\. Hidrogeles ópticos / sensores ópticos reversibles de pH**

**Artículo real de respaldo:** *“Optical Hydrogel Detector for pH Measurements”* (Biosensors, 2022\) 

* **Evidencia científica:**

  * Hidrogel sensible al pH cuya superficie ha sido moldeada con patrón de lente Fresnel; al cambiar el pH, el hidrogel se hincha o se contrae, cambiando la focalidad de la lente y por lo tanto la intensidad óptica medida.

  * Rango de pH evaluado fue \~4-7 (más sensible en región ácida pH \~4.5-5.5).

* **Métricas de desempeño:**

  * Cambio de potencia óptica de \~13 % con cambio de pH en esa región.

  * Respuesta reversible, buen tiempo de respuesta (corto)

**3.-Patentes Relevantes**

**WO2025049410A1** — *3D-printed epidermal wearable microfluidic electronic skin* (sistema 3D-impreso tipo “electronic skin”, biomateriales \+ microfluidos).

Piel electrónica microfluídica vestible epidérmica impresa en 3D para la vigilancia multimodal de la salud basada en aprendizaje automático.

Sistemas y métodos para un sistema vestible que monitoriza diversos biomarcadores mediante una piel electrónica vestible impresa en 3D. En concreto, el sistema vestible consiste en una piel electrónica microfluídica vestible epidérmica impresa en 3D que puede estar compuesta por una combinación de nanomateriales multidimensionales, polímeros e hidrogeles. La piel electrónica microfluídica vestible epidérmica puede integrarse con sensores, electrodos, microfluídica y un procesador para recopilar y analizar biomarcadores moleculares de muestras de biofluidos en la piel del usuario, a la vez que analiza sus biomarcadores fisiológicos para evaluar su estado de salud o recopilar métricas de monitorización.

**US20230255542A1** — *Patch for sensing a physiological response* (parche para detectar condiciones fisiológicas; útil como referencia de arquitectura para parches con múltiples sensores). 

Se describe un parche para detectar distintas condiciones indicativas de una respuesta fisiológica. El parche incluye una base para fijarse a una región de la piel que experimenta una respuesta fisiológica. El parche también incluye un primer sensor en la base que detecta una primera condición indicativa de la respuesta fisiológica de la región de la piel, un segundo sensor en la base que detecta una segunda condición indicativa de la respuesta fisiológica, y un tercer sensor en la base que detecta una tercera condición indicativa de la respuesta fisiológica. El primer sensor, el segundo

**WO2021176277A1** — *Skin-like wearable electronic device and method of manufacturing thereof*

Se proporcionan sistemas y métodos para evaluar parámetros de salud cardiovascular, que comprenden un sistema configurado para crear un mapa de presión de la superficie fisiológica (como la piel) utilizando una combinación de actuadores y conjuntos de sensores de presión

**4.-Productos Comerciales**

## 1\. Epinephrine Auto-Injector (Ej: EpiPen)

* Es un dispositivo portátil para administración automática de epinefrina (adrenalina) en casos de anafilaxia u otras reacciones alérgicas graves.

* Viene en dosis estándar (por ejemplo 0,3 mg) o versiones junior (0,15 mg) dependiendo del paciente.

* Está diseñado para uso rápido: el usuario o un familiar puede activarlo ante los primeros síntomas de una reacción alérgica grave, mientras espera atención médica.

* Su diseño incluye una aguja retráctil automática y mecanismos de seguridad para evitar activaciones accidentales. (Ver instrucciones oficiales del fabricante)

Aunque no es un dispositivo sensorial ni bioimpreso, sirve como ejemplo de un dispositivo médico crítico, portátil, confiable, con requisitos muy altos de seguridad, regulaciones, tolerancia del usuario, y diseño robusto para uso en condiciones adversas. En tu proyecto, puedes aprender sobre estándares de usabilidad, diseño para fiabilidad y requisitos reguladores.

## 

## 2\. i-STAT Handheld Blood Analyzer (Abbott)

* Sistema portátil de análisis de sangre para punto de atención (“point-of-care”) que permite obtener parámetros con calidad de laboratorio en minutos.

* Solo requiere pequeñas muestras de sangre (2-3 gotas) para muchos tipos de pruebas (gases sanguíneos, electrolitos, metabolitos, marcadores cardíacos, etc.).

* El equipo incluye un lector portátil \+ cartuchos de prueba desechables que contienen los biosensores necesarios.

* Algunos modelos tienen conectividad inalámbrica (por ejemplo, i-STAT 1 Wireless) para transferir resultados automáticamente al sistema de registro médico (EMR / LIS).

 Este dispositivo es un benchmark tecnológico: muestra qué tan integrados, rápidos y confiables pueden llegar a ser los sistemas portátiles de diagnóstico. En tu proyecto, tus sensores de pH / temperatura podrían buscar acercarse (aunque sea a menor escala) a la agilidad, precisión y confiabilidad que demuestra el i-STAT.

## 3\. Lactate Scout+ (EKF Diagnostics)

* Es un analizador portátil de lactato de sangre (handheld) desarrollado por EKF Diagnostics.

* Requiere un volumen muy pequeño de sangre (≈ 0,2 µL de sangre capilar) para obtener el resultado.

* El resultado se entrega rápidamente (≈ 10 segundos) tras la aplicación de la muestra.

* Incorpora compensación de hematocrito: tiene mecanismos para ajustar sus lecturas según el valor de hematocrito del paciente, mejorando precisión frente a variaciones fisiológicas.

* Incluye funciones adicionales como cronómetro, temporizador, almacenamiento de datos, conectividad Bluetooth para descarga de resultados.   
* Memoria: puede almacenar múltiples resultados (por ejemplo, 250 registros).

Como dispositivo portátil, esto te da un ejemplo de cómo se ha optimizado un analizador para ser usado en campo, con rapidez, poca muestra, ajustes automáticos y conectividad. Tus sensores de pH / temperatura podrían tomar inspiración para minimizar volumen, tiempo, calibración automática y almacenamiento / transmisión de datos.

**5.-Enlace al producto**

1\. Asumir el problema en forma crítica.

Reconocer la Urgencia Vital: El problema central no es solo técnico, sino médico-vital. La anafilaxia es una emergencia que puede ser mortal en minutos.

Criticar la Propuesta Inicial: Un sensor de pH no es la solución de primera línea. La administración inmediata de adrenalina se basa en síntomas clínicos, no en una medición de pH. Un sensor podría dar una falsa sensación de seguridad o retrasar el tratamiento.

Definir el Alcance Real: El objetivo útil no es "diagnosticar anafilaxia", sino posiblemente "monitorizar la gravedad del shock y la eficacia del tratamiento en un entorno hospitalario controlado, una vez iniciada la reanimación".

2\. Averiguar el estado de la tecnología.

Tecnología Médica Estándar (Gold Standard): La gasometría arterial es el método preciso y confiable para medir pH, pCO2, HCO3- y lactato. Es invasiva (requiere punción arterial) y se realiza en laboratorio o punto de atención (point-of-care).

Tecnología de Sensores Disponibles:

    Electrodos de Vidrio para pH: Alta precisión, pero frágiles, requieren calibración constante y no son adecuados para contacto directo con sangre sin un sistema de medición complejo (flujo, anticoagulantes).

    Sensores de pH de Estado Sólido (ISFET): Más robustos que los de vidrio, potencial para miniaturización. Son la base de algunos glucómetros y analizadores portátiles. Su precisión en matrices complejas como la sangre es un desafío.

    Sensores Ópticos de pH: Utilizan un colorante que cambia de color con el pH. Pueden ser desechables, evitando problemas de contaminación. Es una tecnología prometedora para aplicaciones "point-of-care".

Conclusión: La tecnología base existe, pero integrarla en un dispositivo fiable, rápido y seguro para uso en emergencias es el reto principal.

3\. Analizar la situación del problema.

Necesidad No Cubierta: No existe un dispositivo rápido, no invasivo y portátil para cuantificar el grado de acidosis en segundos en el lugar donde ocurre la emergencia (pre-hospitalaria).

Barreras Principales:

    Biológicas: La necesidad de una muestra de sangre (venosa o arterial). La coagulación y el contenido proteico de la sangre interfieren con los sensores.

    Técnicas: Velocidad de medición (\< 60 segundos), calibración automática o de larga duración, precisión clínica (error \< ±0.02 unidades de pH).

    Regulatorias: Cualquier dispositivo médico que se use para diagnóstico o monitorización requiere aprobación de entidades como la FDA (EE. UU.) o la EMA (UE), un proceso largo y costoso que exige estudios clínicos rigurosos.

4\. Comprobar las posibilidades de realización.

Factible a Nivel de Prototipo (Baja Fidelidad): Sí. Es posible construir un sistema con un Arduino, un sensor de pH genérico y una solución tampón para demostrar el principio de medición de pH in vitro.

Factible como Producto Médico (Alta Fidelidad): Extremadamente difícil y costoso a corto/medio plazo.

    Posible: La tecnología ISFET u óptica podría, en teoría, integrarse en un cartucho desechable con un micro-analizador.

    Limitaciones Críticas: El mayor obstáculo no es técnico, sino médico y regulatorio. La necesidad de una muestra de sangre invasiva y la velocidad de la anafilaxia hacen que la utilidad clínica real sea cuestionable frente a la simplicidad del diagnóstico sintomático.

**6\. Lista de exigencias.**

**Tabla 1\. Lista de exigencias para el proyecto**

| LISTA DE EXIGENCIAS |  |  | Páginas |
| :---: | :---: | ----- | :---: |
|  |  |  | Ed. rev. 1 |
| Proyecto: |  |  | Fecha: 25/09/2025 |
| Cliente: |  | UNIVERSIDAD PERUANA CAYETANO HEREDIA | Elaborado: A.A, I.G, K.C, L.S  |
| Fecha (cambios) | Deseo o exigencia | Descripción | Responsable |
|  | E | Precisión Clínica: Error máximo de ±0.03 unidades de pH en rango 7.0-7.4 | K.C |
|  | E | Tiempo de Respuesta: \<60 segundos desde toma de muestra hasta resultado | K.C |
|  | E | Biocompatibilidad: Cumplir norma ISO 10993 (cartucho desechable estéril) | I.G |
|  | E | Fiabilidad: Indicación clara de errores (muestra insuficiente, sensor fallido) | L.S |
|  | E | Tipo de Muestra: Sangre venosa o capilar (≤0.5 mL) | I.G |
|  | E | Automatización: Calibración automática con cartucho desechable pre-calibrado | K.C |
|  | E | Robustez: Operativo en condiciones ambientales variables (10°C-40°C) | K.C, L.S |
|  | E | Interfaz de Usuario: Pantalla clara con indicador de severidad | A.A |
|  | E | Conectividad: Transmisión Bluetooth para historial médico | A.A, K.C |

**7\. Plan de trabajo**

![][image1]

**8.-Conclusiones y Recomendaciones**

Síntesis de hallazgos:

* La tecnología para desarrollar un sensor de pH portátil existe pero requiere importantes inversiones  
* La integración en un cartucho desechable biocompatible es el principal desafío técnico  
* La utilidad clínica real debe demostrarse frente al diagnóstico sintomático estándar

Propuestas de desarrollo o mejora:

1. Iniciar con un prototipo de bajo costo usando sensores ISFET comerciales y Arduino  
2. Enfocar inicialmente el dispositivo para monitorización hospitalaria rather than uso prehospitalario  
3. Establecer alianzas con empresas de dispositivos médicos para la fase regulatoria  
4. Considerar el lactato como parámetro adicional dado su papel central en la acidosis del shock

**9.- Bibliografía**

Miri, A. K., Khalilpour, A., Cecen, B., Maharjan, S., Shin, S. R., & Khademhosseini, A. (2019). Multiscale bioprinting of vascularized models. *Biomaterials, 198,* 204–216. [https://doi.org/10.1016/j.biomaterials.2018.08.006](https://doi.org/10.1016/j.biomaterials.2018.08.006)

Wencel, D., Kaworek, A., Abel, T., Efremov, V., Bradford, A., Carthy, D., Coady, G., McMorrow, R. C. N., & McDonagh, C. (2018). Optical sensor for real-time pH monitoring in human tissue. *Small, 14*(51), e1803627. [https://doi.org/10.1002/smll.201803627](https://doi.org/10.1002/smll.201803627)

Alqurashi, Y., Elsherif, M., Hendi, A., Essa, K., & Butt, H. (2022). Optical Hydrogel Detector for pH Measurements. *Biosensors, 12*(1), 40\. https://doi.org/10.3390/bios12010040

Dervisevic, M., et al. (2023). Wearable microneedle array-based sensor for transdermal monitoring of pH levels in interstitial fluid. *\[Journal\]*. Recuperado de [https://pubmed.ncbi.nlm.nih.gov/36462430/](https://pubmed.ncbi.nlm.nih.gov/36462430/?utm_source=chatgpt.com)

Miri, A. K., Khalilpour, A., Cecen, B., Maharjan, S., Shin, S. R., & Khademhosseini, A. (2019). Multiscale bioprinting of vascularized models. *Biomaterials, 198*, 204–216. [https://pubmed.ncbi.nlm.nih.gov/30244825](https://pubmed.ncbi.nlm.nih.gov/30244825?utm_source=chatgpt.com)

Wencel, D., Kaworek, A., Abel, T., Efremov, V., Bradford, A., Carthy, D., Coady, G., McMorrow, R. C. N., & McDonagh, C. (2018). Optical sensor for real-time pH monitoring in human tissue. *Small, 14*(51), e1803627. Recuperado de [https://pubmed.ncbi.nlm.nih.gov/30427575/](https://pubmed.ncbi.nlm.nih.gov/30427575/?utm_source=chatgpt.com)

“Skin-like wearable electronic device and method of manufacturing thereof.” (s. f.). WO2021176277A1. Recuperado de [https://patents.google.com/patent/WO2021176277A1/en](https://patents.google.com/patent/WO2021176277A1/en)

“3D-printed epidermal wearable microfluidic electronic skin.” (s. f.). WO2025049410A1. Recuperado de [https://patents.google.com/patent/WO2025049410A1/en](https://patents.google.com/patent/WO2025049410A1/en?utm_source=chatgpt.com)

“Patch for sensing a physiological response.” (s. f.). US20230255542A1. Recuperado de [https://patents.google.com/patent/US20230255542A1/en](https://patents.google.com/patent/US20230255542A1/en?utm_source=chatgpt.com)

EpiPen. (s. f.). Recuperado de [https://www.epipen.com/en](https://www.epipen.com/en?utm_source=chatgpt.com)

Abbott. (s. f.). i-STAT System. Recuperado de [https://www.globalpointofcare.abbott/us/en/product-details/apoc/i-stat-system-us.html](https://www.globalpointofcare.abbott/us/en/product-details/apoc/i-stat-system-us.html?utm_source=chatgpt.com)

EKF Diagnostics. (s. f.). New Lactate Scout+ Analyzer launched. Recuperado de [https://www.ekfdiagnostics.com/news/new-lactate-scout-plus-analyzer-launched/](https://www.ekfdiagnostics.com/news/new-lactate-scout-plus-analyzer-launched/?utm_source=chatgpt.com)

[image1]: <data:image/png;base64,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>