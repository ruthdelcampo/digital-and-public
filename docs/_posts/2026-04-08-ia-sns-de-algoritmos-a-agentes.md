---
layout: default
title: "La IA en el SNS: de algoritmos a skills, de skills a agentes"
date: 2026-04-11
author: Ruth del Campo
lang: es
---

# La IA en el SNS: de algoritmos a skills y agentes

---

Estos días de vacaciones he aprovechado para leer la **[Estrategia de Inteligencia Artificial para el Sistema Nacional de Salud](https://www.sanidad.gob.es/areas/saludDigital/doc/eIASNS_v13.pdf)** (eIASNS), publicada por el Ministerio de Sanidad y aprobada por el Consejo Interterritorial del SNS en noviembre de 2025.

La leo con especial interés porque me apasiona la salud digital y me fascina como a muchísima gente cómo la IA va a revolucionar todos los procesos actuales, siendo la salud uno de los campos con mayor impacto. 

---

## Una estrategia que parte de la realidad

El Ministerio y las comunidades autónomas han hecho los deberes: sesiones bilaterales con cada CCAA, cuestionarios técnicos y normativos a los servicios de salud y sus proveedores, análisis de licitaciones y proyectos. El resultado es un inventario de **155 algoritmos de IA** ya operativos en el SNS — 81 comerciales, 56 de desarrollo propio y 18 sin clasificar — con un desglose por especialidad clínica, fase del proceso asistencial y grado de madurez.

Esa foto, imperfecta como toda primera instantánea, tiene valor: demuestra que la IA no es algo que "va a llegar" al SNS. Ya está aquí. De forma desigual, fragmentada, con diferencias notables entre comunidades autónomas, pero aquí.

La estrategia se apoya en un **marco de gobernanza que ya existe y funciona**: la Comisión de Salud Digital del Consejo Interterritorial, el modelo de liderazgos compartidos de la Estrategia de Salud Digital, y las estructuras de coordinación entre el Ministerio y las CCAA que llevan operando desde 2021. 

El **mapa del marco regulatorio** es una sección bastante útil donde se muestran los solapamientos, obligaciones cruzadas y niveles de riesgo entre las diferentes regulaciones europeas.

Además, **la eIASNS es la primera estrategia sectorial de inteligencia artificial impulsada desde un ministerio para su ámbito competencial específico**. Existe la Estrategia Nacional de IA (la ENIA de 2020, actualizada en 2024), coordinada por SEDIA con carácter transversal. Pero ningún otro ministerio ha publicado una estrategia de IA adaptada a las particularidades de su sector.

---

## Una observación desde abril de 2026

Dicho todo lo anterior — y reconocido el mérito — hay algo que me llama la atención al leer el documento hoy.

La eIASNS habla de **algoritmos**. Consistentemente. Los inventaría, los clasifica, los cataloga en un Marketplace, los evalúa para otorgarles un Sello SNS. El lenguaje es coherente con el del Reglamento de IA europeo, que también habla de "sistemas de IA" como unidades discretas que se registran, se clasifican por riesgo y se supervisan.

Pero el mundo de la implementación práctica de la IA ha evolucionado notablemente. Lo que hoy están desplegando las organizaciones no son tanto algoritmos aislados como **agentes de IA**: sistemas que combinan modelos fundacionales con instrucciones específicas del dominio, acceso a datos en contexto, y capacidad de acción dentro de flujos de trabajo reales.

La diferencia entre pensar en algoritmos y pensar en agentes tiene implicaciones directas sobre **quién puede desarrollar, quién puede desplegar y quién puede usar** la IA en el SNS.

---

## Algoritmos, skills y agentes: tres conceptos que conviene separar


| | **Algoritmo** | **Skill** | **Agente** |
|---|---|---|---|
| **Qué es** | Un modelo entrenado para una tarea específica (clasificar imágenes, predecir reingresos, detectar arritmias) | Conocimiento clínico codificado en instrucciones estructuradas: reglas, protocolos, límites, formato de salida | Un sistema de IA que ejecuta uno o varios skills, accede a datos, razona y produce resultados dentro de un flujo de trabajo |
| **Quién lo crea** | Data scientists e ingenieros de ML, con datos de entrenamiento e infraestructura de computación | Expertos del dominio — clínicos, normativistas, gestores — que codifican su conocimiento | Equipos técnicos que integran modelos, skills y acceso a sistemas de información |
| **Quién lo usa** | El profesional sanitario, a través de una integración técnica previa | El agente de IA, que aplica el skill cuando el contexto lo requiere | El profesional sanitario, interactuando directamente — normalmente en lenguaje natural |
| **Cómo se actualiza** | Reentrenamiento con datos nuevos (costoso, lento — meses) | Actualización del texto y las reglas (ágil, auditable — días) | Actualización de skills y/o del modelo subyacente |
| **Cómo se audita** | Métricas de rendimiento del modelo — el modelo en sí es opaco | Las instrucciones son legibles: se puede leer exactamente qué reglas sigue | Trazabilidad completa: qué skill se aplicó, qué datos se consultaron, qué resultado se produjo |

En la práctica, un agente de apoyo clínico en una consulta de atención primaria podría usar varios skills simultáneamente — triaje, revisión de medicación, codificación diagnóstica — y también invocar algoritmos específicos cuando los necesita, como un modelo de predicción de riesgo cardiovascular. El profesional interactúa con el agente, no con los algoritmos individuales.

---

## Por qué el SNS necesita pensar más en skills y agentes que en algoritmos


**Los algoritmos necesitan data scientists en el destino.** Para desplegar un algoritmo de clasificación de imágenes en un hospital, necesitas un equipo técnico capaz de integrarlo con el PACS, validar su rendimiento con la población local, monitorizar la deriva del modelo y resolver incidencias. Eso limita el despliegue a los centros con capacidad técnica suficiente. El inventario de 155 algoritmos en todo el SNS — para un sistema que atiende a **48 millones de personas** — refleja esa limitación.

**Los agentes basados en skills escalan.** La interfaz de un agente de IA es el lenguaje natural — la misma que millones de personas ya usan con ChatGPT, Claude o Gemini. El skill encapsula la complejidad técnica y normativa; el profesional no necesita saber cómo funciona el modelo por debajo, de la misma manera que no necesita saber cómo funciona el motor de búsqueda de su Historia Clínica Electrónica. Esto cambia radicalmente la **escala de despliegue posible**.

**Los skills se actualizan sin reentrenar.** Si cambia una guía de práctica clínica — algo que ocurre regularmente — actualizar un skill significa modificar sus instrucciones y reglas. Actualizar un algoritmo entrenado significa reentrenarlo con datos nuevos, revalidarlo y redesplegar. La primera opción se mide en días; la segunda, en meses.

**Los skills son auditables por diseño.** La trazabilidad que exige el AI Act — saber por qué un sistema de IA produjo un resultado concreto — es mucho más sencilla con un skill documentado cuyas reglas se pueden leer, que con un modelo de deep learning cuya lógica interna es opaca.

Y hay un argumento que conecta con la propia arquitectura de la eIASNS: **los skills encajan naturalmente en el modelo de gobernanza federada del SNS**. Se pueden desarrollar a nivel estatal con conocimiento clínico consensuado, extender a nivel autonómico con las particularidades de cada servicio de salud, y parametrizar a nivel de centro. Es gestión multinivel aplicada al conocimiento clínico computabilizado.

---

## La oportunidad de los modelos abiertos para los agentes inhouse

Hay un elemento adicional que el documento no aborda y que encaja muy bien: la creciente disponibilidad de **modelos fundacionales de código abierto**.

Hoy en día los modelos abiertos son una opción muy sólida para proyectos con uso intensivo de IA y recursos limitados. A pesar de que no son modelos frontera, las capacidades que ofrecen suelen estar tan solo unos meses por detrás de los frontera comerciales. Por ello, la funcionalidad de modelos actuales como Opus 4.6 podrá estar en abierto en un año, y la flexibilidad de despliegue de un modelo abierto es mucho mayor.

Esto no es un detalle menor. Si cada hospital necesita una licencia de un modelo propietario para ejecutar los agentes de IA, el coste de despliegue a escala del SNS sería alto. Pero si los skills se diseñan para funcionar sobre modelos abiertos — que se pueden ejecutar en infraestructura propia — la ecuación económica cambia.

La infraestructura del **[Espacio Nacional de Datos de Salud](https://digital.gob.es/digitalizacion/la-economia-del-dato/espacio-nacional-datos-salud)** (ENDS) podría servir como plataforma de datos e infraestructura de ejecución de estos modelos y agentes.

## Un paso adelante

 El Ministerio de Sanidad y las comunidades autónomas han conseguido algo que no es fácil: consensuar una visión común sobre cómo integrar la IA en un sistema sanitario descentralizado, con un presupuesto comprometido de cientos de millones de euros e indicadores con hitos concretos.

La próxima iteración de la estrategia — o quizá su primer plan de acción operativo — se beneficiaría de incorporar el concepto de agentes y skills como pilar del despliegue. No porque los algoritmos no tengan su lugar, sino porque los agentes permiten escalar la IA a los profesionales y pacientes del SNS de una forma que los algoritmos solos no pueden. Es decir, el impacto en el SNS va a ser más directo y accionable.

El SNS no va a ganar la carrera de los modelos de IA. Pero tiene algo muy valioso: el conocimiento clínico colectivo de 17 servicios de salud que atienden a 48 millones de personas, y la legitimidad institucional para convertirlo en estándares.

De algoritmos a agentes. De conocimiento tecnológico a conocimiento activable.

---
