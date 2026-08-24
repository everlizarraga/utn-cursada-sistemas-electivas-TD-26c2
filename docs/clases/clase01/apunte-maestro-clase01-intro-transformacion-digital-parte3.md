# 📚 Apunte Maestro — Clase 01 · Introducción: Transformación Digital en las organizaciones

## Parte 3 de 3 — El mapa de la materia, el vocabulario plantado y las reglas de la cursada

**Materia:** Transformación Digital (K3561) — 2C 2026 · **Clase 01** — lunes 10/8, virtual

**Esta parte cubre:** el mapa de las 9 unidades y cómo se van a recorrer, el vocabulario que quedó plantado al presentarlas (ERP y "sistema de gestión", niveles de decisión, organizaciones data-driven, on-premise/cloud/SaaS, procesos agénticos, reportes de analistas, los tiers del mercado), el adelanto de la historia de la IA, la conexión con el resto de la carrera, y **todas las reglas operativas de la cursada**: modalidad, calendario, Liga TD, TP integrador. Cierra con el **checkpoint de la clase completa** (las tres partes).

**Se apoya en:** Partes 1 y 2 (casos, lecciones y marco conceptual). Lo ya explicado se cita, no se repite.

**Leyenda:** 🔴 central-evaluable · 🟡 secundario · 🟢 mencionado al pasar · 🕳️ madriguera (tangente controlada)

---

## 1. 🟡 El mapa de la materia: 9 unidades (que se van a cruzar)

El programa está organizado en nueve unidades, pero con una aclaración importante de entrada: **en la práctica los temas se van a entrecruzar**. Las unidades 7, 8 y 9 —transformación digital, innovación, tecnologías emergentes e IA— no quedan para el final: sus temas se van cruzando dentro de todas las clases anteriores, con ejemplos en cada una. El orden formal es una guía, no un recorrido rígido.

| Unidad | Nombre | Qué cubre (síntesis) |
|---|---|---|
| **1** | Sistemas Empresariales | La empresa como sistema; niveles de planificación y decisión (estratégico/táctico/operativo); Balanced Scorecard, KPIs, dashboards estratégicos; organizaciones *data-driven*; introducción a Industria 4.0. |
| **2** | Implementar un ERP | Qué son los ERP y qué rol cumplen; ¿desarrollar a medida o comprar?, ¿infraestructura propia o nube?; cómo se elige e implementa un software empresarial; historia, módulos, ERP in-memory y real-time; SaaS; "Intelligent ERP" con IA; caso de negocio, costos y retorno de inversión; reportes de analistas y jugadores del mercado. |
| **3** | Plataforma Ventas | Procesos de venta y preventa; marketing digital; qué son los CRM; integración con e-commerce, puntos de venta y pasarelas de pago. |
| **4** | Plataforma Compras | Procesos de compras; *supply chain* (cadena de abastecimiento); logística; e-procurement; rendimiento de proveedores; impresión 3D y blockchain en la cadena. |
| **5** | Plataforma Producción | Módulo de producción de un ERP; previsión de demanda; planeamiento y control; integración con sistemas industriales (SCADA, MES, PLCs); MRP; sensorización, IIoT, mantenimiento predictivo con IA. |
| **6** | Plataforma Contable-Financiera | Contabilidad y finanzas en los sistemas de gestión; tesorería, consolidación, controlling, activos fijos; cashflow, cuentas a pagar/cobrar; dashboards de CFO; indicadores financieros; las fintech como disruptor. |
| **7** | La transformación digital en las organizaciones | La 4ta revolución industrial; qué es y qué no es TD; organizaciones ambidiestras; pensamiento exponencial y diseño de futuros; unicornios digitales; casos de éxito y fracaso. |
| **8** | Cómo innovan las organizaciones | Design Thinking (diseño centrado en las personas); experimentación y el error como parte del proceso; innovación abierta vs cerrada; hiper-personalización; crowdsourcing y gamificación. |
| **9** | Tecnologías emergentes | Machine learning, RPA, big data, computer vision, realidad aumentada, IoT, procesamiento del lenguaje natural, biometría digital, blockchain, IA generativa, asistentes virtuales, video analytics — con casos de uso reales por industria y su impacto en procesos y experiencia del cliente. |

Vas a notar que buena parte de las unidades 7, 8 y 9 ya apareció en esta clase (Partes 1 y 2): eso es exactamente el cruce anunciado. Otros nombres que quedaron sembrados para más adelante: el paradigma **SMAC** (las siglas de *Social, Mobile, Analytics, Cloud* — la combinación de redes sociales, movilidad, analítica y nube como base de la era digital), las **tecnologías cognitivas** (el paraguas de la IA en todas sus ramas) y los **gemelos digitales** (la réplica virtual de un proceso o planta física para simular sobre ella) — todos con su desarrollo en las clases que vienen.

---

## 2. 🔴 El vocabulario que quedó plantado

Al recorrer el plan aparecieron términos que van a usarse toda la cursada. Acá está cada uno, con lo que se explicó de él.

### 2.1 ERP y "sistema de gestión": una traducción con trampa

**ERP** viene de *Enterprise Resource Planning* — planificación de los recursos empresariales. Es el sistema central con el que una organización lleva su operación: compras, ventas, facturación, stock, contabilidad, sueldos. Y un dato clave de arquitectura que quedó adelantado: **los ERP integran todo en una única base de datos** — de ahí viene buena parte de su valor (y de la solución al problema de los silos de la Parte 2, §8).

La trampa está en la traducción. En español, al ERP se le dice **"sistema de gestión"** a secas: el Tango, el Bejerman, el Odoo son "sistemas de gestión". Pero si traducís literalmente, "sistemas de gestión" es un concepto **más amplio**: todo sistema que una empresa usa para gestionar información o procesos — el ERP, sí, pero también el **CRM** (*Customer Relationship Management*, el sistema de gestión de la relación con los clientes — Salesforce es el líder mundial; por algo su logo empapela la Fórmula 1 y el tenis), el *Supply Chain Management*, el *Human Capital Management*. En esta materia, cuando se dice "sistema de gestión" sin más, se está hablando del ERP específicamente. Queda aclarado para que no genere confusión — es la misma cosa.

Sobre las siglas en inglés en general, rige lo dicho en la Parte 1 (§1): se usan porque no tienen traducción de uso real y así aparecen en cualquier entrevista o proyecto. Ejemplo perfecto: **SaaS** (*Software-as-a-Service*): contratar un sistema pagando una suscripción periódica, en vez de comprar una licencia perpetua y montarlo en servidores propios. Nadie dice "software como servicio" en una reunión — se dice SaaS.

### 2.2 On-premise → cloud: el cambio de fondo que ya pasó

**On-premise** significa "en las instalaciones propias": todo el software instalado en servidores que la empresa posee — fierros propios. Hasta hace no tanto (pensá en la época del famoso "efecto año 2000") esa era la norma absoluta. Hoy la foto se invirtió: prácticamente todo es **cloud** — los sistemas viven en la nube. En el medio pasaron también los cambios de arquitectura: del paradigma **cliente-servidor** (un programa instalado en cada máquina hablando con un servidor central) a las **arquitecturas de microservicios** (el sistema partido en muchos servicios chicos e independientes que se comunican entre sí). La materia no hace el recorrido histórico — lo que importa es el impacto actual de ese nuevo escenario sobre las organizaciones.

### 2.3 Niveles de planificación y decisión: la misma información, distinta altura

En toda organización hay tres niveles de decisión — **estratégico, táctico y operativo** — y el punto central es este: **los sistemas guardan toda la información al máximo detalle granular, pero la presentan distinto según el nivel de quien decide**.

El ejemplo para fijarlo: un director regional de una cadena de supermercados (un Walmart, un Jumbo) mira la marcha del negocio **agregada** — ventas, costos, tendencias por región. Jamás va a mirar cuántos paquetes de spaghetti Mamaluchetti al huevo se vendieron en la sucursal Aldo Bonzi: ese detalle, a nivel estratégico, no le sirve para nada. Ahora, el **gerente de esa sucursal**, que maneja la reposición y el stock, necesita exactamente ese detalle.

El paralelismo técnico, con algo que ya manejás de bases de datos: es la diferencia entre un `SELECT` que trae todos los registros bien granulares y un `SELECT` con `GROUP BY` que muestra la información agrupada y agregada. Misma tabla, misma información — distinta altura de mirada. Los dashboards estratégicos, los KPIs y todo el tablero de decisión de la unidad 1 se construyen sobre esta idea.

### 2.4 De registrar a decidir (y de decidir a accionar): la organización data-driven

La evolución de los sistemas empresariales que la materia va a recorrer se resume en una línea:

> Sistemas que **registraban** datos (transacciones, datos maestros) → sistemas que dan **información para tomar decisiones** → sistemas cada vez más **autónomos**, guiados por IA.

Del primer estadio al segundo aparecen los **KPI** (*Key Performance Indicators* — indicadores clave de rendimiento: los pocos números que resumen la salud del negocio), los **dashboards** (tableros visuales que concentran esos indicadores) y el concepto de organización **data-driven**: la que se guía por datos para decidir, en vez de por intuición u olfato. Del segundo al tercero aparece lo agéntico — que merece su propia entrada.

### 2.5 Proceso agéntico: la definición que hay que llevarse hoy

> **Un proceso agéntico es un proceso con inteligencia artificial autónoma, capaz de tomar decisiones en función de los objetivos que se le plantearon y de encontrar el mejor camino para resolver la meta que se le dio.**

La diferencia con lo que ya conocés: **no es un ChatGPT** al que le preguntás cosas y te responde. Es un **agente** al que le das instrucciones y objetivos, y se va a trabajar solo. El ejemplo canónico: *"tenés que evitar quiebres de stock: andá evaluando hora a hora los niveles según los sistemas, y cuando detectes una alerta de potencial quiebre, generá la orden de reposición automática y mandala"*. Le diste las instrucciones — y a partir de ahí tenés un proceso **sin intervención humana**, capaz de resolver los problemas y trabas que vaya encontrando en el camino.

Esto conecta con la idea de **sistemas de acción** (*systems of action*): la información de la empresa deja de ser solo un registro guardado en una base de datos y pasa a ser **información accionable** — dispara decisiones y acciones por sí misma, con el humano supervisando. Es la tecnología de la que hoy más se habla en las empresas, las primeras ya están experimentando con ella, y tiene su clase entera dedicada (clase 03, presencial) — además de ser el corazón conceptual de una de las propuestas obligatorias del TP.

> 🎓 **Para el parcial, si te preguntan:** *¿Qué es un proceso agéntico?*
> Es un proceso con IA autónoma que toma decisiones en función de objetivos planteados y encuentra el camino para cumplir la meta, sin intervención humana — por ejemplo, un agente que monitorea el stock hora a hora y ante riesgo de quiebre genera y envía la orden de reposición solo. Se diferencia de un chatbot en que no responde preguntas: ejecuta un objetivo, resolviendo las trabas que encuentra.

### 2.6 Los reportes de analistas: los "reviewers" del software empresarial

¿Cómo decide una empresa qué sistema implementar? Una de las herramientas principales son los **reportes de analistas**: informes de empresas internacionales —**Gartner, Forrester, IDC** son las tres grandes— que se dedican a analizar y comparar todos los sistemas empresariales del mercado, armando matrices y cuadrantes: qué soluciones hay para cada categoría, pros y contras de cada una, en qué sector funciona mejor ("este CRM lo usan 50 bancos en Latinoamérica y tiene red de partners en todas las ciudades — pero el mantenimiento es costoso").

La analogía exacta: el youtuber que hace el *unboxing* y compara teléfonos — "la cámara de este es mejor, pero la batería de aquel dura más" — y en quien confiás porque se supone que **no está aceitado por ninguna marca**: es neutral, como se le supone a un periodista. Eso mismo, pero para el software empresarial. Algunos informes son de pago; otros se liberan públicamente, y durante la cursada se van a ver ejemplos concretos.

**El principio agnóstico que gobierna todo esto: no hay ERPs mejores o peores en abstracto — hay necesidades.** ¿Qué es mejor, una Ferrari o un Toyota Etios? Nadie discute cuál es más potente. Ahora: si tu necesidad es llevar a los nenes al jardín e ir al Coto una vez por mes, con la Ferrari la vas a romper toda en las calles y vas a pagar un mantenimiento absurdo para una necesidad que no tenés. Una empresa no implementa un sistema costosísimo y complejo si no lo necesita. La decisión sale de una **matriz de evaluación desde el negocio**: qué procesos hay que cubrir, si tiene que ser multimoneda o multiidioma, si consolida planificación contable, si maneja una o múltiples sociedades fiscales, qué cuesta la mano de obra local ("me venden un ERP noruego buenísimo… y cuando necesite soporte tengo que pagarle el avión a un consultor desde Noruega"). De ese análisis sale en qué segmento se mueve la empresa y qué sistema le cierra en costo-beneficio. Cómo se arma formalmente ese análisis —el **business case**, el caso de negocio que justifica una inversión— se ve al detalle en la unidad 2.

### 2.7 El mapa del mercado: los tiers

Los jugadores del mercado ERP se organizan en niveles (*tiers*):

| Tier | Quiénes | Perfil |
|---|---|---|
| **Tier 1 — los tres grandes** | **SAP** (alemana, el líder mundial histórico de los sistemas de gestión), **Oracle** (creció comprando otros; hoy una suite completa), **Microsoft Dynamics** (menos presente en las corporaciones gigantes, fuerte en el segmento medio) | Grandes corporaciones, operaciones globales. |
| **Tier 2 — intermedios** | Infor, Epicor, TOTVS, IFS, Sage X3 | Empresas medianas-grandes. |
| **Tier 3 — locales / segmento chico** | Tango, Buenos Aires Software (BAS), Bejerman, Calipso, Softland, NetSuite, Odoo, Red Plataforma | PyMEs y empresas locales — los que más se ven en Argentina. |

Aclaración de alcance idéntica a la de los analistas: **no hay que memorizarlos ni aprenderlos** — la materia es agnóstica, no defiende a ninguno. El objetivo es conocer el mapa: reconocer nombres y logos que ya viste, entender dónde juega cada uno y qué tipo de empresa usa cada cual. (Más de uno de estos nombres aparece en el trabajo de compañeros de la cursada — administrando Salesforce, o en la adopción de CRM en una petrolera — y ese tipo de casos reales alimenta las clases.)

---

## 3. 🟡 El aperitivo de la IA: 75 años de historia (que casi nadie conoce)

La inteligencia artificial va a terminar cruzando todas las clases y todo lo que se hable — es hoy el principal tema de conversación en todas las empresas. Antes de meterse de lleno (tiene sus clases propias), quedó plantado un dato que sorprende hasta a estudiantes de sistemas:

**¿Cuántos años tiene la inteligencia artificial? Unos 75.** El consenso ubica su origen alrededor de **1950**, en el paper fundacional de **Alan Turing** — sí, el mismo de la cinta de Turing que viste en Lógica y Estructuras Discretas. Contexto: post Segunda Guerra Mundial. Turing fue quien ayudó a quebrar el **código Enigma** — el cifrado con el que los nazis mandaban sus mensajes — y se considera que eso acortó la guerra en cinco años o más a favor de los aliados (la biopic *El código enigma*, con Benedict Cumberbatch, cuenta esa historia y vale la pena conocerla). De ese paper sale el **test de Turing**: la prueba de si una máquina puede hacerse pasar por humana — y de esa idea derivan, entre otras cosas, los **CAPTCHA** que seguís resolviendo hoy en la web ("demostrá que sos humano").

De ahí en adelante, el timeline que se va a recorrer en las clases de IA: la cinta de Turing → los primeros chatbots → el *machine learning* → el *deep learning* y las redes neuronales → la IA generativa y agéntica actual. Dos hitos para dimensionar la profundidad histórica:

- Las **redes neuronales** se exploran desde hace décadas (los años 80 y antes). El paper de los **Transformers** —la arquitectura sobre la que se construyen los LLM actuales (*Large Language Models*, los modelos grandes de lenguaje detrás de ChatGPT o Claude)— es, en esa línea de tiempo, historia reciente, "acá nomás".
- En **2024, los dos premios Nobel de Física y de Química se otorgaron por trabajos relacionados con redes neuronales**: el de Química a los creadores de DeepMind (hoy Google DeepMind), por los modelos que predicen la estructura tridimensional de las proteínas —cómo se pliegan a partir de la cadena de aminoácidos— usados para descubrir fármacos y curas; y el de Física alrededor de las redes neuronales y el **backpropagation** (el algoritmo con el que se entrenan) — polémico para algunos, porque "eso no es física".

Y la paradoja que cierra el aperitivo: el *machine learning* tiene unos 25 años, y las empresas **recién ahora** estaban encontrándole la vuelta para aplicarlo masivamente… cuando apareció algo totalmente distinto (la generativa) y quedaron sin saber para dónde correr. Ese desfasaje entre lo que la tecnología ya puede y lo que las organizaciones logran absorber es, en el fondo, otro capítulo de la tormenta perfecta (Parte 2, §9).

---

## 4. 🟢 Esta materia como punto de encuentro de la carrera

Una promesa que conviene registrar, porque le da sentido retroactivo a media carrera: **casi todas las materias que venís cursando aparecen acá**. El "¿para qué mierda sirve esto?" de varias encuentra su respuesta en esta cursada:

- **Lógica y Estructuras Discretas** (la ex Matemática Discreta): los retículos algebraicos, el álgebra de Boole, la cinta de Turing — la base sobre la que funciona un LLM y un proceso agéntico. No habría IA sin eso.
- **Probabilidad y Estadística**: las redes bayesianas, los árboles de decisión, las máquinas de soporte vectorial, el error tipo 1 y tipo 2, sensibilidad, especificidad, la matriz de confusión — exactamente lo que hace funcionar los modelos predictivos y el machine learning. Conviene tenerlo fresco para las clases de IA.
- **Economía y Administración**: el análisis de negocio y la justificación de inversiones — cómo una empresa decide invertir en implementar un ERP (el business case de la unidad 2).
- **Electivas como Gestión del Cambio Organizacional** (el impacto cultural de estos proyectos en las empresas) y **Creatividad e Innovación** (prototipado de productos) — se cruzan con las unidades de innovación.

La aclaración honesta que acompaña la promesa: las empresas hoy **no desarrollan su propio LLM** — usan los existentes como software de base. No hace falta dominar el detalle matemático para trabajar con IA; pero entender que todo aquello era la base de esto le da un porqué a lo que estudiaste.

Y el deslinde final: **esta no es una materia de programación**. No se programa nada. El que se sienta canchero y quiera probar cosas de *vibe coding* (programar delegándole el código a la IA mediante instrucciones en lenguaje natural) con Python y temas de IA, bárbaro — pero no es requisito, ni por tiempo ni por profundidad se va a entrar ahí.

---

## 5. 🔴 Las reglas de la cursada (todo lo operativo, en un solo lugar)

### 5.1 Modalidad, días y horarios

- **Lunes, 19:00 puntual.** Cursada **híbrida**: la mayoría de las clases virtuales (Zoom, link fijo en el aula virtual) y **5 presenciales** en Medrano — el mínimo de presencialidad que pide la facultad — de las cuales 2 son las defensas del TP. Las presenciales elegidas son las de dinámica taller/debate (los temas de IA); las más conceptuales van por Zoom.
- **Las virtuales son sincrónicas**: clases en vivo por un medio digital, no videos grabados para mirar cuando quieras. Cierran ~21:30 (tope declarado 22:00), con un break de ~8-10 minutos en el medio.
- **Las presenciales** arrancan 19:00 sin break y cortan 21:00-21:15 (consideración con los que viajan lejos). El aula de Medrano se publica en el aula virtual unos días antes de cada una.

### 5.2 Calendario completo (13 clases + 4 feriados)

Este cuatrimestre tiene 4 lunes feriados (17/8, 21/9, 12/10 y 23/11) pero una semana más de duración, así que la cantidad de clases queda igual. El calendario vive en una planilla online enlazada en el aula y en un **calendario de Zoom suscribible** que agenda automáticamente todas las clases con su temario en la cuenta de Google de la facultad — y se actualiza si hay cambios.

| # | Fecha | Modo | Tema | Hito TP |
|---|---|---|---|---|
| 01 | 10/8 | Virtual | Introducción: Transformación Digital en las organizaciones | |
| 02 | 24/8 | Virtual | Los sistemas de gestión — ERP | |
| 03 | 31/8 | **Presencial** | El impacto de la IA: empresa "aumentada" y "sistema de acción" | |
| 04 | 7/9 | Virtual | Subsistema de Ventas | **Entrega propuesta TP** |
| 05 | 14/9 | Virtual | Subsistema de Compras | |
| 06 | 28/9 | Virtual | Subsistema Industrial 4.0 | |
| 07 | 5/10 | Virtual | Subsistema Financiero-Contable / RRHH | |
| — | 12/10 | *(feriado)* | — | **Entrega 1ra parte** |
| 08 | 19/10 | **Presencial** | TD 1/4 — IA, las personas y las organizaciones | |
| 09 | 26/10 | **Presencial** | TD 2/4 — Gestión de la Innovación | |
| 10 | 2/11 | Virtual | TD 3/4 — De Machine Learning a la IA generativa y agéntica | |
| 11 | 9/11 | Virtual | TD 4/4 — Lab IA + lowcode, casos de uso reales | **Entrega 2da parte y final** |
| 12 | 16/11 | **Presencial** | Presentación TP — sesión 1 | Defensa oral |
| 13 | 30/11 | **Presencial** | Presentación TP — sesión 2 | Defensa oral |

Posible ajuste a tener en el radar: hay 2-3 viajes laborales al exterior del docente antes de fin de año. La intención declarada es dar la clase igual desde donde esté; si un huso horario lo hace inviable, se avisa con tiempo y se reprograma (el historial: una sola clase cancelada por esto en años). En la **próxima clase presencial**, además, hay ronda de presentaciones: quién sos, si trabajás, por qué te anotaste, qué te pasa con la IA.

### 5.3 Sin grabaciones: por qué, y qué implica

**Las clases no se graban.** Hasta hace unos años se grababan y subían a YouTube; se dejó de hacer por pedido de la facultad (fomentar la sincronicidad y la presencialidad) y quedó a decisión de cada profesor. Acá la decisión es no grabar, con dos argumentos: la gente se suelta más a opinar y discutir cuando no queda registro, y —el argumento de época— armar una clase de dos o tres horas para que después la vean resumida por una IA en dos minutos desmotiva el formato entero.

Lo que sí: **todo el material de soporte se sube al aula virtual después de cada clase** — lo conceptual, los ejercicios, y un catálogo de las aplicaciones de IA que se van usando. Si faltás, encontrás el material, pero **la clase en sí no está en ningún lado**. Implicación de estudio directa: lo que se explica en vivo, o lo capturás vos, o se pierde.

La contracara de la libertad: no se toma lista, nadie te persigue si te levantás — "esto es la universidad, cada uno elige qué valor le da". La participación se mide de otra manera:

### 5.4 La Liga Transformación Digital (la trivia)

Desde la **clase 02**, cada clase abre con una **trivia de Quizizz** (la plataforma de preguntas tipo Kahoot) sobre lo visto la clase anterior. Con eso se arma un campeonato a lo largo de toda la cursada — la **Liga TD** — que es, a la vez, la medida de participación y de puntualidad (se juega en los primeros minutos de cada clase). El reglamento completo está publicado en el aula; lo esencial:

**Puntaje por fecha, según posición en la trivia:**

| Posición | 1º | 2º | 3º | 4º | 5º | 6º | 7º | 8º | 9º | 10º |
|---|---|---|---|---|---|---|---|---|---|---|
| Puntos | **25** | 18 | 15 | 12 | 10 | 8 | 6 | 4 | 2 | 1 |

Gana la Liga quien acumula más puntos en toda la cursada; empates se definen por fechas ganadas y luego por podios.

**Premios:**

| Premio | Beneficio |
|---|---|
| 🥇 Individual 1º | **+2 puntos** en la nota del TP y de cursada — **o acceso a promoción** |
| 🥈🥉 Individual 2º y 3º | +1 punto en nota de TP y de cursada |
| Grupo con más podios | +1 punto en el TP grupal |
| Top 2 grupos | Prioridad para elegir fecha de presentación |

Leelo estratégicamente: el primer puesto individual de la Liga puede valer por sí solo el acceso a la promoción, y es la única vía de nota que no depende del grupo. Diez minutos al inicio de cada lunes, con la clase anterior repasada, es la apuesta de mejor retorno de toda la cursada.

### 5.5 El TP integrador: la evaluación de la materia

**No hay parcial.** La materia se aprueba o promociona con un único **trabajo práctico integrador grupal** — más los puntos de la Liga. La consigna, presentada a grandes rasgos (el enunciado completo está subido al aula; se formaliza y se aclaran dudas en la próxima clase):

- **Grupos de 4** (excepcionalmente uno de 5 si la división deja a alguien suelto). Los arman ustedes —el grupo de WhatsApp es el canal natural— y se avisan para cargarlos en el aula virtual.
- **Parte 1 — el caso real:** elegir una empresa u organización a la que algún integrante tenga acceso (trabaja, trabajó, conoce, tiene un familiar) y estudiar a alto nivel un proceso o área — o la empresa entera si es chica: cuáles son sus sistemas de gestión principales, qué procesos soportan, diagnóstico de la situación actual, dónde el sistema le está quedando chico.
- **Parte 2 — la propuesta:** ponerse en el rol de una **consultora ficticia en innovación tecnológica y de negocio** que, en función de ese diagnóstico, le propone a la empresa una hoja de ruta de innovación y adopción de IA: **dos o tres iniciativas concretas** para transformarse digitalmente — evolucionar hacia una empresa *aumentada* (potenciada, no reemplazada) por la IA. La metáfora exacta de la consigna: *agarrar un Blockbuster y ver cómo lo convertirías en un Netflix* — con la salvedad de que la parte 1 es real y la parte 2 es el ejercicio propositivo (si la empresa después compra o no las ideas, no importa).
- **Entregables:** un informe tipo **monografía** (que se construye con lo que se va viendo clase a clase) + una **presentación ejecutiva** defendida en público en las últimas dos clases — como si fueran la consultora presentándole la propuesta a los decisores de la empresa para terminar de convencerlos. El TP es la propuesta comercial; la defensa es la reunión ejecutiva.
- **Ritmo:** todavía no hay que hacer nada — pero conviene ir pensando casos candidatos ya. Se pueden proponer dos o tres opciones y hay ayuda del docente para elegir la que mejor aplique. En una o dos semanas los grupos ya deberían estar arrancando. Las fechas duras están en el calendario de arriba: propuesta el 7/9, primera parte el 12/10, entrega final el 9/11, defensas el 16/11 y el 30/11 (los grupos se reparten entre ambas sesiones — y los top 2 de la Liga eligen fecha).

El mensaje de cierre sobre la nota, textual en espíritu: con un buen trabajo y una buena presentación hay buenas probabilidades de promocionar — y la trivia suma encima. Está todo dado; está en manos de cada uno.

### 5.6 Canales y quién dicta

**Dudas:** foro del aula virtual, o mail al docente — responde cuando puede, en cualquier horario. En el aula también se puede ver el material de cursadas anteriores, como referencia de todo lo que se va subiendo clase a clase.

**El docente**, en dos líneas que explican el enfoque de toda la materia: Ing. en Sistemas de la UTN FRBA (plan '95, egresado hace ~15 años), con ~28 años en una misma consultora tecnológica — arrancó programando en **ABAP** (el lenguaje de programación propio de SAP) y pasó por todos los roles: desarrollador, analista, líder de proyecto, líder técnico, preventa, arquitecto de solución, y hoy un rol comercial regional para Sudamérica en verticales de negocio (trabaja sobre todo con salud y seguros: prepagas, clínicas, optimización de agendas de quirófano, sistemas para médicos y financiadores). De ahí salen los casos reales que atraviesan la cursada — YPF, bancos, Mercado Libre, fintechs, healthtechs, multinacionales y PyMEs — dentro de lo que la confidencialidad permite. La materia está armada desde esa experiencia: lo que hoy está pasando de verdad en las empresas, no teoría de libro.

---

## ✅ Checkpoint — Clase 01 completa

Diez preguntas para verificar que la clase quedó entendida. Sin respuestas acá: respondelas por escrito o en voz alta, y después contrastá (las respuestas modelo van al complemento de la unidad).

1. Una cadena de retail invierte en que sus entregas de e-commerce bajen de 48 a 2 horas. ¿Eso es transformación digital? ¿Es una disrupción? Justificá usando los conceptos exactos de la clase.
2. "Blockbuster quebró porque no se adaptó al streaming." ¿Qué tiene de incompleta esta afirmación, y qué matices le agregarías?
3. ¿Por qué "yo sé lo que quiere mi cliente" es el pecado capital de los proyectos empresariales, y qué técnicas concretas existen para reemplazar esa suposición por conocimiento?
4. Explicá **explotar** y **explorar**, y por qué una empresa que hace solo uno de los dos está en problemas (un riesgo distinto para cada caso).
5. ¿Por qué Uber apareció cuando apareció y no veinte años antes? ¿Qué regla general sobre la tecnología ilustra eso?
6. Uber no tiene coches, Airbnb no tiene casas, YouTube no tiene contenido, Booking no tiene hoteles. ¿Qué dice ese patrón sobre dónde está el valor en la era digital?
7. Nombrá dos razones estructurales distintas por las que a una empresa grande le cuesta más innovar que a una startup (pista: una es de costos/velocidad, la otra vive puertas adentro de sus sistemas).
8. ¿Qué es un proceso agéntico y en qué se diferencia de usar un chatbot? Dá un ejemplo concreto.
9. ¿Para qué sirven los reportes de analistas (Gartner, Forrester, IDC) y por qué el principio rector al elegir un ERP es que "no hay mejores ni peores"?
10. ¿Qué significa que una organización sea *data-driven*, y cómo se relaciona con los niveles de decisión estratégico/táctico/operativo?

---

**FIN DE LA PARTE 3 — Apunte Maestro Clase 01 · Fin del apunte maestro de la clase 01**
