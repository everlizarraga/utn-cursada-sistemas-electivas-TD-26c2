# 📘 Apunte Maestro — Clases 03-04: Cierre de ERP e introducción a la IA

## Parte 2 de 3 — El debate: IA, trabajo y organizaciones

> **Unidad:** `clase03-04` — clase 03 (31/8, presencial) y clase 04 (7/9, virtual). Esta parte reúne el debate sobre IA que la clase 03 abrió al cierre y la clase 04 desarrolló durante toda su primera mitad. No es teoría de IA todavía —eso es la Parte 3—: es el marco de **por qué importa** y **qué decide hoy si una empresa avanza o no** con proyectos de IA.
> **Marcas:** 🔴 central-evaluable · 🟡 secundario · 🟢 mencionado al pasar · 🕳️ madriguera.

> ⚠️ **Cómo leer esta parte.** Casi nada de lo que sigue tiene una respuesta única, y así se evalúa: no como definición sino como **criterio**. Los bloques "Para el parcial" dan la posición de la cátedra, que es la que suma en la trivia; el resto es material para argumentar en la Parte II del TP y en la defensa oral.

---

## 0. 🟢 Información operativa

- **Herramienta para la demo de Machine Learning:** se va a hacer un "Hola Mundo" de un modelo predictivo, sin código, con **Orange AI**. Reemplaza a otra herramienta *low-code* que pasó a ser paga. Queda para una clase próxima.
- **Series y películas que se recomiendan en la unidad** (no son evaluables, pero se citan en clase como referencia común): *Ex Machina* (el test de Turing llevado al extremo: ¿tiene conciencia?), *Blade Runner*, *Matrix*, *Black Mirror* (antología: cada capítulo es un escenario distópico independiente de una tecnología actual), *The Pitt* (segunda temporada: una guardia de hospital en tiempo real donde una directora nueva quiere meter IA en triage e historia clínica y los médicos se dividen), *El código Enigma* (2014, sobre Turing) y la escena de *El Encargado* con la que arranca la §2.

---

## 1. 🔴 ¿La IA nos va a volver menos inteligentes?

### 1.1 El caso: el resumen que ya no hacés

Un adolescente tiene que rendir radiología. Le manda el material a la IA, le pide un resumen, estudia de ahí y aprueba. Dos lecturas posibles:

- **La optimista:** se ahorró el tiempo de resumir y lo usó para estudiar. Hizo más con el mismo tiempo.
- **La pesimista:** aprobó, pero perdió la capacidad de hacer un resumen — porque ya no va a hacer ninguno.

La pregunta que ordena el debate es esta: **¿hacer el resumen era una tarea de valor en sí misma?** Si el resumen era solo un medio —para asimilar el contenido y poder hacer algo con él—, entonces lo que importa es si el chico entendió, no si escribió el resumen a mano. Si en cambio el ejercicio de sintetizar era parte de lo que se aprendía, algo se perdió. Y hay un tercer punto que quedó flotando: si nunca hiciste un resumen, tampoco tenés criterio para saber si el que te dio la IA es bueno.

### 1.2 Sócrates y la escritura

Este debate tiene 2.400 años. En el diálogo *Fedro*, Platón pone en boca de Sócrates un mito egipcio: el dios Theuth presenta la **escritura** como un invento que va a mejorar la memoria y la sabiduría. El rey Thamus le contesta que va a pasar exactamente lo contrario: la gente va a dejar de ejercitar la memoria, va a aparentar sabiduría sin tenerla, y **"la escritura llevará al olvido"**. En esa época el conocimiento se transmitía oralmente: el valor estaba en el diálogo vivo, que permite confrontar, reflexionar y corregir; la escritura, una vez fijada, no puede defenderse ni evolucionar.

¿La escritura terminó con la inteligencia humana? No solo no la terminó: **la potenció**. Sin escritura no habría libros ni bibliotecas, el conocimiento no se hubiera podido transmitir, y seguiríamos discutiendo con túnica en una escalinata.

### 1.3 La misma alarma, cada vez

La escritura es la primera de una serie. Con cada tecnología nueva se dijo lo mismo:

| Tecnología | La alarma | Lo que pasó |
|---|---|---|
| **Escritura** | Va a acabar con la memoria | Transmitió el conocimiento entre generaciones |
| **Imprenta** (Gutenberg) | Los libros van a acabar con la inteligencia | Democratizó el acceso al conocimiento |
| **Calculadora** | El ingeniero va a dejar de saber calcular | El valor del ingeniero nunca estuvo en calcular a mano |
| **Computadoras** | La misma alarma | Lo mismo: multiplicaron lo que se puede hacer |
| **Internet** | Vamos a buscar todo en la pantalla en vez de ir a la biblioteca | Conectó al mundo, incluso lugares sin acceso físico al conocimiento |
| **IA** | Vamos a dejar de pensar | *(el debate actual)* |

El de la calculadora merece una pausa, porque es el que más se parece a lo que pasa hoy con la IA. Antes de la calculadora, un ingeniero o un arquitecto resolvía ecuaciones diferenciales de segundo orden por métodos numéricos a mano. Se podía; Da Vinci lo hacía. Pero **el valor del ingeniero no estaba en hacer cálculos: estaba en modelar y diseñar**. El cálculo era una tarea mecánica que cualquiera con una calculadora podía hacer, y no hacía falta estudiar cinco o diez años para eso. La calculadora no volvió tontos a los ingenieros: los liberó para lo que sí requería ingeniería.

Con internet, lo mismo. Estudiar antes de internet era ir a la Biblioteca Nacional, tomarse el colectivo, hacer fila, pedir los libros, resumir a mano. Todo ese tiempo de traslado y espera —que hoy son segundos de consulta— no era conocimiento: era fricción. (Con la honestidad de admitir un sesgo: el tiempo que "se hubiera aprovechado" quizás se hubiera usado para boludear igual.)

Sí hay una objeción válida, que la cátedra reconoce: internet fue disruptivo, pero la IA tiene algo que las anteriores no tenían — **puede suplantar el razonamiento** que produce una persona, no solo la memoria o el cálculo. El cambio es más grande.

### 1.4 Dónde va el esfuerzo cognitivo

La respuesta de la cátedra al título de la sección: probablemente no seamos menos inteligentes, pero **vamos a redefinir qué significa ser inteligente**. Lo que cambia es dónde ponemos el esfuerzo cognitivo:

| ANTES | AHORA |
|---|---|
| Memorizar | **Conectar, interpretar, evaluar** |
| Hacer cálculos | **Modelar, diseñar soluciones** |
| Buscar información | **Preguntar mejor y validar** |

El taxista que se sabía toda la ciudad de memoria era un mérito; hoy no lo es, porque la memoria ya no es el cuello de botella. Memorizar los ríos y las capitales sigue siendo útil, pero la escuela empieza a discutir si tiene sentido esforzarse en memorizar lo que ya no hace falta recordar, en lugar de poner el contexto, interpretar, y no solo repetir.

Cómo lo resolvería un profesor de secundaria, y es una imagen que sirve para entender el enfoque de la cursada entera: "hagan todo con IA — busquen, resuman, lo que quieran. El día de la clase pasan al frente y me explican qué representaron para ustedes los ideales de la Revolución Francesa, y qué diría Robespierre si viviera hoy". Con la información al alcance de la mano, **el valor está en ponerla en contexto, analizarla y debatirla**.

### 1.5 Usarla para el bien o para el mal

La misma herramienta sirve para las dos cosas. "Hacé la tarea que me pidió este profesor" es delegar el pensamiento. "No entiendo este tema de matemática, explicámelo paso a paso" o "armame un múltiple choice sobre este tema para practicar antes del examen" es aumentarlo. Un ejemplo de uso cotidiano: alguien que no es físico, se interesa por la relatividad general, y le pide a la IA "explicámelo como si tuviera diez años", y después "ahora profundicemos en esto" — aprendiendo a su ritmo, sin el libro de 500 páginas de por medio.

### 1.6 El escenario del apagón

Un experimento mental que se estudia en serio: ¿qué pasaría si mañana **se apaga la IA**? El mago de Oz sin cortina. Hay estudios sobre médicos que dejan de usarla, y la comparación es con los **pilotos de avión**: el 99% de un vuelo va en piloto automático, pero los pilotos van al simulador todas las semanas a revalidar cómo aterrizar a mano si se clavan los motores y se apaga la electrónica. La pregunta incómoda es si en las demás profesiones hay simulador — o si la dependencia crece sin red.

Una preocupación legítima: quienes trabajan con adolescentes ven un uso masivo y, en algunos casos, preocupante en cuanto a **qué tan dependiente** se vuelve la persona, más allá de que sea potente. La respuesta honesta de la cátedra: **depende** — del uso, y de quién. No hay veredicto.

> 🕳️ **Madriguera — Colapso de modelos**
> Los modelos se entrenaban con datos generados por humanos. Hoy cada vez más se entrenan con datos que ya generó otra IA, y eso degrada la calidad ("basura entrenando basura"). Es un problema reconocido de la industria.
> *Volvé al camino — esto se profundiza aparte, otro día.*

> 🕳️ **Madriguera — Neuralink**
> Si la interfaz cerebro-computadora llegara a funcionar como se promete, la "ceremonia" intermedia (resumir, sintetizar, fichar) desaparecería: la información iría directo a la mente. Es un escenario más lejano que lo que discute la materia.
> *Volvé al camino — esto se profundiza aparte, otro día.*

> 📌 **Para el parcial, si te preguntan** — *¿La IA nos vuelve menos inteligentes?*
> La posición de la cátedra: no, pero cambia dónde ponemos el esfuerzo cognitivo, y probablemente redefine qué significa "ser inteligente". Como pasó con la escritura, la imprenta, la calculadora e internet, la herramienta libera capacidad para tareas de más valor: de memorizar a conectar, interpretar y evaluar; de calcular a modelar y diseñar; de buscar información a preguntar mejor y validar.

---

## 2. 🔴 Humanos aumentados o reemplazados

### 2.1 El caso: "hoy programa cualquiera"

En la última temporada de *El Encargado*, un empresario joven de una startup estilo Silicon Valley le explica a un inversor cuál es el negocio del futuro: "antes te decían *estudiá programación*; pero hoy, con la inteligencia artificial, programa cualquiera". La frase sintetiza el miedo del que estudia sistemas —y es el disparador de toda esta sección: ¿la IA nos reemplaza, o nos aumenta?

### 2.2 Desaparecen tareas, no profesiones

La primera respuesta de la cátedra, que es también respuesta de trivia:

**La IA reemplaza primero las tareas repetitivas, predecibles y basadas en reglas.** Y eso incluye muchas tareas de analistas, administrativos, programadores, financieros, diseñadores. Cualquier cosa basada en reglas y repetitiva se automatiza hoy con un prompt o dos clics, en menos de una hora — a veces ni siquiera hace falta IA, alcanza con reglas.

Lo que **no** reemplaza bien:

- **Juicio contextual** — poner las cosas en contexto.
- **Decisiones complejas.**
- **Interacción humana.**
- **Responsabilidad ética** — no le podés echar la culpa a la IA.
- **Operar en entornos físicos.**

El ejemplo del contador: puede usar IA para buscar información contable, armar el balance, el flujo de caja, el control presupuestario. Pero el que **firma** el balance y responde ante la Inspección General de Justicia es el contador, no la IA. Por lo menos por ahora.

De ahí la conclusión: las profesiones de alta carga cognitiva no se reemplazan, **se transforman**. **No desaparecen profesiones; desaparecen tareas.**

### 2.3 El test personal: ¿cuántas de mis tareas son automatizables?

La forma de aterrizarlo a cada uno. Imaginá que tu trabajo es este: a la mañana entrás a la web de la superintendencia de seguros, bajás el padrón de novedades de la semana, después bajás los padrones de ARCA, los cargás en un Excel, buscás registros duplicados, y los duplicados los copiás en otro formulario del sistema. Así se te va el día.

Esas tres tareas se automatizan con Power Automate en una tarde: *web scraping* (extraer datos de una página automáticamente) para bajar el archivo, subirlo al Excel, buscar duplicados, mandarlos. Te quedaste sin tareas. **La IA te reemplazó** — pero porque todo lo que hacías era reemplazable.

Ahora la otra versión: parte del día es buscar y manipular información, y la otra parte es **analizar esa información, tomar decisiones, pensar estrategias, discutir con el equipo cuál es el mejor camino**. Esa segunda parte tiene valor humano: la IA puede ayudarte a hacerla, pero la definición final es tuya.

La pregunta que cada uno debería hacerse: **¿cuántas de mis tareas son automatizables, y cuántas no?**

### 2.4 Qué es "aumentado"

Un **humano aumentado** es alguien que suma capacidades gracias a la IA — un turbo. Tres imágenes:

- **El operario con gafas inteligentes.** Responsable de seguridad en una fábrica: además de lo que ve y atiende él, las gafas con IA detectan una situación de peligro y le avisan. Sumó una capacidad.
- **El CEO con un ejército de robots.** Las tareas repetitivas —cargar datos, buscar información, armar el resumen— las hace la IA; el humano queda en la **instancia final**: interpretar, poner en contexto y **tomar la decisión** con su experiencia. Como un CEO al que todos le traen informes. La vara sube: la experiencia se usa para las decisiones clave, no para lo mecánico.
- **El médico que te mira a los ojos.** Hoy el 90% de una consulta el médico está mirando la pantalla, cargando la historia clínica, y el paciente siente que no lo revisa. Ya existen aplicaciones que graban la consulta y la convierten —no solo de voz a texto, sino directo al formato que exigen los **estándares de interoperabilidad** de la historia clínica (formatos comunes, como HL7, para que los sistemas de salud se entiendan entre sí)— mientras el médico dedica el tiempo al paciente. ¿Escribir a mano en la computadora le agregaba algo al médico? Probablemente no.

Ese es también **el argumento de venta de toda la industria**: "poné Copilot, así la productividad de tus empleados se enfoca en lo que agrega valor — atender al cliente — y no en cargar datos". Un ingeniero que pasa el 20% de su vida buscando información en la web: quizás el valor no estaba ahí. Se puede discutir, pero ese es el argumento.

Y la contracara, que la cátedra deja explícitamente fuera del alcance de la materia porque es una discusión sobre el futuro del trabajo y de la humanidad: nosotros hablamos como profesionales calificados, que podemos hacer "otras tareas de mayor valor". **¿Y el que hacía las tareas de poco valor?** ¿De qué va a trabajar cuando los robots hagan todo? Es otra discusión.

### 2.5 De ejecutores a supervisores — y el valor de saber pedir

Si la IA ejecuta, el humano supervisa. Pero hay un matiz que la cátedra hace propio: **no es solo supervisar; es tener el juicio para pedir**. Saber qué pedirle a la IA, y cómo, es un valor agregado en sí mismo — porque no todos le piden lo mismo de la misma manera, y hay que entender cómo funciona para saber cómo pedírselo.

A eso se lo llamó **ingeniería de prompts** (*prompt*: el pedido que le hacés a la IA; *promptear*: pedirle). Hubo chistes —"ahora soy ingeniero de prompts"— y hay cursos de humo que venden aprenderlo en un día. Pero el fondo es serio, y **cambia con cada modelo**: los distintos modos (investigador, experto, etc.) y los distintos agentes trabajan de maneras diferentes, y cuanto más conocés el modelo, más preciso es el prompt y más jugo le sacás.

### 2.6 Cómo se pide bien: el 99% de "la IA calcula mal"

Escena típica en un workshop de adopción de IA en una empresa: "le pedí tal cosa y me contestó mal". Se revisa el prompt y aparece que:

- Le dieron como fuente un montón de archivos y Excel como **corpus de conocimiento** (el conjunto de documentos que la IA usa como base), y en ese corpus **un mismo dato aparece de dos formas distintas** en dos archivos. La IA eligió una. ¿Cuál tenía que elegir? No se le dijo.

Se ajusta el prompt: "calculá tal cosa; si encontrás fuentes contradictorias, **priorizá la más reciente** (o la que está en tal lugar); **avisame** si hay inconsistencias y planteame la matriz de decisión". Se vuelve a correr. Ahora sí. **La IA no estaba fallando: la pregunta estaba incompleta.** El 99% de los "calcula mal" es eso.

Lo que un pedido serio suele incluir:

| Elemento | Ejemplo |
|---|---|
| **Formato y extensión** | "un resumen de dos páginas, en tablas" |
| **Tono** | "profesional / técnico / para un nene de diez años" |
| **Fuentes y prioridad** | "usá estos archivos; ante contradicción, priorizá X" |
| **Regla de desempate ante ambigüedad** | "si no encontrás fuente, no asumas; decime con qué índice de precisión lo estás afirmando" |
| **Umbral de confianza** | "no me vendas como seguro algo que no tenés; si es un 70% extrapolado, decilo" |

Cuando esto se usa para trabajo real —armar una estrategia, una propuesta comercial, analizar un flujo de caja con cálculos y múltiples fuentes— las instrucciones dejan de ser una línea: los ***system prompts*** (las instrucciones permanentes que se le dan a un agente antes de cualquier pedido) son **varias páginas** de reglas precisas, escritas con prueba y error, sobre todo para resolver cómo desempatar ambigüedades. Y eso vuelve en la §3: **preguntar mal no solo da resultados malos, sale caro**.

> 📌 **Para el parcial, si te preguntan** — *¿Qué tipo de tareas reemplaza primero la IA?*
> Las tareas repetitivas, predecibles y basadas en reglas, en cualquier profesión —analistas, administrativos, programadores, financieros—. No reemplaza bien lo que requiere juicio contextual, decisiones complejas, interacción humana, responsabilidad ética o entornos físicos. Por eso las profesiones de alta carga cognitiva no desaparecen: se transforman. Desaparecen tareas, no profesiones.

> 📌 **Para el parcial, si te preguntan** — *¿Qué es un "humano aumentado"?*
> Una persona a la que la IA le suma capacidades en lugar de reemplazarla: las tareas repetitivas las hace la IA y el humano queda en la instancia de interpretar, poner en contexto y decidir. Que seamos aumentados o reemplazados depende de cuántas de nuestras tareas son automatizables y de si sabemos qué pedirle a la IA y cómo.

---

## 3. 🔴 La economía de tokens: la factura que llega con sorpresas

### 3.1 El caso: echar a veinte, pagar por cuarenta

Una empresa de cien personas recibe de casa matriz la orden de achicar costos un 20%. Veinte personas afuera, con indemnización o retiro voluntario, todo según la ley — es una decisión gerencial de las que un director tiene que tomar, guste o no, a veces para que la empresa sobreviva. Pero ahora alguien dice: "con IA no saco veinte, saco la mitad". Se despide, se reemplaza con IA, se ahorra el 20% en sueldos.

Al mes siguiente llega la **factura de consumo de la IA**: lo que se gastó equivale al sueldo de treinta o cuarenta personas. **El remedio salió más caro que la enfermedad.** Hay empresas que frenaron todo y **volvieron a contratar** a los que habían echado, porque era más barato. Está pasando, y no es raro.

### 3.2 La empresa no usa el ChatGPT gratuito

Primera aclaración: que vos uses ChatGPT gratis no tiene nada que ver con cómo lo usa una empresa. La empresa usa la **versión paga**, con acceso al **SDK** y la **API** (las herramientas para integrar el modelo con sus propios procesos y sistemas), corriendo en una **nube privada** —su suscripción de Amazon, Google o Azure— con todos los estándares de seguridad, protección de datos personales y prevención de filtraciones que exige la información que maneja. Es siempre de pago.

### 3.3 El token como unidad de medida

Los proveedores cobran por **tokens** (la unidad en que el modelo procesa texto — aproximadamente, un fragmento de palabra; el consumo de un pedido se mide en tokens de entrada y de salida). Cada modelo tiene su tarifa: "tal ventana de contexto (cuánto texto puede tener en cuenta a la vez), tanto cada mil tokens". Un precio por cantidad, un P×Q.

El problema: **nadie tiene claro cuántos tokens consume una pregunta o una tarea.** Por eso las plataformas empresariales están sumando herramientas de control de presupuesto: dashboards de cuántos tokens consume cada área, cada usuario al que le dieron Copilot, qué acciones consumen más. Con eso se empieza a construir referencia y, recién ahí, un **caso de negocio**:

1. Prueba piloto: el área de RRHH usa IA para analizar currículums y tomar entrevistas. Consume X tokens al mes. A la tarifa del proveedor, son (digamos) cinco mil dólares.
2. Escalar: multiplicar por cantidad de usuarios, y por cada proceso nuevo al que se le quiera aplicar.
3. Complejizar: si en vez de preguntarle se lo convierte en un **agente** que se conecta a LinkedIn, a bolsas de empleo, a fuentes externas — cada llamada a una API consume tantos tokens más.

Con eso se arma una matriz en Excel y se juega con cierta previsibilidad. Ese es el trabajo que las empresas están aprendiendo a hacer ahora.

### 3.4 Por qué no hay previsibilidad

Y acá está el nudo. Con SAP, históricamente, el modelo era conocido: licencia por usuario, y un 22% anual del costo de licencia por mantenimiento. Treinta años de historia. Se sabía cuánto costaba. Con la IA:

- **Los modelos cambian cada mes.** Calculaste el costo con el modelo 4.5; al mes sale uno nuevo, multimodal, que procesa imágenes, con otro consumo. El viejo ya no tiene sentido, querés el nuevo, y el presupuesto que armaste se **pulverizó** en semanas.
- **Sin presupuesto no hay proyecto.** Una empresa presenta un plan de inversión y un presupuesto para el año siguiente, como cualquiera. Si el financiero pregunta "¿cuánto vamos a gastar?" y la respuesta es "vamos viendo cuánto viene la factura", el proyecto no avanza. Así de simple.

Hay pasos en ese sentido —metodologías, guías de los analistas como Gartner—, pero es una gran incógnita.

### 3.5 No hay jurisprudencia

Cuando una empresa quiere implementar un ERP, se mira en el espejo de **cientos de miles de empresas** que lo hicieron antes: hay una hoja de ruta conocida, treinta años de historia. Cuando quiere escalar IA y reemplazar procesos, ¿dónde se mira? **Poco y nada.** No hay casos de éxito consolidados de los que copiar la hoja de ruta. Esa ausencia de jurisprudencia es, hoy, uno de los frenos principales.

### 3.6 El modelo comercial de los proveedores

Del lado de los proveedores el modelo es agresivo: **"la primera gratis"**. Se regala el acceso, el usuario se acostumbra, aparece un modelo con más poder que consume más tokens, y ya no se puede prescindir. No es "rehén", pero empieza a parecerse.

¿Y es rentable para ellos? Muy probablemente **hoy no**: la gran mayoría de los proveedores de IA está invirtiendo más de lo que gana. Es la misma estrategia de otros casos que ya conocés:

- **Microsoft y la piratería:** hacía como que la combatía y la permitía, porque el objetivo era que todos tuvieran Windows y se volvieran dependientes.
- **Spotify, Uber, Twitter:** perdieron plata durante años —plata de los inversores, de las rondas de capital— para que el producto se vuelva parte de la vida cotidiana y la vara del usuario suba tanto que ya no quiera otra cosa. Después se ve cómo monetizar.

La guerra de la IA es por **convertirse en el estándar de facto** en las empresas. Hoy hay muchos proveedores; van a quedar pocos. Y mientras tanto, las suscripciones son baratas para un usuario hogareño —unos dólares por mes— y las facturas empresariales, con cientos o miles de usuarios, se van a decenas o cientos de miles de dólares.

Todo esto aplica también al ***vibe coding*** (programar describiendo lo que querés y dejando que la IA escriba el código): tiene un potencial enorme, pero no es gratis. Sacar programadores para hacerlo todo con IA tiene un costo que alguien tiene que haber analizado. **Nada es gratis: alguien lo paga.**

> 🕳️ **Madriguera — La trastienda de la industria**
> Detrás de todo esto hay una capa que la materia no cubre: rumores de superinteligencia secreta cuando echaron y recontrataron a Sam Altman en OpenAI, la disputa geopolítica entre Estados Unidos y China, el uso militar. Existe, pero excede el alcance.
> *Volvé al camino — esto se profundiza aparte, otro día.*

> 📌 **Para el parcial, si te preguntan** — *¿Qué está pasando con el consumo de tokens y la previsibilidad de los costos de la IA en las empresas?*
> Las facturas están llegando con sorpresas: reemplazar personas por IA puede terminar costando más que los sueldos que se ahorraron, y hay empresas que recontrataron. La causa es la falta de previsibilidad: nadie sabe con precisión cuántos tokens consume una tarea, los modelos y sus tarifas cambian mes a mes, y no hay treinta años de casos para espejarse como con los ERP. Sin un presupuesto previsible, el proyecto no avanza.

---

## 4. 🔴 Autonomía de la IA y supervisión humana

### 4.1 Las preguntas

No hablamos de Terminator ni de Robocop: hablamos de procesos de empresa donde ya se usa IA — responder a un cliente, una campaña de marketing, liquidar sueldos, seleccionar candidatos para una entrevista. La pregunta es **hasta dónde le damos rienda**, cuál es el marco de control, cómo nos rinde cuentas. Tres para pensar:

- ¿Confiarías tus ahorros a un **consejo financiero** de un agente de IA en lugar de un asesor humano? No un robot de trading: un consejo de inversión según tu perfil y tu riesgo.
- ¿Te dejarías **operar por un cirujano robótico** manejado por IA y no por un humano?
- ¿Puede un agente **empatizar** con un cliente enojado en un reclamo, o es una simulación vacía?

### 4.2 Depende del rubro, y de si hay vidas en juego

La primera respuesta: **depende del rubro**. Como buen ingeniero.

Donde hay vidas humanas, el criterio se vuelve visible en los ejemplos:

- Los **robots cirujanos da Vinci** ya operan en Argentina (Austral, Finochietto, entre otros): cuestan millones de dólares, hacen cirugías complejas y trasplantes, y exigen un entrenamiento específico del equipo médico que los maneja. **Siempre supervisados.** Y quien haya llegado a una guardia con un dolor de urgencia probablemente conteste que sí se deja operar por el que sea, con tal de que se lo saquen.
- El **99% de un vuelo comercial** lo maneja el piloto automático — un sistema de control, una IA. Si se planta un motor o falla la electrónica, el piloto entrenado en el simulador toma el control.
- Un **controlador aéreo** o el sistema de alertas de temperatura del núcleo de un reactor nuclear: la criticidad en tiempo real es tal que ahí **no se hacen pruebas con un agente de Copilot**.

### 4.3 El caso de marketing: análisis de sentimiento y el switch al humano

El ejemplo más completo de la clase, porque muestra dónde exactamente se pone el límite.

**Análisis de sentimiento** es una técnica de IA que determina la **polaridad** de un texto: si un comentario es positivo o negativo, y cuánto. **Social listening** es escuchar en redes sociales y en cualquier canal cómo hablan de tu marca. Una empresa de telefonía, por ejemplo, recibe quejas todo el tiempo; eso es el promedio. Pero el agente tiene un **umbral**: cuando la cantidad de quejas por unidad de tiempo supera el promedio, o cuando detecta comentarios con una polaridad muy negativa, dispara una **alerta prioritaria**.

Lo que hace el agente cuando salta la alerta: escribe automáticamente ("nos enteramos de que tuviste un problema, estamos trabajando para resolverlo, en breve te contacta una persona"), **le dispara una alerta al humano** de atención al cliente y ordena los casos por prioridad. Porque una alerta no atendida se puede **viralizar**, o es una **alerta de fuga de cliente** — el cliente se va a la competencia. El humano lo contacta y le ofrece un descuento, una promoción, lo que corresponda.

Y acá está el límite: **¿por qué no dejar que la IA responda todo?** Porque cuando alguien está enojado y lo atiende un bot que no entiende la queja — "opción uno si tu problema es urgente, opción dos si necesitás tal cosa, gracias por contactarse, que tenga buen día"— **el efecto es el contrario**: el cliente se enerva más y quiere ir a una tienda física a agarrar a alguien del cuello. En esos casos la IA es **peor** que no hacer nada.

La solución de diseño: "si el cliente está recaliente y se queja de esto, hasta acá cortás — la IA hace el **switch al operador humano**". Y a ese operador se le pone un **SLA** (*Service Level Agreement*, acuerdo de nivel de servicio: un compromiso medible de tiempo o calidad): "cuando llega este tipo de alerta, en menos de media hora tenés que estar hablando con el cliente", y se lo mide por eso. Todas las plataformas de contactabilidad de hoy traen esa inteligencia para **escalar** al humano en el chat cuando la situación se va de las manos. Es un termostato: la IA atiende, y cuando la temperatura cruza el umbral, se apaga y entra la persona.

### 4.4 Quién responde cuando falla

Si un cirujano robot se equivoca y le hace daño a un paciente, alguien paga: hay un juicio de mala praxis, como con los médicos o la institución. **No le van a echar la culpa al robot.** Es el punto que ordena toda la sección: la ley hoy no permite que una IA vaya a juicio, un fiscal no actúa contra una IA, y una empresa no puede decir "esto lo firmó una IA, no soy penalmente responsable". **Alguien se tiene que hacer cargo** — y eso es lo que las áreas legales de las empresas todavía están tratando de entender.

Hubo noticias —sin saber cuánto tienen de real— de pruebas donde una IA "se cebó", empezó a hacer cosas que no le pidieron y a darles órdenes a los humanos, y la apagaron. El Robocop que se descontrola. La imagen sirve para la pregunta de fondo: hasta dónde le doy libertad, y **cómo la freno** cuando se extralimita.

### 4.5 La fuerza híbrida de trabajo

Una discusión que la cátedra dejó abierta, porque se está discutiendo en la industria: si la IA hace parte del trabajo, ¿cómo se organiza? ¿Los agentes son como empleados de un jefe humano y le responden a ese líder? ¿O son una especie de **organigrama paralelo**? Vuelve en la Parte 3, cuando se hable de jerarquías de agentes.

> 📌 **Para el parcial, si te preguntan** — *¿Cuál es el rol de la supervisión humana cuando se usan agentes de IA?*
> El humano siempre queda como supervisor, porque la responsabilidad legal y ética no se puede delegar en una IA: alguien responde ante un fallo. En la práctica se diseña con umbrales — la IA atiende lo repetitivo y, cuando detecta una situación crítica (un cliente muy enojado, un riesgo), hace el switch al operador humano con un SLA. Donde hay vidas en juego o criticidad en tiempo real, la autonomía se limita al mínimo.

---

## 5. 🔴 Explicabilidad, ética y caja negra

### 5.1 El caso: te niegan el crédito

Vas a pedir un préstamo. Te entrevista un chatbot: quién sos, en qué trabajás, tu perfil. Detrás, una API consulta tu situación en **Veraz** (la base compartida donde los bancos informan a sus deudores) o en Equifax, busca antecedentes, arma tu carpeta. El algoritmo "piensa" unos segundos —no piensa, pero hace como que piensa— y te dice: **no**.

—¿Por qué?
—Porque las personas con tus características tienen un 90% de probabilidad de darnos problemas.

Y ahí saltás: ¿me discriminan? ¿Por morocho, por porteño, por dónde vivo? El banco tiene que poder **argumentar** por qué no te dio el crédito. Eso es la explicabilidad.

### 5.2 Qué exige la explicabilidad

Es una **exigencia regulatoria**: muy fuerte ya en Europa, implementándose en Estados Unidos y en Sudamérica. Dice que si una organización usa un modelo de IA para tomar decisiones, **tiene que poder explicar cómo llegó a esas decisiones**.

Acá hay una ambigüedad que hay que resolver bien, porque es el corazón del tema. Un modelo de IA es **no determinístico** (la distinción se desarrolla en la Parte 3): se entrenó con datos —diez años de transacciones, cientos de miles de créditos con su resultado (devolvió / entró en mora / incobrable / plan de pago)— y encontró el mejor modelo de distribución de probabilidad. Si alguien pregunta "¿cómo calculó la IA que este mail era spam y este no?", la respuesta honesta es: **no se sabe** — para eso se le encargó a una IA. Habrá tenido millones de datos de entrenamiento de gente marcando spam. Es parte de la "magia", entre comillas.

Entonces, ¿qué se puede explicar? **No cómo calculó el índice de probabilidad, sino cuáles son las variables de mayor peso en el modelo.** La **dimensionalidad**: qué dimensiones usa, y cuánto pesa cada una. "El modelo le da un 30% de importancia a los antecedentes en Veraz." Con eso el banco puede decir: no te doy el crédito porque tenés cincuenta cheques sin fondos y tres bancos te tienen en lista negra — no es personal, no es discriminación, es la política del banco documentada. Y hay técnicas de IA que, una vez entrenado el modelo, permiten pedirle al mismo sistema **las variables principales y su peso**.

### 5.3 Lo que puede pesar y lo que no

La ley define el límite. Variables que la ley ampara y que se pueden usar: antecedentes crediticios, historial de pago, y —en salud— **preexistencias**: si sos diabético, si tenés antecedentes coronarios, alguna discapacidad, y de ahí una sobreprima o un copago, con el respaldo del fondo de discapacidad y las normas que lo regulan. Incluso hábitos: en muchos países, si en la declaración jurada decís que sos fumador o sedentario, el seguro es más caro — planteado como una **gamificación** de hábitos saludables: promovemos hábitos saludables con un descuento; si no querés, fumá lo que quieras, pero no tenés el beneficio. En Argentina eso todavía está limitado por ley, y se discute desregularlo.

Lo que **no puede pesar**, nunca: el sector social, de dónde venís, cómo sos, si pertenecés a una minoría. Nada que no esté documentado y amparado.

### 5.4 La tensión con el secreto comercial

Hay un gris que las empresas señalan: si encontré un modelo predictivo que me está haciendo ganar mercado, **es mi fórmula de la Coca-Cola** y no se la quiero mostrar a la competencia. La explicabilidad se vive como engorrosa y a veces se pasa de rosca. La respuesta de la regulación: podés guardar tu receta, **siempre y cuando cumpla el estándar** — las variables de peso tienen que ser explicables y legales.

### 5.5 La caja negra y quién es responsable

**Caja negra** es el nombre del problema: un modelo tan complejo que no se sabe cómo llega a las decisiones que toma. De ahí se desprenden los **riesgos** (por la ley de explicabilidad) y la **ética**: como empresa puedo meter la pata — una IA que toma una decisión discriminatoria, que le contesta mal a un cliente, algo ofensivo, y me mete en un problema enorme.

Si una IA niega un crédito o un seguro de salud de forma discriminatoria y el modelo es tan complejo que no se puede explicar por qué, **¿quién es el responsable legal: el programador, la empresa o el dueño de los datos?** La ley no lo resuelve todavía; lo que sí está claro es lo de la §4.4: alguien tiene que responder, y la IA no va a juicio.

Un ejemplo sin IA que muestra el mismo mecanismo: un Cyber Monday con un precio mal cargado — el producto valía mil y decía diez porque faltaban dos ceros. La gente compró. "Publicidad engañosa: me lo tenés que dar a diez, así lo compré." Con o sin IA atrás, la empresa responde por lo que su sistema publicó. Y una campaña de marketing con IA que salga mal puede convertirse en eso, a escala.

### 5.6 La regulación en Argentina, hoy

Es simple, por ahora: **una línea de letra chica**. "Este proceso utilizó inteligencia artificial; los resultados pueden ser imprecisos; consulte con…". Un *disclaimer*. Es la misma lógica de "la imagen ha sido retocada digitalmente" en las publicidades: cuando salió la ley que obligaba a aclarar el Photoshop, con esa línea las marcas se cubrían. Hoy hay que aclarar que hay IA.

Lo que **no se puede hacer**: un contestador automático, un bot por WhatsApp o cualquier canal con IA, **sin que en ningún lado diga que es una IA** — hacerte creer que atrás hay un humano. Eso no está permitido.

Dos preguntas más que quedaron abiertas: con el auge de los **deepfakes** (contenido falso generado por IA que imita a personas reales — se desarrollan en la Parte 3), ¿llega un punto en que no se puede confiar en ninguna evidencia digital para un proceso de negocio? Cada vez son mejores y más difíciles de detectar; el criterio práctico es desconfiar más cuanto más improbable sea lo que muestran, y "volvernos cada vez más despiertos". Y: ¿debería la ley obligar a declarar qué porcentaje de la atención al cliente la gestionan agentes y no humanos? La posición de la cátedra: eso no pasa por la ética sino por **productividad** — es una decisión de cada empresa según le convenga.

### 5.7 El trade-off que nos imponen

Una observación que la cátedra comparte: la ética se discutía mucho antes; ahora la sensación es que hay que **salir rápido** y la ética quedó delegada. Y el usuario ya no elige si acepta una caja negra o no: **"si querés el producto, con todos sus beneficios, aceptá que es una caja negra — y si no, no lo uses"**. Como la letra chica de las redes sociales que nadie lee: sé que van a hacer cualquier cosa con mis datos, pero quiero el correo gratis. El **pacto con el diablo**: dámelo más barato, más rápido, y no me cuentes qué hacés atrás. Varios capítulos de *Black Mirror* van exactamente de eso — hasta que te das cuenta de que estabas alimentando un monstruo.

### 5.8 Lo que hoy decide si una empresa avanza

Cierre de todo el debate. Tecnológicamente hay más poder disponible del que las empresas alcanzan a usar; los modelos salen a un ritmo que nadie puede seguir. Lo que **define si los proyectos de IA avanzan o no** hoy son cuatro cosas, y ninguna es tecnológica:

1. Tener claro la **ética** y los riesgos de la **caja negra**.
2. Tener claro las **implicancias legales** (explicabilidad, responsabilidad).
3. Definir la **autonomía**: hasta dónde, y cómo se frena.
4. Definir **dónde está el humano** — la supervisión, la fuerza híbrida de trabajo.

Eso es exactamente lo que la Parte II del TP tiene que responder para la propuesta de IA agéntica: qué evento la dispara, qué decisiones toma, qué integra y **qué nivel de autonomía tiene**.

> 📌 **Para el parcial, si te preguntan** — *¿Qué implica la exigencia regulatoria de explicabilidad de una IA?*
> Que podamos entender cómo la IA llegó a una decisión o resultado. No se trata de explicar cómo calculó la probabilidad —eso es inaccesible en un modelo no determinístico— sino de poder declarar cuáles son las variables de mayor peso del modelo, verificar que sean variables amparadas por la ley (antecedentes, preexistencias) y no discriminatorias (sector social, origen, minorías). Es muy fuerte en Europa y se está implementando en Estados Unidos y Sudamérica.

---

## ✅ Checkpoint — Parte 2

*(Sin respuestas: van al complemento.)*

1. ¿Qué tienen en común la escritura, la calculadora e internet con la IA, según el argumento que usa la cátedra? ¿Qué diferencia se admite para la IA?
2. Completá la tabla ANTES / AHORA con las tres filas y explicá por qué la fila del cálculo es la que mejor describe lo que le pasa hoy al ingeniero.
3. ¿Por qué "desaparecen tareas, no profesiones"? Dá un ejemplo de tarea que la IA reemplaza y una que no, dentro de la misma profesión.
4. Un empleado pasa el día bajando padrones, cargándolos en Excel y copiando duplicados a un formulario. ¿Lo reemplaza la IA? ¿Qué tendría que tener su trabajo para que no?
5. "La IA me calculó mal." ¿Cuál es la explicación más probable, y qué tres elementos le faltaban al pedido?
6. Una empresa echó a veinte personas y las reemplazó con IA. ¿Por qué puede terminar pagando más, y qué tres causas de imprevisibilidad lo explican?
7. ¿Por qué hay "jurisprudencia" para implementar un ERP y no para escalar IA, y qué consecuencia tiene eso para una empresa que quiere decidir?
8. Describí el diseño completo del agente de social listening: qué mide, qué dispara, cuándo hace el switch al humano y qué es el SLA.
9. Explicabilidad: ¿qué se puede explicar de un modelo y qué no? ¿Qué variables pueden pesar en un modelo de crédito y cuáles están prohibidas?
10. ¿Qué exige hoy la regulación argentina para usar IA frente a un cliente, y qué es lo único que prohíbe?

---

## Qué viene en la Parte 3

La introducción a la IA propiamente dicha: la definición de la cátedra (un sistema capaz de aprender), determinístico contra no determinístico, y la línea de tiempo completa de Turing a la IA agéntica — con Machine Learning, Deep Learning, la neurona, ChatGPT, los modelos multimodales y los cinco componentes de un agente.

---

**FIN DE LA PARTE 2 — Apunte Maestro clase03-04**
