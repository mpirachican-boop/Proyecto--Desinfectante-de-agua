# PROTOTIPO DESINFECTANTE DE AGUA

**Integrantes:**
* Mariana Isabella Pirachicán Mahecha
* Angel Steeven Gachancipá García
* Alejandro

**Institución:** Universidad Nacional de Colombia  
**Facultad:** Ingeniería — Taller de Ingeniería Electrónica  
**Docente:** Johnny Cubides  
**Fecha:** 6 de Noviembre de 2026  

---

## 1. Situación Problema

En la vereda Las Lajas, ubicada en el municipio de Supatá, varias familias utilizan aguas provenientes de fuentes naturales (nacederos o ríos) para su abastecimiento diario. Sin embargo, esta agua no cuenta con las medidas de seguridad requeridas para el consumo humano y transporta patógenos que afectan la salud comunitaria. Ante la falta de un servicio eficiente de acueducto y alcantarillado, las familias se ven obligadas a recurrir a estas fuentes desprotegidas.

Esta situación refleja una brecha estructural a nivel nacional. Según datos de la Encuesta Nacional de Calidad de Vida (ECV) del DANE, solo el **59.9%** de los habitantes de zonas rurales en Colombia cuentan con acceso a la red de acueducto, frente al **95%** en cabeceras municipales. Esta disparidad obliga al **19.5%** de la población rural a abastecerse de ríos, quebradas o nacederos. Asimismo, el Índice de Riesgo de la Calidad del Agua (IRCA) del Ministerio de Salud registró un valor del **37.5%** en zonas rurales (categorizado como riesgo alto), lo que evidencia la urgencia de implementar soluciones locales de potabilización.

---

## 2. Marco de Referencia Global

El proyecto se alinea directamente con los Objetivos de Desarrollo Sostenible (ODS) de la ONU:

* **ODS 6 (Agua Limpia y Saneamiento):** Busca garantizar la disponibilidad, gestión sostenible y saneamiento del agua para todos, ofreciendo una fuente tratada e higiénica.
* **ODS 3 (Salud y Bienestar):** Reduce la incidencia de enfermedades gastrointestinales e infecciosas provocadas por el consumo de agua contaminada, mejorando la calidad de vida en comunidades vulnerables.

---

## 3. Descripción del Prototipo

Se plantea un dispositivo automatizado capaz de desinfectar el agua recolectada (previamente filtrada) mediante dosificación controlada de cloro. El prototipo está construido sobre una estructura con tanque de 5L, mangueras plásticas, motor de mezcla, sensores de nivel/calidad, compuertas de paso y un microcontrolador **ESP32**.

---

## 4. Requerimientos Funcionales (RF)

| ID | Descripción del Requerimiento | Criterio Verificable |
| :--- | :--- | :--- |
| **RF1** | Controlar la cantidad de cloro suministrada mediante una minibomba peristáltica de 12V. | Dosificación exacta de solución de cloro según el volumen de agua ingresado (5 Litros). |
| **RF2** | Temporizar el tiempo de reposo del agua con cloro. | Mantener el agua retenida durante 30 minutos continuos y emitir una alerta sonora al finalizar. |
| **RF3** | Homogeneizar la mezcla de agua y cloro dentro del tanque. | Activación del mezclador/hélice durante el ciclo de dosificación. |
| **RF4** | Controlar el flujo de entrada y salida del agua. | Apertura y cierre de compuertas electromecánicas de acuerdo con la señal de los sensores. |

---

## 5. Requerimientos No Funcionales (RNF)

| ID | Descripción del Requerimiento | Atributo de Calidad / Restricción |
| :--- | :--- | :--- |
| **RNF1** | Garantizar la seguridad química del agua tratada. | Mantener el nivel de cloro residual dentro de los límites seguros para consumo humano. |
| **RNF2** | Optimizar el consumo energético del sistema. | Alimentación continua a 12V DC con bajo consumo, integrable a baterías o paneles solares. |
| **RNF3** | Asegurar la resistencia química y mecánica de los componentes. | Materiales resistentes a la corrosión por cloro y exposición al agua (PETG, silicona, PVC). |
| **RNF4** | Permitir mantenibilidad y facilidad de limpieza. | Diseño con acceso rápido para la recarga del tanque de cloro y lavado del contenedor principal. |

---

## 6. Evaluación de Viabilidad de Requerimientos

* **Prototipo (PMV):** Valida conceptual y técnicamente el uso del microcontrolador ESP32, temporización, bombeo peristáltico y mezclado en laboratorio.
* **Producto Final:** Requerirá la sustitución de polímeros por materiales con certificación de grado alimentario, integración de sensores de cloro residual libre y cumplimiento de la normativa sanitaria nacional (RAS).

---

## 7. Business Model Canvas

| Bloque del Canvas | Descripción Aplicada al Proyecto |
| :--- | :--- |
| **Socios Clave** | Junta de Acción Comunal de la vereda Las Lajas, Alcaldía de Supatá, proveedores de electrónica. |
| **Actividades Clave** | Programación del ESP32, diseño de circuitos de potencia, ensamblaje mecánico de tanques y mezclador. |
| **Recursos Clave** | Microcontrolador ESP32, bomba peristáltica 12V, sensores, impresora 3D y equipo proyectista. |
| **Propuesta de Valor** | Sistema automatizado y económico de desinfección de agua para fuentes no tratadas en fincas rurales. |
| **Relaciones con Clientes** | Capacitaciones a familias rurales en uso, recarga de cloro y mantenimiento básico del kit. |
| **Canales** | Demostraciones comunitarias, ferias académicas y alianzas con comités de agua veredales. |
| **Segmento de Clientes** | Familias rurales de la vereda Las Lajas y propietarios de fincas en Supatá sin acueducto. |
| **Estructura de Costos** | Adquisición de electrónica (ESP32, sensores, bomba), insumos mecánicos y horas de desarrollo. |
| **Fuentes de Ingresos** | Venta directa del kit desinfectante para fincas y servicios de instalación/mantenimiento. |

---

## 8. Referencias

1. Naciones Unidas, "Objetivos de Desarrollo Sostenible", 2026.
2. DANE, "Encuesta Nacional de Calidad de Vida (ECV) 2024," Bogotá, Colombia, 2025.
3. Instituto Nacional de Salud, "Informe Nacional de Calidad del Agua para Consumo Humano (INCA)," Bogotá, Colombia, 2025.
