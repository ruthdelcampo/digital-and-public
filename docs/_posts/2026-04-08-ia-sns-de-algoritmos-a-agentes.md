---
layout: default
title: "La IA en el SNS: de algoritmos a skills, de skills a agentes"
date: 2026-04-11
author: Ruth del Campo
lang: es
---

# La IA en el SNS: de algoritmos a skills, de skills a agentes

---

Estos días de vacaciones me han dado algo que últimamente escasea: tiempo para leer con calma. Entre las lecturas que tenía pendientes estaba la **[Estrategia de Inteligencia Artificial para el Sistema Nacional de Salud](https://www.sanidad.gob.es/areas/saludDigital/doc/eIASNS_v13.pdf)** (eIASNS), publicada por el Ministerio de Sanidad y aprobada por el Consejo Interterritorial del SNS en noviembre de 2025.

La leo con especial interés porque me apasiona la salud digital y me fascina como a muchísima gente cómo la IA va a revolucionar todos los procesos actuales, siendo la salud uno de los campos con mayor impacto. 

---

## Una estrategia que parte de la realidad

Me ha sorprendido positivamente la honestidad del diagnóstico de partida. Antes de proponer nada, el Ministerio y las comunidades autónomas han hecho los deberes: sesiones bilaterales con cada CCAA, cuestionarios técnicos y normativos a los servicios de salud y sus proveedores, análisis de licitaciones y proyectos. El resultado es un inventario de **155 algoritmos de IA** ya operativos en el SNS — 81 comerciales, 56 de desarrollo propio y 18 sin clasificar — con un desglose por especialidad clínica, fase del proceso asistencial y grado de madurez.

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

En la conversación actual sobre IA estos tres conceptos se mezclan con frecuencia. Merece la pena definirlos:

| | **Algoritmo** | **Skill** | **Agente** |
|---|---|---|---|
| **Qué es** | Un modelo entrenado para una tarea específica (clasificar imágenes, predecir reingresos, detectar arritmias) | Conocimiento clínico codificado en instrucciones estructuradas: reglas, protocolos, límites, formato de salida | Un sistema de IA que ejecuta uno o varios skills, accede a datos, razona y produce resultados dentro de un flujo de trabajo |
| **Quién lo crea** | Data scientists e ingenieros de ML, con datos de entrenamiento e infraestructura de computación | Expertos del dominio — clínicos, normativistas, gestores — que codifican su conocimiento | Equipos técnicos que integran modelos, skills y acceso a sistemas de información |
| **Quién lo usa** | El profesional sanitario, a través de una integración técnica previa | El agente de IA, que aplica el skill cuando el contexto lo requiere | El profesional sanitario, interactuando directamente — normalmente en lenguaje natural |
| **Cómo se actualiza** | Reentrenamiento con datos nuevos (costoso, lento — meses) | Actualización del texto y las reglas (ágil, auditable — días) | Actualización de skills y/o del modelo subyacente |
| **Cómo se audita** | Métricas de rendimiento del modelo — el modelo en sí es opaco | Las instrucciones son legibles: se puede leer exactamente qué reglas sigue | Trazabilidad completa: qué skill se aplicó, qué datos se consultaron, qué resultado se produjo |

En la práctica, un agente de apoyo clínico en una consulta de atención primaria podría usar varios skills simultáneamente — triaje, revisión de medicación, codificación diagnóstica — y también invocar algoritmos específicos cuando los necesita, como un modelo de predicción de riesgo cardiovascular. El profesional interactúa con el agente, no con los algoritmos individuales.

---

## Por qué el SNS necesita pensar en skills y agentes

Esto no es una cuestión terminológica. Tiene consecuencias prácticas directas.

**Los algoritmos necesitan data scientists en el destino.** Para desplegar un algoritmo de clasificación de imágenes en un hospital, necesitas un equipo técnico capaz de integrarlo con el PACS, validar su rendimiento con la población local, monitorizar la deriva del modelo y resolver incidencias. Eso limita el despliegue a los centros con capacidad técnica suficiente. El inventario de 155 algoritmos en todo el SNS — para un sistema que atiende a **48 millones de personas** — refleja esa limitación.

**Los agentes basados en skills escalan.** La interfaz de un agente de IA es el lenguaje natural — la misma que millones de personas ya usan con ChatGPT, Claude o Gemini. El skill encapsula la complejidad técnica y normativa; el profesional no necesita saber cómo funciona el modelo por debajo, de la misma manera que no necesita saber cómo funciona el motor de búsqueda de su Historia Clínica Electrónica. Esto cambia radicalmente la **escala de despliegue posible**.

**Los skills se actualizan sin reentrenar.** Si cambia una guía de práctica clínica — algo que ocurre regularmente — actualizar un skill significa modificar sus instrucciones y reglas. Actualizar un algoritmo entrenado significa reentrenarlo con datos nuevos, revalidarlo y redesplegar. La primera opción se mide en días; la segunda, en meses.

**Los skills son auditables por diseño.** La trazabilidad que exige el AI Act — saber por qué un sistema de IA produjo un resultado concreto — es mucho más sencilla con un skill documentado cuyas reglas se pueden leer, que con un modelo de deep learning cuya lógica interna es opaca.

Y hay un argumento que conecta con la propia arquitectura de la eIASNS: **los skills encajan naturalmente en el modelo de gobernanza federada del SNS**. Se pueden desarrollar a nivel estatal con conocimiento clínico consensuado, extender a nivel autonómico con las particularidades de cada servicio de salud, y parametrizar a nivel de centro. Es gestión multinivel aplicada al conocimiento clínico computabilizado.

---

## Qué podría construir el SNS: tres ejemplos concretos

Para que esto no quede en abstracción, pensemos en agentes que podrían desarrollarse a nivel estatal — basados en guías clínicas y protocolos consensuados del SNS — y desplegarse en las CCAA:

**Un agente de apoyo a la prescripción en insuficiencia cardíaca**, basado en la Guía de Práctica Clínica del SNS. El skill contendría el algoritmo de decisión terapéutica de la guía (primera línea, segunda línea, ajustes por función renal, contraindicaciones), las interacciones medicamentosas relevantes y los criterios de derivación a cardiología. El agente consultaría los datos del paciente en la Historia Clínica Electrónica y le diría al médico de primaria: *"Según la guía, en este perfil de paciente con FEVI reducida y función renal preservada, estaría indicado iniciar IECA + betabloqueante. El paciente actualmente solo tiene prescrito enalapril. ¿Quieres ver el razonamiento completo?"* El skill estatal define la lógica clínica; la extensión autonómica lo conecta con la HCE de cada CCAA; la extensión de centro ajusta el formulario local.

**Un agente de codificación diagnóstica asistida**, basado en CIE-10-ES y las reglas de codificación del CMBD. Leería la nota clínica del alta, propondría los códigos diagnósticos y de procedimiento, y marcaría las dudas de clasificación. Hoy la codificación la hacen documentalistas clínicos con alta carga de trabajo y escasez de personal. Un agente con un skill bien construido propondría una codificación inicial que el documentalista revisa y valida. No necesita un algoritmo entrenado *ad hoc* sino un modelo de lenguaje con las instrucciones correctas y acceso a la tabla CIE-10-ES completa.

**Un agente de adherencia terapéutica para pacientes crónicos**, que interactuaría con el paciente a través de la app de salud autonómica, le recordaría la medicación, le haría preguntas estandarizadas de seguimiento (cuestionarios validados como el Morisky-Green), detectaría señales de alarma y las comunicaría al equipo asistencial. El skill estatal incluiría los cuestionarios validados y las reglas de derivación; la extensión autonómica lo conectaría con la carpeta de salud digital del ciudadano.

En los tres casos, el valor diferencial no está en el modelo de IA — que puede ser un modelo fundacional existente — sino en el **conocimiento clínico codificado en el skill**. Y ese conocimiento es exactamente lo que el SNS tiene y ninguna empresa tecnológica puede replicar: guías de práctica clínica consensuadas, protocolos validados por 17 servicios de salud, estándares de codificación adaptados al contexto español.

---

## Dos mundos de IA que conviven (y que necesitan reglas distintas)

La estrategia inventarió 155 algoritmos comerciales y 81 de desarrollo propio. Los menciona, pero no profundiza en una diferencia fundamental: **se gobiernan de forma completamente distinta**.

**IA comercial**: la que viene embebida en el dispositivo médico. Un ecógrafo, un retinógrafo con IA incorporada. Viene certificada (marcado CE, MDR/IVDR), la responsabilidad recae en el fabricante. El hospital la consume como usuario.

**IA colaborativa**: la que construye el SNS. Un equipo del Hospital La Paz que desarrolla un modelo de predicción de reingresos. Tres CCAA que entrenan federadamente un detector de melanomas. Aquí el SNS es el responsable, el código es suyo, las decisiones de diseño son suyas.

Para la IA colaborativa, la apuesta debería ser **abierta por defecto**: código fuente completo, referencias a datos de entrenamiento, notebooks de validación. No por ideología, sino por razones prácticas: el AI Act exige transparencia para sistemas de alto riesgo; con 17 CCAA, la reutilización es supervivencia; la validación científica necesita reproducibilidad; el entrenamiento federado que propone la estrategia necesita código compartido; y el dinero es público.

---

## El Marketplace como registry versionado

La estrategia propone un Marketplace IASNS. Pero ¿qué es exactamente? Un PDF con una lista de algoritmos no sirve. Una web informativa tampoco.

Lo que necesita el SNS es un **registry versionado** — conceptualmente similar a lo que npm es para JavaScript o Docker Hub para contenedores, pero adaptado al contexto sanitario. Un sitio donde las skills se publican con su manifiesto, se descubren, se evalúan y se despliegan de forma estandarizada.

### Dos tracks, un registry

| | Track abierto (desarrollo propio) | Track comercial |
|---|---|---|
| **Qué se publica** | Código fuente, datos de entrenamiento (o referencia), validación | Metadatos, documentación, certificaciones |
| **Licencia** | Open source | Propietaria |
| **Responsabilidad** | CCAA que desarrolla + Oficina IASNS | Fabricante |
| **Normativa principal** | AI Act | AI Act + MDR/IVDR + Marcado CE |

### El Sello SNS como validación con dos capas

La estrategia propone un Sello SNS con cinco dimensiones (normativa, tecnológica, asistencial, seguridad, económica). Para hacerlo operativo, debería funcionar como un proceso de validación en dos capas:

**Capa automática** (como un pipeline de CI/CD):
- Clasificación de riesgo según AI Act
- Completitud de documentación y manifiesto
- Calidad de código y escaneo de seguridad
- Métricas de sesgo sobre datasets de referencia

**Capa humana** (comité de evaluación):
- Validación clínica: ¿resuelve el problema que dice resolver?
- Revisión ética: ¿hay sesgos no detectados automáticamente?
- Cumplimiento normativo: ¿encaja en el marco MDR si aplica?

Una skill puede publicarse en el Marketplace sin sello — tal como dice la estrategia. Pero el sello indica que ha superado la validación completa. Y como las skills evolucionan, el sello se reevalúa con cada versión mayor.

---

## El workflow: quién hace qué, y cuándo

Este es el hueco más grande de la estrategia. Propone estructuras de gobernanza (Oficina IASNS, Oficinas IA CCAA, coordinadores en centros), pero no concreta el flujo operativo. Aquí va una propuesta:

### 1. Identificación de necesidad
**Quién:** profesionales clínicos, gestores hospitalarios, planificadores de CCAA.

Un médico detecta que pasa demasiado tiempo clasificando lesiones dermatológicas. Un gestor hospitalario ve que los reingresos a 30 días son prevenibles. Un planificador de CCAA necesita predecir la demanda de UCI en temporada de gripe.

La propuesta se formaliza y la Oficina IA de la CCAA la prioriza. **Paso clave:** antes de desarrollar, consultar el Marketplace. Quizás otra CCAA ya lo ha resuelto.

### 2. Desarrollo
**Quién:** equipos mixtos clínico-técnicos del hospital, grupos de investigación, equipos TIC de la CCAA.

Se desarrolla usando las plantillas estándar del SNS (estructura de skill, manifiesto, tests mínimos). Si necesita datos de varios centros, se coordina el entrenamiento federado a través de la Oficina IASNS.

La Oficina proporciona plantillas, guías, acceso a infraestructura compartida y asesoramiento normativo. No desarrolla ella misma — habilita.

Aquí hay un matiz importante: **no todo requiere entrenar un modelo desde cero**. Muchas de las skills más útiles — como los tres ejemplos anteriores — consisten en codificar conocimiento clínico en instrucciones estructuradas que un modelo fundacional existente puede ejecutar. Esto cambia quién puede desarrollar: no solo data scientists, sino expertos clínicos con el apoyo técnico adecuado.

### 3. Validación clínica
**Quién:** equipo clínico del hospital + revisores independientes.
**Dónde:** en los espacios controlados de pruebas que propone la estrategia.

Estudio prospectivo, comparación con el estándar de cuidado actual, test de sesgos por demografía, evaluación de explicabilidad. El resultado es un informe de validación que acompaña a la skill en el registry.

### 4. Revisión y Sello SNS
**Quién:** Oficina IASNS + Oficina IA de la CCAA.

Checks automáticos + revisión humana. Si pasa → Sello SNS. Si no → feedback específico para iterar.

### 5. Publicación y despliegue
La Oficina IASNS publica la skill en el Marketplace. Cualquier CCAA puede descubrirla, evaluarla y decidir si la adopta. El despliegue lo hace cada CCAA en su infraestructura, usando paquetes estandarizados (contenedores) y APIs documentadas.

### 6. Monitorización y ciclo de vida
- **El hospital** monitoriza la operación diaria (¿funciona? ¿responde?).
- **La CCAA** monitoriza el rendimiento clínico (¿sigue siendo precisa? ¿hay drift?).
- **El Ministerio** agrega métricas nacionales (los indicadores 2027/2030 de la estrategia).

Cuando los datos cambian o el rendimiento se degrada, se publica nueva versión. Si una skill deja de ser útil o segura, se depreca en el registry con aviso a todos los que la tienen desplegada.

### El papel de cada nivel

| Nivel | Rol | Analogía |
|---|---|---|
| **Hospital** | Identifica, desarrolla, valida, despliega, monitoriza | El equipo de producto |
| **CCAA** | Prioriza, coordina, proporciona infraestructura | La plataforma |
| **Ministerio** | Estándares, Sello, Marketplace, métricas nacionales | El registry + governance |

---

## La oportunidad de los modelos abiertos

Hay un elemento que la estrategia no aborda y que encaja perfectamente en esta lógica: la creciente disponibilidad de **modelos fundacionales de código abierto**.

Modelos como Mistral (francés, europeo), LLaMA de Meta, o los que puedan surgir de iniciativas como ALIA (el proyecto español de modelos de lenguaje) o del programa europeo EuroHPC, ofrecen una base sobre la que los skills del SNS podrían operar **sin dependencia de licenciamiento costoso** de proveedores comerciales.

Esto no es un detalle menor. Si cada hospital necesita una licencia de un modelo propietario para ejecutar agentes de IA, el coste de despliegue a escala del SNS sería prohibitivo. Pero si los skills se diseñan para funcionar sobre modelos abiertos — que se pueden ejecutar en infraestructura propia o soberana — la ecuación económica cambia completamente.

La infraestructura del **[Espacio Nacional de Datos de Salud](https://digital.gob.es/digitalizacion/la-economia-del-dato/espacio-nacional-datos-salud)** (ENDS), que ya se está construyendo con una inversión de 100 millones de euros del Plan de Atención Digital Personalizada, podría servir no solo como plataforma de datos sino como infraestructura de ejecución de estos modelos y agentes. La inversión en capacidad de computación ya está prevista; lo que falta es articular para qué se va a usar.

---

## Lo que hace falta para que esto funcione

La estrategia pone la primera piedra. Para que el modelo de skills y agentes funcione, necesita complementarse con:

1. **Una definición estándar de skill** (manifiesto, interfaz, documentación mínima) — consensuada entre CCAA.
2. **Infraestructura de compute compartida**, aprovechando el ENDS, para que los hospitales puedan desarrollar y ejecutar modelos sin depender de presupuestos individuales para GPUs.
3. **Un registry real**, no un catálogo. Con versionado, APIs de búsqueda, y mecanismos de despliegue estandarizados.
4. **Un marco de entrenamiento federado operativo**, no solo mencionado. Herramientas, protocolos, gobernanza de datos.
5. **Capacitación dual**: no solo en uso de IA (como plantea la estrategia), sino en creación de skills para expertos clínicos y desarrollo técnico para equipos hospitalarios.

---

## Un paso adelante

Quiero cerrar como empecé: reconociendo el mérito. La eIASNS es un ejercicio serio de planificación interterritorial en un ámbito que avanza a una velocidad que dificulta cualquier ejercicio estratégico. El Ministerio de Sanidad y las comunidades autónomas han conseguido algo que no es fácil: consensuar una visión común sobre cómo integrar la IA en un sistema sanitario descentralizado, con un presupuesto de 297 millones de euros y unos indicadores con hitos concretos.

Mi reflexión no pretende ser una crítica sino una aportación: creo que la próxima iteración de la estrategia — o quizá su primer plan de acción operativo — se beneficiaría de incorporar el concepto de skills y agentes como pilar del despliegue. No porque los algoritmos no tengan su lugar (lo tienen, especialmente en imagen médica y modelos predictivos), sino porque los agentes permiten escalar la IA a los profesionales y pacientes del SNS de una forma que los algoritmos solos no pueden.

El SNS no va a ganar la carrera de los modelos de IA. Pero tiene algo que ninguna empresa tecnológica puede replicar: **el conocimiento clínico colectivo de 17 servicios de salud que atienden a 48 millones de personas**, y la legitimidad institucional para convertirlo en estándares. Ese conocimiento, hoy atrapado en PDFs de guías clínicas y en la cabeza de profesionales con experiencia, es el activo que hay que computabilizar.

De algoritmos a skills. De skills a agentes. De conocimiento pasivo a conocimiento activable. Ese es el siguiente paso.

---

*Ruth es funcionaria de la Administración General del Estado. Las opiniones expresadas en este blog son personales y no representan la posición oficial de ninguna institución.*
