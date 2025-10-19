"Año de la recuperación y consolidación de la economía peruana"

# Informe técnico y lista de exigencias

Curso: Fundamentos de Diseño

**Docentes:**

**JHOMER RODRIGO CONTRERAS PAUCCA**

**RENZO JOSE CHAN RIOS**

**HARRY ANDERSON RIVERA TITO**

**UMBERT LEWIS DE LA CRUZ RODRIGUEZ**

**Asesor:**

**Lizardo Kendy Torres Ayala**

**Integrantes:**

**Areche Espeza Bryam Angello** 

**Carvallo Neciosup Kevin Esty**  

**Gygax Malca  Ivana Francesca**

**Sihuincha Palacin Shedira Lumeris**

 

**06 de Octubre de 2025** 

	

Implementación de sensores de bajo costo para mejorar la sensibilidad en la medición del pH en un sistema hidrogel bio impreso

1. **Introducción** 

La degradación de alimentos perecederos como carnes y pescados representa un desafío global en seguridad alimentaria y sostenibilidad. Actualmente, los métodos para determinar la frescura se basan principalmente en fechas de caducidad estimadas o en la inspección visual subjetiva, lo que genera tanto riesgos para la salud pública como un desperdicio alimentario significativo. Frente a esta problemática, surge la necesidad de desarrollar sistemas de monitorización simples, accesibles y confiables que proporcionen información en tiempo real sobre el estado de los productos. Esta investigación propone el desarrollo de un parche sensor basado en hidrogel bioimpreso con antocianinas, pigmentos naturales extraídos de fuentes vegetales, cuyo color varía de manera reversible según el pH del producto (1, 2). Al adherirse al envase del alimento, el sensor detecta los compuestos alcalinos liberados durante la descomposición microbiana, cambiando visiblemente de color para alertar a consumidores y distribuidores. La integración de un sistema de lectura con Arduino permite, además, la cuantificación objetiva del pH, ofreciendo una solución de bajo coste y doble funcionalidad para la gestión de la frescura en la cadena alimentaria.

2. **Objetivo del informe:**  
   **Objetivo General:**  
   Desarrollar un sistema confiable, económico y biocompatible para el monitoreo del pH en tiempo real, basado en hidrogeles bioimpresos con pigmentos naturales sensibles al pH, que permita mejorar la precisión y estabilidad en la detección de cambios químicos en alimentos como vegetales, carne roja, pollo, mariscos y pescados, contribuyendo así al control de su frescura y calidad.  
 


   **Objetivo Específico**  

1. Analizar los fundamentos teóricos y tecnológicos relacionados con sensores ópticos, hidrogeles poliméricos y pigmentos naturales sensibles al pH .  
2. Evaluar la precisión y sensibilidad del sensor desarrollado mediante pruebas experimentales en diferentes tipos de alimentos perecibles.  
3. Diseñar un sistema de medición que combina materiales naturales y componentes electrónicos de bajo costo.  
4. Promover el uso de materiales sostenibles y tecnologías accesibles en el diseño de sensores inteligentes para aplicaciones de control sanitario y conservación de alimentos.  
5. Implementar un sistema óptico de detección que permita registrar los cambios de color asociados a variaciones del pH en tiempo real.  
     
     
     
     
3. **Revisión de la Literatura:**   
   **3.1Artículo 1:**   
* **Título del artículo:**  Red Cabbage Anthocyanin-Loaded Bacterial Cellulose Hydrogel for Colorimetric Detection of Microbial Contamination and Skin Healing Applications  
* **Autores:** Hanna Melnyk, Olesia Havryliuk, Iryna Zaets,Tetyana Sergeyeva,Ganna Zubova ,Valeriia Korovina ,Maria Scherbyna, Lilia Savinska ,Lyudmila Khirunenko ,Evzen Amler, Maria Bardosova, Oleksandr Gorbach,Sergiy Rogalsky, Natalia Kozyrovska   
* **Fecha de publicación:** 31 July 2025  
* **Revista:** [Polymer-Based Composite Materials: Advancements and New Trends in Biomedical Engineering and Research](https://www.mdpi.com/journal/polymers/special_issues/Q3157P8253)

El artículo aborda el  desarrollo de materiales halocrómicos innovadores y de bajo costo para diagnosticar la contaminación microbiana en heridas y quemaduras puede facilitar eficazmente la regeneración tisular. En este estudio, combinamos la capacidad de detección del pH de las antocianinas de la col lombarda (RCA), de gran colorido, con su potencial cicatrizante dentro de una película única de polímero de celulosa que imita la matriz cutánea. Las actividades biológicas del extracto de RCA en celulosa bacteriana (BC) no mostraron citotoxicidad ni potencial de sensibilización cutánea en células humanas a concentraciones de RCA similares a las liberadas por los apósitos de BC/RCA (4,0–40,0 µg/mL). Se observó una disminución de la viabilidad celular y la apoptosis en células cancerosas humanas con RCA. La detección ocular invisible de la señal temprana de cambio de color de las RCA en respuesta a la alteración del pH por bacterias se registró con una aplicación para teléfonos inteligentes. La incorporación de RCA al polímero de BC ha alterado la morfología de su matriz, dando como resultado una red de microfibrillas de celulosa más densas. La completa coincidencia de los modos vibracionales detectados en los espectros de absorción del compuesto de celulosa/RCA con los modos en las RCA probablemente indica que estas conservan su estructura en la matriz de BC. Se pueden recomendar hidrogeles halocrómicos de BC/RCA, asequibles y sensibles, para la monitorización en línea de la contaminación microbiana, haciéndolos accesibles para los pacientes[(1)](https://www.zotero.org/google-docs/?34M2MM)  
	**3.2Artículo 2:**

* **Título del artículo:** Investigating the microbial properties of sodium alginate/chitosan edible film containing red beetroot anthocyanin extract for smart packaging in chicken fillet as a pH indicator  
* **Autores:** Milad Ranjbar, Mohammad Azizi, Gholamhassan Asadi, Hamed Ahari  
* **Fecha de publicación:** 5 August 2023  
* **Revista:** National Library of Medicine National: Center for Biotechnology Information

Este artículo remarca la tendencia actual en la producción de películas inteligentes se enfoca en el uso de indicadores de color sensibles al pH de origen natural. En este estudio se elaboraron películas comestibles a base de alginato de sodio y quitosano con la incorporación de extracto de antocianinas de betarraga, evaluando sus propiedades y su aplicación como recubrimiento para filetes de pollo. Se trabajó con tres tratamientos: control, A25%-Ch75% y A25%-Ch75%-Ac. Los resultados mostraron que el extracto no produjo diferencias notables en los espectros FTIR, aunque redujo la cristalinidad del material según el análisis XRD. Las imágenes SEM evidenciaron mayor porosidad y alteración en las cadenas poliméricas. En los filetes recubiertos se observó un aumento de parámetros microbiológicos y químicos con el tiempo, siendo menor en las muestras con extracto de betarraga. La dureza de las muestras disminuyó durante el almacenamiento, pero aumentó significativamente en las que contenían antocianinas. Los cambios de color coincidieron con la estructura de las antocianinas. En conjunto, la película con extracto de betarraga mejoró la calidad, prolongó la vida útil y redujo la carga microbiana del pollo, además de funcionar como indicador natural de deterioro[(2)](https://www.zotero.org/google-docs/?hCCAiT)

	**3.3Artículo 3:**

* **Título del artículo:** Novel colorimetric indicators based on alginate hydrogel beads containing anthocyanin for visual freshness monitoring of shrimp and minced chicken.  
* **Autores:** Samira Mohammadalinejhad, Ida-Johanne Jensen a , Marcin Kurek b , Jørgen Lerfall  
* **Fecha de publicación:** 1 May 2024  
* **Revista:** Intelligent packaging Freshness indicator Alginate hydrogel Anthocyanin 

El artículo presenta el desarrollo de nuevos indicadores colorimétricos mediante la incorporación de antocianinas en perlas de hidrogel de alginato mediante extrusión electrostática para un envasado inteligente. Se produjeron perlas de hidrogel de dos tamaños diferentes y se aplicaron en envases de camarones y pollo picado para detectar visualmente el estado de frescura durante el almacenamiento. Se analizó la frescura de los productos, el recuento viable de diversos tipos de bacterias (psicrotróficas, productoras de H2C, mesófilas y Pseudomonas spp.), el contenido de nitrógeno básico volátil total (NBVT), el pH, el valor K, el valor H y el nivel de aminas biógenas. El cambio de color de los indicadores (ΔE) se correlacionó con estos parámetros. El análisis de color de los indicadores durante el almacenamiento indicó valores de ΔE inferiores a 10 y superiores a 30 en los hidrogeles incorporados a los envases de pollo picado y camarones, respectivamente. El cambio de color de ambos indicadores integrados en el empaque de camarones se correlacionó fuertemente con el cambio en los recuentos viables, TVB-N, pH, valor K y valor H (r ≥ 0.8, p \< 0.016), así como con las aminas biógenas (r \= 0.7, p \< 0.05). Los indicadores aplicados al empaque de pollo picado mostraron cambios sutiles de color durante el almacenamiento, mientras que los del empaque de camarones reflejaron consistentemente las variaciones en la vida útil. Este enfoque innovador muestra potencial para mejorar la seguridad alimentaria y el control de calidad, especialmente en el empaque de mariscos, donde los indicadores han sido eficaces para señalar visualmente la frescura del producto[(3)](https://www.zotero.org/google-docs/?KOIy7m)

4. **Patentes Referenciales:**

### **4.1. Patente 1**

* **● Nombre de la patente:** pH sensing biofilm  
   **● País de origen:** Estados Unidos  
   **● Fecha de patentado:** 21 de agosto de 2018  
   **● Código:** US10054548B1  
   **● Enlace directo:**  
   https://patents.google.com/patent/US10054548B1  
* El modelo de invención denominado *pH sensing biofilm* describe un biopolímero funcionalizado capaz de detectar variaciones de pH mediante un cambio de color visible. La estructura consiste en un biofilm biodegradable fabricado a partir de nanocelulosa y biopolímeros naturales (como alginato o pectina), dentro del cual se inmovilizan antocianinas extraídas de *Petunia hybrida*.  
   El material presenta una alta sensibilidad cromática en el rango de pH 2–10, permitiendo identificar la degradación de productos alimenticios o variaciones en medios biológicos. Además, posee propiedades antimicrobianas y biocompatibles, haciéndolo útil tanto en empaques inteligentes como en recubrimientos biomédicos. La patente destaca la simplicidad del proceso de fabricación y su potencial para aplicaciones industriales ecológicas y sostenibles[(4)](https://www.zotero.org/google-docs/?1gT1rV)

### **4.2. Patente 2**

* **● Nombre de la patente:** pH indicator film comprising natural anthocyanin and biopolymer, and method for preparing the same  
   **● País de origen:** Corea del Sur  
   **● Fecha de patentado:** 14 de agosto de 2018  
   **● Código:** KR101877606B1  
   **● Enlace directo:**  
   https://patents.google.com/patent/KR101877606B1  
* El modelo de utilidad denominado *pH indicator film comprising natural anthocyanin and biopolymer* presenta una película flexible desarrollada a partir de agar, almidón de papa y antocianinas naturales obtenidas de fuentes como col morada, papa púrpura o aronia.  
   La estructura del film permite un cambio cromático progresivo según el pH del entorno, variando de rojo en medios ácidos a azul en medios básicos. Posee además resistencia al agua y buena estabilidad térmica, lo que mejora su durabilidad frente a la humedad ambiental.  
   Este sistema fue diseñado para monitorear la frescura de alimentos perecibles, actuando como indicador visual del grado de deterioro microbiano. Su fabricación utiliza métodos de mezclado en caliente y secado a baja temperatura, lo cual garantiza la preservación de los pigmentos naturales sin pérdida de sensibilidad[(5)](https://www.zotero.org/google-docs/?mpEONw)

**4.1 Patente 3:** 

**● Nombre de la patente:** Smart hydrogel-based colorimetric sensor for pH monitoring  
 **● País de origen:** China  
 **● Fecha de patentado:** 5 de marzo de 2021  
 **● Código:** CN112485547A  
 **● Enlace directo:**  
 https://patents.google.com/patent/CN115381191A/en

El modelo de invención denominado *Smart hydrogel-based colorimetric sensor for pH monitoring* describe un sensor colorimétrico inteligente basado en hidrogel polimérico con pigmentos naturales sensibles al pH, tales como antocianinas y curcumina.  
El diseño incluye una matriz de hidrogel de poliacrilamida y alginato, con agentes reticulantes que estabilizan el colorante dentro de la red polimérica. El sensor responde a cambios de pH mostrando variaciones reproducibles de color (de rojo a violeta y azul) en el rango pH 3–9, con tiempo de respuesta inferior a 10 segundos.  
 Además, el dispositivo puede integrarse con módulos ópticos o cámaras de smartphone para monitoreo digital, ofreciendo una alternativa de bajo costo para aplicaciones en bioimpresión, control de calidad de alimentos o monitoreo ambiental.  
 Su innovación radica en el método de inmovilización de pigmentos, que evita su lixiviación y prolonga la vida útil del sensor hasta 30 días sin degradación perceptible del color[(6)](https://www.zotero.org/google-docs/?90HQNI)

5. **Productos comerciales:** 

**5.1  Single-Use pH Flow-Through Cell (PreSens)**  
Sensor óptico de pH de uso único, diseñado para medir pH en líquidos en flujo continuo. Usa fluorescencia óptica en lugar de electrodos, lo que evita contaminación del medio. Es preciso (±0.05 pH) y rápido (\<2 min). Ideal para monitoreo en línea o automatizado en bioprocesos y sistemas experimentales[(7)](https://www.zotero.org/google-docs/?q0Z8jD)

**5.2  PhotoHA-IRG Hydrogel Kit (Merck Millipore):**  
Kit de ácido hialurónico metacrilado que forma hidrogeles al exponerse a luz UV. Se usa en cultivos celulares 3D por su alta hidratación y compatibilidad biológica. Permite crear estructuras suaves y porosas donde se pueden integrar sensores ópticos o colorimétricos para medir pH o condiciones químicas del entorno[(8)](https://www.zotero.org/google-docs/?7K0SxN)

**5.3Producto 3:  GelXA (CELLINK):**  
Bioink híbrido de GelMA, alginato y goma xantana, optimizado para bioimpresión 3D. Tiene buena viscosidad, elasticidad y fidelidad de forma, permitiendo crear hidrogeles precisos. Puede mezclarse con colorantes naturales o sensores electrónicos, útil para desarrollar constructos bio impresos con respuesta a pH[(9)](https://www.zotero.org/google-docs/?MANZ0A)

6. **Lista de exigencias:**

	

|  LISTA DE EXIGENCIA |  |  | Páginas: 6 |
| :---: | :---: | ----- | ----- |
|  |  |  | **Edición:**  |
|  **PROYECTO:** |  |  Sensor de ph biotecnológico   | **Fecha: 29/09/25** |
|  |  |  | **Revisado:**  |
|  **CLIENTE:** |  |  UNIVERSIDAD PERUANA CAYETANO HEREDIA | **Elaborado: I.G , S.S , KC** |
| Fecha  (cambios) | Deseo o Exigencia | **Descripción** | **Responsable** |
| 23/09/25 | E | **Función principal:** ● Detectar los cambios de color asociados a la variación       del pH en alimentos perecederos, indicando su nivel de frescura o deterioro. ● Integrar un sistema sensor de color basado en hidrogel con antocianinas que reacciona ante los compuestos liberados durante la descomposición. ● Permitir la lectura del cambio cromático mediante un módulo Arduino para cuantificar objetivamente el estado del producto. **Función secundaria:**  ● Proporcionar una señal visual clara y accesible para consumidores y distribuidores sobre la frescura del alimento. ● Enviar datos al sistema de registro o aplicación móvil para un seguimiento en tiempo real de la calidad del producto. ● Contribuir a la reducción del desperdicio alimentario al ofrecer una herramienta económica y sostenible para la gestión de la cadena alimentaria. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Geometría:** El sensor de color será compacto y delgado, diseñado para adherirse fácilmente a la superficie externa del envase del alimento sin alterar su forma ni funcionalidad. Su estructura estará compuesta por una fina capa de hidrogel bioimpreso con antocianinas, alojada en un soporte flexible y transparente que permita la visibilidad del cambio de color. Las dimensiones de referencia estarán optimizadas para adaptarse a distintos tipos de empaques, garantizando una instalación segura, ligera y ergonómica, compatible con los estándares de envasado comercial. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Cinemática:**El sistema de detección del sensor de color no requiere movimiento mecánico, pero su respuesta cromática se basa en un proceso dinámico de difusión y reacción química dentro del hidrogel. Al entrar en contacto con los compuestos volátiles liberados por el alimento en descomposición, las moléculas de antocianina modifican su estructura molecular, produciendo un cambio gradual y reversible de color. Este proceso constituye el “movimiento funcional” del sensor, garantizando una respuesta estable, segura y reproducible ante variaciones de pH, sin comprometer la integridad del material ni del envase. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Fuerzas:** El sensor debe ejercer una presión uniforme y mínima, suficiente para mantener el contacto entre el hidrogel y el medio de medición del pH, sin comprometer su estructura ni alterar sus propiedades físico-químicas. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Energía:**El sistema sensor de color será alimentado mediante una fuente eléctrica de baja potencia, adecuada para el funcionamiento del módulo Arduino y los componentes electrónicos asociados. En aplicaciones portátiles o de transporte, podrá incorporar una batería recargable de litio que garantice autonomía y continuidad en la medición. Para optimizar el consumo energético, el sistema incluirá un modo de reposo que reducirá la actividad del microcontrolador cuando no se detecten variaciones significativas en el color. Además, se integrarán protecciones básicas contra sobrecarga y cortocircuito, asegurando un funcionamiento estable, seguro y eficiente durante todo el monitoreo del alimento. |  **I.G , S.S , KC**  |
| 23/09/25 | E | **Materia:** Flujo material y transporte:El sistema está compuesto por un hidrogel bioimpreso que actúa como medio sensible al pH, permitiendo el transporte controlado de iones H⁺ y otras especies químicas que modifican su color o conductividad. Propiedades físicas y químicas:El hidrogel presenta alta capacidad de absorción de agua, elasticidad y biocompatibilidad. Sus propiedades químicas incluyen sensibilidad al pH, transparencia óptica y biodegradabilidad. Productos de entrada y salida: Entrada: muestra o entorno con determinado nivel de pH Salida: señal o cambio físico-químico observable en el hidrogel Materiales adicionales: Se emplean biopolímeros naturales (como alginato o celulosa), colorantes indicadores de pH, electrodos conductores de bajo costo y componentes electrónicos para la medición y registro de datos. Materiales prescritos (normativa): El diseño sigue lineamientos de seguridad y sostenibilidad, priorizando materiales no tóxicos, biodegradables y compatibles con alimentos, conforme a las recomendaciones de la Organización Mundial de la Salud (OMS) y las normas INACAL/INDECI    |  **I.G , S.S , KC** |
| 23/09/25 | E | **Señales (información):**  El sistema contará con las siguientes señales de entrada y salida, necesarias para garantizar la correcta medición y monitoreo del pH en el hidrogel bioimpreso: **Señales de entrada:** Señal de encendido: Activa los componentes eléctricos y electrónicos del sistema de medición, incluyendo los sensores de pH y los módulos de procesamiento. Señal de inicio: Inicia el proceso de calibración y lectura del sensor de pH integrado en el hidrogel bioimpreso. Señal de calibración: Permite ajustar los valores de referencia del sensor antes de cada medición, asegurando precisión en los resultados. Señales de sensores:  Lecturas de sensores ambientales Sensor de PH. Sensor de temperatura. Sensor de humedad. **Señales de salida:** Señal de estado: Indica si el sistema está listo, en proceso de medición o en reposo. Señales de lectura: Muestra los valores obtenidos de pH en pantalla o los transmite a un dispositivo externo para su registro y análisis. Señal de advertencia: Emite una alerta visual o sonora cuando el pH registrado se encuentra fuera del rango normal o indica deterioro del producto. Señal de fin de medicion:  Notifica la finalización del proceso de lectura y almacenamiento de datos. Señales de control a actuadores: Envía instrucciones a los módulos que controlan el contacto o reemplazo del hidrogel, o la activación de sistemas de notificación externa. |  **I.G , S.S , KC** **I.G , S.S , KC** |
| 23/09/25 | E | **Control:** El sistema del sensor de color supervisa constantemente las variaciones cromáticas asociadas al estado de frescura del alimento. ● Un algoritmo integrado en el módulo Arduino procesa la información captada por el sensor de color y determina el nivel de deterioro según los valores de pH estimados. ● Ópera en tres modos: monitoreo normal (alimento fresco), advertencia (inicio de descomposición) y alerta (producto no apto para consumo). ● Garantiza una supervisión en tiempo real con retroalimentación visual inmediata mediante el cambio de color, y opcionalmente, envío de datos a una interfaz o aplicación para registro y análisis.  |  **I.G , S.S , KC**  |
| 23/09/25 | E | **Electrónico (Hardware):** El sistema del sensor de color está diseñado para operar de manera confiable, continua y con bajo consumo energético: Centro de control: un microcontrolador Arduino o ESP32/ESP8266 (NodeMCU) actúa como el núcleo del sistema, coordinando la lectura del sensor de color y el procesamiento de los datos obtenidos. Sensor óptico o de pH: detecta los cambios en la tonalidad del hidrogel con antocianinas, los cuales reflejan variaciones en el pH y, por tanto, en el estado de frescura del alimento. Puede emplearse un sensor de color TCS3200 o un sensor analógico de pH, según la configuración del sistema. Módulo de visualización y registro: muestra los resultados de manera inmediata mediante indicadores LED o pantalla LCD, y registra los datos para su análisis posterior. Energía asegurada: el sistema puede funcionar conectado a una fuente eléctrica convencional o mediante batería recargable, garantizando autonomía y continuidad durante el monitoreo. |  **I.G , S.S , KC**  |
| 23/09/25 | E | **Software:** El sistema cuenta con una plataforma digital intuitiva y accesible para la supervisión y gestión de la frescura de los alimentos: **Aplicación web o móvil:** presenta gráficos claros sobre la variación del pH y el estado del color del sensor, además de emitir alertas visuales o sonoras cuando el alimento se encuentra en proceso de deterioro. **Panel de control (Dashboard):** muestra indicadores en tiempo real y un historial de mediciones, permitiendo analizar la evolución de la frescura durante el almacenamiento o transporte. **Firmware especializado:** programado en el microcontrolador (**Arduino, ESP32 o ESP8266**), gestiona la adquisición de datos del sensor de color o pH, procesa los valores y controla el envío automático a la nube. **Notificaciones automáticas vía IoT:** el sistema puede enviar alertas o informes mediante **correo electrónico, aplicación móvil o plataforma en línea**, garantizando una supervisión remota eficiente y oportuna. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Comunicaciones:** El sistema del sensor de color garantiza una conexión inalámbrica estable y segura para la transmisión continua de datos. Utiliza módulos con conectividad WiFi o Bluetooth (como ESP32 o ESP8266) que permiten enviar en tiempo real la información sobre el pH y el estado de frescura del alimento hacia la nube o una aplicación móvil. La comunicación es de doble sentido: el sistema no solo envía datos y alertas al usuario, sino que también permite recibir instrucciones o configuraciones remotas, como calibraciones, actualización de umbrales o reinicio del monitoreo. De esta manera, el usuario puede supervisar y gestionar el estado del producto a distancia, garantizando una interacción confiable, rápida y eficiente entre el sensor y la plataforma digital. |  **I.G , S.S , KC**  |
| 23/09/25 | E | **Seguridad:** La prioridad principal del sistema es garantizar un monitoreo confiable y seguro de los alimentos. El sensor de color está diseñado para operar sin contacto directo con el producto, evitando cualquier riesgo de contaminación o alteración en su composición. Además, los materiales utilizados como el hidrogel con antocianinas y el soporte protector son no tóxicos, biodegradables y compatibles con el uso alimentario. En caso de fallos eléctricos o desconexión temporal, el sistema mantiene la integridad de los datos gracias a su batería de respaldo y almacenamiento local. Asimismo, las alertas visuales y remotas permiten detectar a tiempo cualquier cambio que indique deterioro o condiciones inadecuadas de conservación. El sistema está protegido contra sobrecarga, cortocircuito y errores de transmisión, asegurando un funcionamiento estable y confiable durante toda la vida útil del sensor**.** |  **I.G , S.S , KC** |
| 23/09/25 | E | **Ergonomía:** El sensor de color ha sido diseñado con un enfoque centrado en la facilidad de uso y la accesibilidad para todo tipo de usuarios. Su estructura compacta y flexible permite una colocación sencilla sobre el envase del alimento, sin necesidad de herramientas ni conocimientos técnicos. El cambio visible de color del hidrogel proporciona una señal clara e intuitiva, fácilmente interpretable por cualquier persona, desde consumidores comunes hasta personal de control de calidad. Asimismo, la interfaz digital asociada al sistema ofrece una visualización comprensible y moderna, con gráficos y alertas simples que facilitan la interpretación del estado del producto. Esto garantiza una experiencia ergonómica, segura y cómoda, incluso para usuarios con poca experiencia tecnológica o con limitaciones visuales o motrices. |  **I.G , S.S , KC**  |
| 23/09/25 | E | **Fabricación**:La fabricación del sensor de color se desarrolla bajo criterios de sostenibilidad, durabilidad y eficiencia. Los materiales empleados como el hidrogel bioimpreso con antocianinas y el soporte polimérico transparente son biocompatibles, biodegradables y resistentes a la humedad, garantizando su estabilidad durante el almacenamiento y transporte de alimentos. El diseño modular del sistema permite reemplazar fácilmente el parche sensor o los componentes electrónicos en caso de desgaste, prolongando así su vida útil y reduciendo el impacto ambiental. La producción se plantea mediante procesos de bioimpresión y ensamble electrónico, combinando la fabricación local de las estructuras del sensor con la adquisición de módulos electrónicos estándar (como Arduino o ESP32) a proveedores especializados. Este enfoque asegura un equilibrio entre calidad, accesibilidad y sostenibilidad, optimizando tanto los costos como la disponibilidad de materiales. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Control de calidad:** Antes de su implementación, cada sistema de medición de pH con hidrogel bioimpreso pasará por un riguroso proceso de control de calidad. En primer lugar, los hidrogeles serán evaluados en cuanto a su homogeneidad, transparencia y capacidad de respuesta ante distintos niveles de pH, verificando que presenten cambios medibles y reproducibles Posteriormente, los sensores electrónicos se calibraron utilizando soluciones patrón de pH Finalmente, se realizarán pruebas de campo en entornos simulados o reales, como superficies alimentarias o medios líquidos. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Montaje:** La instalación del sensor de color es rápida, sencilla y adaptable a diferentes tipos de envases o superficies alimentarias. El diseño del parche permite adherirse fácilmente al exterior del empaque mediante materiales autoadhesivos o soportes flexibles, sin alterar la integridad del producto ni sus condiciones de conservación. El sistema incluye un manual de instalación claro e intuitivo, que orienta paso a paso el proceso de montaje, conexión del módulo electrónico (Arduino o ESP32) y calibración inicial del sensor. Gracias a su diseño compacto y modular, el montaje puede realizarse sin herramientas especializadas, lo que facilita su uso tanto en entornos domésticos como industriales.  |  **I.G , S.S , KC** |
| 23/09/25 | E | **Transporte:** El sensor de color ha sido diseñado para facilitar su distribución, almacenamiento y manipulación en diferentes etapas de la cadena alimentaria. Su estructura ligera, flexible y compacta permite transportarlo fácilmente en grandes cantidades, sin requerir condiciones especiales de espacio o peso. Cada unidad se embala utilizando materiales protectores contra golpes, humedad y polvo, garantizando la integridad del hidrogel y de los componentes electrónicos durante el traslado. Gracias a su diseño robusto y a su bajo peso, el sensor puede transportarse manualmente o mediante vehículos convencionales, asegurando una logística eficiente y económica desde el punto de fabricación hasta su aplicación final en el punto de venta o distribución. |  **I.G , S.S , KC** |
| 23/09/25 | D | **Uso:** Desea que el sensor de color está diseñado para su aplicación en entornos cotidianos de manipulación, almacenamiento y distribución de alimentos perecederos, como supermercados, plantas procesadoras, restaurantes o incluso hogares. Su funcionamiento es silencioso, pasivo y ergonómico, lo que permite un monitoreo continuo sin interferir en las actividades diarias. El cambio visible de color del hidrogel facilita una interpretación inmediata del estado de frescura, sin necesidad de dispositivos adicionales. En configuraciones avanzadas, el sistema puede conectarse a una plataforma digital para registrar los datos de pH y emitir alertas automáticas. Además, el sensor puede reemplazarse o reiniciarse manualmente después de cada uso, garantizando un manejo seguro, higiénico y accesible para todo tipo de usuario. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Mantenimiento:** Deseamos realizar una limpieza periódica de los electrodos y de la superficie del hidrogel para evitar la acumulación de residuos o contaminantes que puedan alterar las lecturas, El sistema puede incluir autodiagnósticos electrónicos, que detectan variaciones anómalas en la señal o en la respuesta del sensor, alertando al usuario sobre la necesidad de limpieza, recalibración o cambio del hidrogel. Gracias a estos cuidados simples, el dispositivo conserva su sensibilidad y fiabilidad a largo plazo. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Costos:**  El desarrollo del sensor de color se ha planificado bajo criterios de accesibilidad económica y eficiencia productiva, con el objetivo de ofrecer un dispositivo competitivo y sostenible en el mercado. Se emplean componentes electrónicos y materiales de bajo costo y fácil adquisición, como módulos Arduino o ESP, sensores ópticos estándar y biopolímeros naturales, lo que permite mantener bajos los costos de fabricación y facilitar la reposición de piezas. Gracias a su bajo consumo energético, durabilidad del hidrogel y posibilidad de reutilizar el soporte estructural, la inversión inicial puede amortizarse en un periodo estimado de dos a tres años. Esto convierte al sistema en una solución viable tanto para productores y distribuidores como para consumidores que buscan una herramienta económica y confiable para el control de la frescura alimentaria. |  **I.G , S.S , KC** |
| 23/09/25 | E | **Plazos:** El desarrollo del sensor de color se ha planificado bajo un cronograma ágil y realista, que abarca desde el diseño conceptual hasta la validación experimental del prototipo. Se estima un periodo total de dos a tres meses para completar las etapas principales del proyecto: diseño del sistema, bioimpresión del hidrogel con antocianinas, integración electrónica con el microcontrolador y realización de pruebas piloto en alimentos perecederos. Este cronograma permite evaluar la funcionalidad, sensibilidad y estabilidad del sensor antes de su implementación a mayor escala, garantizando resultados confiables en un tiempo óptimo de desarrollo. |  **I.G , S.S , KC** |

 **Tabla 1\. Lista de exigencias del proyecto**  
**7.Plan de trabajo**

**Tabla 2\. Diagrama de Gantt para el plan de trabajo del proyecto**

Referencia Bibliográfica:

[1\.](https://www.zotero.org/google-docs/?0uYIH4)	[Melnyk H, Havryliuk O, Zaets I, Sergeyeva T, Zubova G, Korovina V, et al. Red Cabbage Anthocyanin-Loaded Bacterial Cellulose Hydrogel for Colorimetric Detection of Microbial Contamination and Skin Healing Applications. Polymers \[Internet\]. enero de 2025 \[citado 15 de octubre de 2025\];17(15):2116. Disponible en: https://www.mdpi.com/2073-4360/17/15/2116](https://www.zotero.org/google-docs/?0uYIH4) 

[2\.](https://www.zotero.org/google-docs/?0uYIH4)	[Ranjbar M, Azizi Tabrizzad MH, Asadi G, Ahari H. Investigating the microbial properties of sodium alginate/chitosan edible film containing red beetroot anthocyanin extract for smart packaging in chicken fillet as a pH indicator. Heliyon. agosto de 2023;9(8):e18879.](https://www.zotero.org/google-docs/?0uYIH4) 

[3\.](https://www.zotero.org/google-docs/?0uYIH4)	[Novel colorimetric indicators based on alginate hydrogel beads containing anthocyanin for visual freshness monitoring of shrimp and minced chicken. LWT \[Internet\]. 1 de mayo de 2024 \[citado 15 de octubre de 2025\];199:116127. Disponible en: https://www.sciencedirect.com/science/article/pii/S0023643824004067](https://www.zotero.org/google-docs/?0uYIH4) 

[4\.](https://www.zotero.org/google-docs/?0uYIH4)	[Patentdocuments US. (54) PH SENSING BIOFILM (56) References Cited.](https://www.zotero.org/google-docs/?0uYIH4) 

[5\.](https://www.zotero.org/google-docs/?0uYIH4)	[KR101877606B1.pdf \[Internet\]. \[citado 15 de octubre de 2025\]. Disponible en: https://patentimages.storage.googleapis.com/0a/2d/f5/5057a68e5985f9/KR101877606B1.pdf](https://www.zotero.org/google-docs/?0uYIH4) 

[6\.](https://www.zotero.org/google-docs/?0uYIH4)	[CN115381191A.pdf \[Internet\]. \[citado 15 de octubre de 2025\]. Disponible en: https://patentimages.storage.googleapis.com/f3/04/9d/3a6c04cece10bb/CN115381191A.pdf](https://www.zotero.org/google-docs/?0uYIH4) 

[7\.](https://www.zotero.org/google-docs/?0uYIH4)	[Product: Single-Use pH Flow-Through Cell FTC-SU-HP5-US \[Internet\]. \[citado 15 de octubre de 2025\]. Disponible en: https://www.presens.de/oemcustom/detail/single-use-ph-flow-through-cell-ftc-su-hp5-us?utm\_source=chatgpt.com](https://www.zotero.org/google-docs/?0uYIH4) 

[8\.](https://www.zotero.org/google-docs/?0uYIH4)	[PhotoHA-IRG, Methacrylated Hyaluronic Acid Hydrogel Kit Photocrosslinked hyaluronic acid hydrogel (CC326 Kit Component 1\) | Sigma-Aldrich \[Internet\]. \[citado 15 de octubre de 2025\]. Disponible en: https://www.sigmaaldrich.com/PE/en/product/mm/cc3261?srsltid=AfmBOooA9rS9fz9QzakCY2mpETfeaql6c36NTdTfbvBYSw053lS6udCP](https://www.zotero.org/google-docs/?0uYIH4) 

[9\.](https://www.zotero.org/google-docs/?0uYIH4)	[GelXA \[Internet\]. CELLINK. \[citado 15 de octubre de 2025\]. Disponible en: https://www.cellink.com/product/gelxa/ l](https://www.zotero.org/google-docs/?0uYIH4)**es:**

