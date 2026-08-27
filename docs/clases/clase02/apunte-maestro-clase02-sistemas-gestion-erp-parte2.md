# 📘 Apunte Maestro — Clase 02: Los sistemas de gestión (ERP)

## Parte 2 de 3 — El mercado hoy: expectativas, analítica y sistemas que actúan

**Transformación Digital · UTN FRBA · 2C 2026 · Clase 02 (24/8, virtual)**

> **Qué cubre esta parte:** el contexto que hace falta para entender en qué se están convirtiendo los sistemas de gestión: cómo maduran las tecnologías (el ciclo de sobreexpectación de Gartner), qué se le pide hoy al análisis de datos (descriptivo → predictivo → prescriptivo), y el cambio de era de los sistemas empresariales: de registrar a actuar (systems of record → engagement → action), con el caso completo de la empresa agéntica y su marco de gobernanza.
> **Antes:** Parte 1 — los cinco conceptos fundacionales. **Después:** Parte 3 — los ERP propiamente dichos.

---

## 6. 🔴 El ciclo de sobreexpectación (Gartner)

### El caso: la fiebre del metaverso

Hace unos años, de golpe, había que estar en el metaverso. Los directorios preguntaban *"¿por qué no estamos haciendo algo con metaverso?"*, y las empresas — por miedo a quedarse afuera — respondían haciendo *algo*: una tienda virtual en el metaverso, un recital de Coldplay contratado en el metaverso… plata gastada, literalmente, en aparecer. ¿Con qué estrategia? Ninguna: *"hay que estar, porque todos están"*.

Volvé un segundo a la sección 5 (Parte 1) y ya sabés cómo termina: nadie se había preguntado **qué problema u oportunidad** se quería abordar en ese canal. ¿Voy a vender en el metaverso los mismos productos que en la tienda de Medrano y Rivadavia? ¿El que compra ahí va a ir a comprar al metaverso? ¿O apunto a un segmento joven que juega videojuegos — y entonces, con qué producto, con qué pricing? Sin esa discusión, estar o no estar no tenía sentido. La expectativa se desinfló, y hoy el metaverso es sinónimo de promesa incumplida.

Ese recorrido — euforia, desinfle, y lo que viene después — no es una anécdota: es un **patrón que siguen todas las tecnologías emergentes**, y tiene nombre y gráfico propios.

### La curva

**Gartner** (consultora de análisis del mercado tecnológico, referente mundial del sector) sostiene que toda tecnología que sale al mercado atraviesa, de una manera u otra, el mismo ciclo — el **ciclo de sobreexpectación** (*hype cycle*): las expectativas suben mucho más rápido que la madurez real, chocan contra la realidad, y recién después del derrumbe la tecnología encuentra su valor verdadero.

```
 Expectativas
    ▲
    │              PICO DE EXPECTATIVAS
    │              SOBREDIMENSIONADAS
    │                    ●●●
    │                  ●     ●  ← empieza la prensa negativa
    │  proliferación ●        ●
    │  de proveedores●         ●  ← consolidación y fracaso            MESETA DE
    │  sobrepromoción●          ●     de proveedores                  PRODUCTIVIDAD
    │  en los medios●            ●                              ____●●●●____
    │               ●             ●                       __●●●●
    │  1ª generación●              ●●             ___●●●●   ← mejores prácticas,
    │  de productos●                 ●●●____●●●●●            metodologías, 3ª gen.
    │  1ª ronda de ●                    ↑                    de productos
    │  capital    ●                 ABISMO DE
    │  I+D     ●●                  DESILUSIÓN
    └────────────────────────────────────────────────────────────────► Tiempo
      LANZAMIENTO      PICO           ABISMO        PENDIENTE DE      MESETA
      TECNOLÓGICO                                   ILUMINACIÓN
```

### Las cinco fases, con sus síntomas

**1. Lanzamiento tecnológico.** Nace la tecnología: I+D, **primera ronda de capital** de inversores que ven "la nueva apuesta", primera generación de productos — caros y muy a medida —, **MVPs** (*mínimo producto viable*: la versión más chica de un producto que sirve para probar la idea), pruebas piloto y pruebas de concepto. Los **early adopters** (los primeros dispuestos a adoptar algo nuevo, por el gusto de ser los primeros) investigan. Empieza la sobrepromoción en los medios: primero la prensa especializada y los informes técnicos… y en el pico ya está cualquiera hablando del tema en la televisión a cualquier hora.

**2. Pico de expectativas sobredimensionadas.** Efecto contagio generalizado — el **FOMO** (*fear of missing out*: el miedo a quedarse afuera) empuja a empresas e inversores a moverse "porque todos se mueven". Proliferan los proveedores: junto a los serios aparecen los chantas prometiendo cosas inviables con tal de subirse a la ola. La actividad ya excede a los early adopters.

**3. Abismo de desilusión.** La realidad no alcanza a la promesa. Empieza la **prensa negativa**, y dentro de las empresas se escucha LA frase — la que vas a escuchar siempre que algo no avanza: ***"no encontramos el caso de negocio"***. Que es, exactamente, la sección 5 de la Parte 1 vista desde el final: se compró tecnología sin problema ni oportunidad definidos, y la cuenta llegó. Consolidación y **fracaso de proveedores**, proyectos sin caso de uso real que se caen, y sin embargo — mirá la curva — sigue habiendo **segunda y tercera ronda de capital** para los emprendimientos que sobreviven. La adopción real en este punto: menos del 5% del mercado.

**4. Pendiente de iluminación.** Ya sin reflectores ni presión de moda, separado el humo, aparecen la **segunda y tercera generación de productos** — paquetes prearmados, familias de productos —, casos que funcionan a pequeña escala, y se desarrollan las **mejores prácticas y metodologías**. El interés se recupera despacio, con otra pendiente: mucho menos pronunciada, mucho más real.

**5. Meseta de productividad.** Expectativa estable: la tecnología rinde lo que promete, los casos generan valor de verdad, y comienza la fase de alta adopción — del orden del 20 al 30% del mercado potencial.

### Lo que la curva NO dice

El valle **no es la muerte** de la tecnología. La curva no baja y desaparece: hace panza y remonta. El metaverso sigue existiendo; blockchain también, con inversiones enormes. Lo que el abismo filtra es el humo: los proveedores oportunistas y los proyectos sin caso de negocio. La tecnología que tiene valor real lo encuentra después, sin apuro.

Ejemplos para ubicar en la curva:

- **NFT** (*tokens no fungibles*: certificados digitales de propiedad sobre un activo único, asociados al mundo cripto): el caso testigo de expectativa que no se recuperó — más allá de usos serios que se discutieron (patentes, tokenización de activos), quedó atrapado en el derrumbe.
- **Realidad virtual**: el hardware que necesitaba (cascos) era demasiado costoso en su momento; no cumplió las expectativas de su pico.
- **Blockchain empresarial** — no cripto/trading, sino usos corporativos: trazabilidad logística, tokenización de activos, industria aseguradora y financiera. Hoy tiene muchos casos de uso reales: es un buen candidato a "ya superó su pico y está madurando".

Y la pregunta que quedó **abierta para la próxima clase**, pensala desde ya: la **IA generativa** (la que crea contenido: texto, imágenes, código) y la **IA agéntica** (agentes que ejecutan acciones de punta a punta con autonomía — se desarrolla en la sección 8), **¿en qué punto de la curva están hoy?** ¿Estamos en el pico de la ola, o ya hay valor real funcionando en las empresas y no es solo promesa?

### ¿Y los ERP dónde están?

En ningún lado de la curva — y eso es un dato, no una omisión. Los ERP tienen **entre 40 y 50 años**: pasaron por todo esto hace décadas y viven en la meseta desde entonces. Pero acá está la clave de toda la clase: **cada tecnología que hoy se les incrusta** — la IA agéntica a la cabeza — **sí está atravesando su propia curva de sobreexpectación**. El ERP tradicional que no se reconvierte y no adopta esta ola queda viejo; el que la adopta, cambia de naturaleza. Ese cruce es exactamente lo que desarrollan las secciones que siguen.

> **📌 Para el parcial, si te preguntan** — *Una tecnología acumula prensa negativa, sus pilotos "no encuentran el caso de negocio" y varios proveedores quiebran. ¿En qué fase del ciclo de sobreexpectación está?*
> En el abismo de desilusión: las expectativas sobredimensionadas del pico chocan con la realidad, cae todo lo que no tenía caso de uso real y se consolida o quiebra la oferta. No implica que la tecnología muera — la que tiene valor remonta después por la pendiente de iluminación hasta la meseta de productividad.

---

## 7. 🔴 Descriptivo → predictivo → prescriptivo

### El caso: el tablero más lindo del mundo

Imaginate el tablero de control perfecto: presupuesto anual contra ejecutado, desvío calculado; plan de ventas de 1.000 unidades, vendimos 900, un 10% abajo — semáforo en rojo. Gráficos de torta, de barras, reportes preciosos armados con Power BI o QlikView (dos de las herramientas visuales de reportes más usadas del mercado), todo lo que se conoce como **Business Intelligence** o **BI**: tableros, dashboards, **KPIs** (*indicadores clave*: mediciones resumidas de un objetivo contra su meta — se desarrollan en la Parte 3).

Ahora la pregunta incómoda: por más lindo que sea, **¿qué estoy mirando?** Cosas que **ya pasaron**. Estoy manejando mirando el espejo retrovisor.

### Los tres niveles de análisis

El nivel de análisis se elige según la **etapa de madurez** y los **objetivos de negocio** — y forman una escalera:

| | **Análisis descriptivo** | **Análisis predictivo** | **Análisis prescriptivo** |
|---|---|---|---|
| Para qué | Conocer lo que ha pasado | Estimar los resultados futuros | Mejorar los resultados posibles |
| Qué hace | Analiza e interpreta lo que ya sucedió | A partir de lo sucedido, intenta predecir lo que sucederá | Identifica estrategias y acciones que mejoren los resultados previstos |
| Las preguntas que responde | ¿Qué pasó? ¿Cómo pasó? | ¿Por qué pasó? ¿Qué podría pasar? | ¿Qué hacer? ¿Cómo hacerlo? |
| Ejemplo | El tablero de ventas del año pasado | El **forecast** de ventas (*pronóstico*: proyección de cuánto se va a vender) | "Decime qué acciones tomar para llegar a la meta" |

La progresión, dicha en una frase: del descriptivo espero que me muestre lo que pasó; del predictivo, que **reduzca la incertidumbre** sobre lo que puede pasar; del prescriptivo ya no espero que me anticipe el futuro — espero que **me ayude a que pase lo que yo quiero que pase**: que me diga cómo cumplir mis metas y objetivos.

### Por qué esto redefine a los sistemas de gestión

Hace unos años, un sistema que transaccionaba, registraba datos y mostraba reportes lindos de lo ocurrido **alcanzaba** — con eso se justificaba implementar SAP u Oracle. Hoy no: con la IA en el medio, la competencia le está haciendo preguntas a sus modelos sobre **lo que puede pasar y cómo actuar** — cómo armar la estrategia con los clientes, cómo afinar la planificación, cómo construir un forecast preciso. Ver lo que pasó está bárbaro, pero si no sirve para anticipar, **falta la mitad de la historia**.

Ese es el desafío en el que están parados hoy los fabricantes de software empresarial, porque es lo que el mercado les demanda: *"¿tu plataforma está capacitada para explotar estas capacidades y ayudarme — o solo me muestra el pasado?"*. Con esa vara, los sistemas de gestión tradicionales **ya no alcanzan**. Qué son y cómo se están reconvirtiendo es el tema de la sección que sigue.

> **📌 Para el parcial, si te preguntan** — *¿Qué diferencia al análisis descriptivo, el predictivo y el prescriptivo?*
> El descriptivo analiza e interpreta lo que ya pasó (tableros, KPIs, BI); el predictivo usa lo sucedido para estimar lo que podría pasar y reducir incertidumbre; el prescriptivo identifica qué acciones tomar para lograr el objetivo buscado. La escalera va de mirar el pasado a anticipar el futuro y, finalmente, a intervenir sobre él.

---

## 8. 🔴 De sistemas de registro a sistemas de acción

### Qué era un ERP, durante décadas

Un ERP tradicional era, en esencia, **un sistema para registrar**: una base de datos relacional enorme — cientos, miles, decenas de miles de tablas — donde quedaba asentado **cada** movimiento de la empresa: cada movimiento de stock, cada compra de mercadería, cada factura, cada orden de compra, cada liquidación de sueldos, cada asiento contable, cada ajuste de inventario, cada amortización de un bien.

Su diseño respondía a eso: sistemas **robustos, seguros y confiables**, capaces de procesar millones de operaciones sin romperse y sin que los hackeen — con interfaces que no buscaban sorprender desde el diseño, porque no estaban pensadas para ser lindas sino para registrar bien. Eso vendía SAP, y por eso lo compraban las empresas más grandes del mundo: la operación completa, asentada de forma íntegra. Un **sistema de registro** (*system of record*).

### El límite — y el cambio de era

Registrar es **una parte de la historia**. Si el sistema *solo* registra, la empresa compró un bodoque carísimo que no la ayuda en nada con la otra mitad — la que venimos arrastrando desde la organización ambidiestra (sección 2, Parte 1): explorar el futuro, desplegar productos creados con IA, abrir canales nuevos, innovar. Y acabamos de ver (sección 7) que el mercado tampoco se conforma ya con mirar reportes del pasado.

De ahí el concepto que da nombre a la nueva era — y que además es **parte de la consigna del TP integrador**: el **sistema de acción** (*system of action*). Un sistema que no solo registra lo que pasa, sino que es capaz de **actuar con esa información, en forma cada vez más autónoma**. Los que actúan son los famosos **agentes** — programas de IA que ejecutan tareas de punta a punta —, y a esa capacidad se la llama **IA agéntica**.

La idea de fondo del cambio: el software empresarial tradicional ayudaba a las empresas a *operar* — gestión, facturación, tareas administrativas. Con la IA generativa, el software pasa a **hacer el trabajo en sí**. El sector legal lo ilustra perfecto: las herramientas pasan de *asistir* a la práctica legal a *ejercerla*.

### La taxonomía completa: tres tipos de sistemas

| Tipo de sistema | Función principal | Ejemplos y características clave |
|---|---|---|
| **Systems of Record** (registro) | Almacenar y organizar datos históricos con precisión | ERP, CRM, hojas de cálculo, permisos, auditoría |
| **Systems of Engagement** (interacción) | Facilitar la interacción y la experiencia del usuario | Interfaces intuitivas, apps móviles, portales, herramientas de colaboración |
| **Systems of Action** (acción) | Representar y manejar el estado actual en tiempo real, generar *insights* a partir de los datos y tomar decisiones autónomas | Orquestación dinámica para monitorear y coordinar flujos activos; IA, analíticas, recomendaciones predictivas |

Dos precisiones para leer bien la tabla:

- **Los tres conviven.** Los sistemas de acción **no reemplazan** a los de registro: se montan encima — a la base registral confiable le **suman la capa de acción** con IA. Sin el registro íntegro abajo, no hay sobre qué actuar.
- **CRM** (*Customer Relationship Management*: el sistema de gestión de la relación con los clientes) aparece acá como ejemplo de sistema de registro junto al ERP. La diferencia precisa entre ERP y CRM — quién gestiona qué — se desarrolla en la próxima clase; por ahora alcanza con saber que son sistemas empresariales distintos y complementarios.

### La evidencia: el mercado ya cambió el discurso

Esto no es una promesa de laboratorio — alcanza con mirar cómo se presentan hoy los líderes del software empresarial. Después de **décadas** presentándose como "el ERP líder", **SAP** (la empresa alemana que desarrolla el ERP más usado por las grandes empresas del mundo) recibe hoy en su página con ***"Autonomous Enterprise"*** — la empresa autónoma: un negocio que puede *pensar, adaptarse y actuar*. **Salesforce**, el CRM líder mundial, directamente te da la bienvenida a ***"la Empresa Agéntica"***, con su agente (Agentforce) respondiendo consultas en la propia portada. Y en la prensa especializada la idea circula sin anestesia: el sistema de registro "está muerto" — fue construido para *recordar* cada interacción y cada dato, pero la memoria sola no genera negocio; la novedad es que el software por fin aprendió a *actuar*, no solo a recordar.

Leelo en clave de la sección 6: todos los fabricantes se están subiendo a la misma ola. Ya no venden "un sistema que registra transacciones para facturar y llevar la contabilidad": venden **plataformas completas para que una empresa pueda volverse autónoma, agéntica — y ambidiestra**: operar el presente y crear productos y modelos nuevos, todo conectado con el hilo de la materia. Quien viene siguiendo estos sistemas hace años lo vive como un cambio de era; quien los conoce recién ahora, ya los va a ver directamente con la mentalidad nueva.

> **📌 Para el parcial, si te preguntan** — *¿Qué diferencia a un sistema de registro de un sistema de acción?*
> El sistema de registro almacena y organiza con precisión los datos históricos de cada transacción (el ERP tradicional: robusto, seguro, confiable); el sistema de acción, además, maneja el estado actual en tiempo real y toma decisiones autónomas sobre esa información mediante agentes de IA. No lo reemplaza: le suma la capa de acción encima del registro. Entre ambos, los sistemas de engagement resuelven la interacción y experiencia del usuario.

---

## 9. 🔴 La empresa agéntica en la práctica: el caso de las 2 AM

### El incendio, versión tradicional

Empresa de turismo — un hotel, una aerolínea — con estrategia **omnicanal** (presencia coordinada en todos los canales: sitio web, redes, app, atención). Un cliente escribe un comentario negativo. Se empieza a viralizar. Peor: lo levanta un influencer con millones de seguidores.

En el mundo tradicional, la secuencia es conocida: a la mañana alguien avisa — *"che, nos están matando en Twitter"* — el responsable de satisfacción del cliente se entera, *"armemos una reunión mañana para ver por qué nos cayó el puntaje"*… y para cuando la empresa decidió algo, ya perdió clientes y está prendida fuego. El tiempo de reacción humano llega tarde por diseño.

### El mismo incendio, versión agéntica

Ahora la plataforma — el CRM, en este caso — monitorea sola, como un termostato. Procesa el lenguaje natural de los comentarios y mide su **polaridad de sentimiento** (si lo que se dice de la marca es positivo o negativo); tiene **umbrales de alerta** definidos: tantos comentarios negativos por hora, una tendencia de caída en el puntaje, o la cercanía de la conversación con una cuenta de alto impacto. A las 2 de la mañana, la polaridad se invierte y salta la alerta. Y ahí se dispara una **cadena de agentes**, cada uno con su tarea:

```
  2:00 AM                                                          8:00 AM
    │                                                                 │
 [DETECCIÓN]──▶[ANÁLISIS]──────▶[COMUNICACIÓN]──▶[CONTACTO]──────▶[INFORME]
  polaridad     un agente        otro agente      otro agente      el equipo
  invertida /   procesa todo     redacta la       identifica a     humano llega
  umbral        lo ocurrido      respuesta        los clientes     con el caso
  superado      sobre la marca   pública          en mayor riesgo  encaminado
                en la última                      y los contacta
                hora                              proactivamente
```

El mensaje a los clientes en riesgo sale automatizado — *"sabemos que quizás no estamos respondiendo como te gustaría; estamos trabajando para mejorar tu experiencia y en breve un operador se va a contactar para ofrecerte un beneficio"* — y **todo eso ocurre sin que un humano intervenga**. El comentario se viralizó a las 2 AM; a las 4 AM, mientras los directivos duermen, el sistema ya accionó e intentó apagar el incendio; a la mañana, el equipo no llega al caos sino al caso encaminado, con el análisis servido. Parece ficción — es, exactamente, la idea agéntica, y es lo que las empresas están empezando a implementar y explorar hoy. El mundo que viene es **híbrido**: humanos y agentes operando juntos.

### El marco de gobernanza: que el remedio no sea peor que la enfermedad

Todo el caso anterior tiene una condición de posibilidad: que el sistema actúe **bien**. Porque si el agente interpretó mal, contactó clientes y encima **alucinó** (inventó contenido falso con total seguridad — el riesgo típico de la IA generativa) o soltó un comentario políticamente incorrecto, tiró más leña al fuego: las consecuencias son peores que no haber hecho nada.

Quiero que mi sistema se vuelva agéntico — pero no que se descontrole y termine como Robocop tiroteando a todos. Para eso existe el marco de **gobernanza**: el conjunto de reglas que delimitan la autonomía para que sea beneficio y no riesgo. Sus piezas:

- **Rango de acción definido**: "esto podés hacer, esto no" — el ámbito exacto donde el agente se puede mover, con **umbrales** que disparan cada decisión.
- **Capa legal, de compliance** (*cumplimiento normativo*: asegurar que se respetan leyes y regulaciones) **y de seguridad**.
- **Nube privada**: que los datos de la empresa y sus clientes no salgan afuera al procesar.
- **Mitigación de alucinaciones**: hoy hay cada vez más técnicas para reducirlas, y por eso el miedo inicial fue bajando — aunque el debate sigue abierto en el mundo, y nadie tiene del todo claro cómo encajar la autonomía ni qué va a pasar con ella. La imagen de la época: no sabemos si le estamos dando una ametralladora a un mono.

### Cuando el error no es reputacional sino económico

Los riesgos de la autonomía no terminan en un comentario desafortunado — hay plata y juicios en el medio. Casos reales del comercio electrónico: en plena promoción tipo Cyber Monday, pasajes a Río de Janeiro que valían 500 dólares se publicaron **a 5 dólares** por un error. ¿"Faltaron dos ceros"? La justicia les dio la razón a los que compraron: hubo **demandas colectivas** y empresas obligadas a honrar el precio publicado. Ahora proyectalo al mundo agéntico: agentes corriendo procesos de fondo, campañas y **pricing autónomo** — y una pifiada de precio en un seguro o en un auto. El problema es gigante. (Hay compilados públicos enteros dedicados a estas metidas de pata de la IA: pilotos autónomos de empresas famosas que, donde tenían que resolver, empeoraron — y se viralizaron.)

🕳️ **Madriguera — Grafos sociales y grados de separación**
Una de las alertas del caso se dispara por la "cercanía en el grafo" con un influencer: las redes se modelan como grafos — personas como nodos, relaciones como aristas — y los grados de separación miden a cuántos saltos está cada uno de cada uno.
*Volvé al camino — esto se profundiza aparte, otro día.*

### 🟡 El dilema del pionero

Detrás de todos estos casos hay una tensión que cualquier organización enfrenta, y que cierra el círculo con el yin-yang dual de la sección 2 (Parte 1): **nadie quiere ser el conejillo de indias** — la prueba piloto que sale mal y termina en demanda — **pero nadie quiere ser el próximo Blockbuster** — el último en moverse cuando el mercado ya se movió. ¿Me mando primero, piso fuerte y capaz gano el mercado? ¿O me quedo en el molde, dejo que el error lo pague otro, y entro después? Depende del mercado, de la estrategia y de mil cuestiones más; a veces el valiente se lleva el gran beneficio y a veces esperar termina siendo mejor. Eso, al final, **es el riesgo empresario** — y si alguien supiera lo que va a pasar, no estaría acá.

> **📌 Para el parcial, si te preguntan** — *¿Qué requiere una empresa para volver agéntico su sistema sin que la autonomía se convierta en un riesgo?*
> Un marco de gobernanza: rango de acción y umbrales definidos ("esto podés hacer, esto no"), capa legal, de compliance y de seguridad, procesamiento en nube privada para que los datos no salgan, y mitigación de alucinaciones. La autonomía solo genera valor si el remedio es mejor que la enfermedad: un agente que alucina o pifia un precio agrava el problema que debía resolver.

---

## ✅ Checkpoint — Parte 2

*Respondé sin mirar el apunte. Las respuestas no están acá a propósito: van al complemento de la unidad.*

1. Nombrá las cinco fases del ciclo de sobreexpectación en orden y describí qué pasa en el abismo de desilusión.
2. "No encontramos el caso de negocio": ¿en qué fase de la curva se escucha esa frase, y con qué concepto de la Parte 1 se conecta directamente?
3. ¿Caer al abismo de desilusión significa que una tecnología murió? ¿Qué es lo que el valle efectivamente filtra?
4. ¿Por qué los ERP no aparecen en el ciclo de sobreexpectación — y qué relación tienen igualmente con él?
5. ¿Qué pregunta responde cada nivel de análisis (descriptivo, predictivo, prescriptivo)? Da un ejemplo de cada uno.
6. ¿Por qué hoy "ya no alcanza" un sistema que registra bien y muestra reportes excelentes del pasado?
7. Systems of record, of engagement y of action: función principal y un ejemplo de cada uno.
8. ¿Los sistemas de acción reemplazan a los sistemas de registro? Justificá con la relación entre ambas capas.
9. En el caso de la crisis nocturna: ¿qué detecta el sistema, qué hace cada agente de la cadena, y con qué se encuentra el equipo humano a la mañana?
10. ¿Qué piezas componen el marco de gobernanza de un sistema agéntico, y qué tipo de consecuencias — más allá de las reputacionales — busca evitar?

---

**Siguiente: Parte 3 — Los ERP propiamente dichos: la empresa como sistema, la definición, silos, niveles de decisión, trazabilidad, interfaces e historia.**

**FIN DE LA PARTE 2**
