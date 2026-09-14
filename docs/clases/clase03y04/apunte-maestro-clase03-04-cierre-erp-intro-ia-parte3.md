# 📘 Apunte Maestro — Clases 03-04: Cierre de ERP e introducción a la IA

## Parte 3 de 3 — Introducción a la IA: de Turing a la IA agéntica

> **Unidad:** `clase03-04` — clase 03 (31/8, presencial) y clase 04 (7/9, virtual). Esta parte es la introducción formal a la inteligencia artificial: primero la definición que usa la cátedra y de la que se deriva todo lo demás, después la línea de tiempo completa. Cubre la **Parte I de la unidad temática "Tecnologías emergentes"** (unidades 7-9 del programa), adelantada a estas clases.
> **Marcas:** 🔴 central-evaluable · 🟡 secundario · 🟢 mencionado al pasar · 🕳️ madriguera.

> 💡 **Alcance.** Cuando se dice "IA" se dicen muchas cosas a la vez: modelos predictivos, Machine Learning, chatbots, agentes, IA generativa, redes neuronales. Todo tiene que ver con todo porque **son subconjuntos de la IA**, y la línea de tiempo existe justamente para ordenar cómo se relacionan y qué tipo de aplicación es cada cosa. El objetivo es entender el **estado del arte** —la expresión, traducida del inglés, significa la tecnología disponible hoy: qué se puede hacer, qué está accesible y qué pueden usar concretamente las empresas—.

---

## 1. 🔴 La definición de la cátedra: un sistema capaz de aprender

### 1.1 El caso: "esperá, que el sistema está pensando"

La ruedita gira y decimos "está pensando". No está pensando: **está procesando**. Un sistema operativo que hace *round robin* (como viste en Sistemas Operativos: repartir el procesador entre tareas por turnos, dando la ilusión de simultaneidad) tampoco piensa. Una IA que toma decisiones y nos responde cosas que parecen pensadas, tampoco: está procesando unos y ceros en función de un entrenamiento que le dimos. La ilusión de pensamiento es exactamente eso, una ilusión.

Ese punto de partida sirve para preguntarse, con precisión, **qué compartimos los humanos con las máquinas y qué no**.

### 1.2 Qué compartimos y qué no

| Capacidad | ¿La tiene la máquina? | Por qué |
|---|---|---|
| **Conciencia** | No | La máquina no es consciente de que es una máquina. Que la IA "tome conciencia" es el escenario de la ficción —*Matrix*, *Ex Machina*—; si pasara, estaríamos subyugados. Procesa modelos, no tiene consciente ni subconsciente. |
| **Empatizar** | No | La empatía es un sentimiento humano: ponerse en el lugar del otro, conmoverse. La máquina **me hace creer** que empatiza; no lo hace. |
| **Pensar** | No | Procesa, no piensa, en el sentido del pensamiento humano. |
| **Aprender** | **Sí** | Puede sumar conocimiento nuevo, reentrenarse y mejorar los modelos con los que decide. Aprende de un modo distinto al humano, pero aprende. |

El caso de la empatía tiene un ejemplo real y polémico: las aplicaciones de acompañamiento en salud mental con IA, donde una persona con depresión habla con un "terapeuta" artificial. Los psicólogos y psiquiatras se oponen en buena parte, y la pregunta de fondo es la de la Parte 2: si eso termina empeorando un cuadro grave, **¿cuál es la responsabilidad, y qué tan probado está?** Que la IA me haga creer que entiende mi dolor, y hasta que se convierta en confidente de lo que no me animo a decirle a un humano, no significa que empatice.

### 1.3 Cómo aprende una máquina

Aprender, para una máquina, es **entrenar modelos**. Hay distintas técnicas —**supervisado**, **no supervisado**, **por refuerzo**— que por ahora alcanza con saber que existen; el ejemplo de esta unidad es el supervisado: se le dan casos etiquetados y aprende de ellos.

El sistema antifraude de un banco: tiene un millón de casos históricos etiquetados — "esta transacción fue fraude, esta no". Ayer se descubrió uno nuevo: un cliente de Buenos Aires conectándose a las tres de la mañana desde Islas Caimán para hacer una transferencia (una **geobarrera** —regla de ubicación— lo hubiera marcado). Se le agrega al modelo. Ahora tiene un millón uno. **¿Es más inteligente que ayer?** Sí, en un 0,000001 — pero más inteligente.

De ahí la regla que usa la cátedra: **con cada dato o ejemplo nuevo, el modelo queda igual o más inteligente**. Poquito o mucho, no importa. A lo sumo se queda igual: si le agregás un caso que ya conocía (alguien con más de diez entradas en Veraz ya disparaba todas las alertas), el modelo está **sobreentrenado** para ese patrón — no aprende nada nuevo, pero tampoco empeora. Más datos de entrada, más aprende.

La única forma de que empeore es **darle datos malos**: corruptos, duplicados, inconsistentes. Igual que un empleado nuevo al que le explicás el trabajo al revés a propósito: mañana hace todo mal, no porque no pueda aprender sino porque aprendió lo incorrecto. La IA **potencia el error** que le diste — que es la lección del RPA en la Parte 1.

### 1.4 Determinístico y no determinístico

Esta distinción es la base de todo lo que sigue, y viene de lo que ya viste con autómatas en Sintaxis y Semántica.

Un **modelo determinístico** es aquel donde igual entrada produce igual salida: si conozco las entradas, sé cuál va a ser la salida. Un algoritmo —una serie de pasos que calcula algo, una raíz cuadrada— se puede ejecutar una vez, dos, cien mil veces y el resultado es siempre el mismo. Un autómata finito determinístico llega a una salida a través de sus estados de forma predecible.

Un modelo de IA es **no determinístico**: no puedo prever la salida. Un modelo predictivo, un sistema antifraude, un filtro de spam: nunca dan el mismo resultado exacto, y nunca llegan a certeza. La curva se acerca a uno **asintóticamente, pero nunca es uno**. El sensor de huella que desbloquea tu teléfono detecta que sos vos con un 99,99%; una radiografía leída por un modelo, ídem; el piloto automático de un avión, un robot de cirugía — todos con una precisión altísima, y todos con un posible punto de falla, porque dependen de los datos. Si fuera uno, no sería inteligencia artificial: sería un algoritmo.

Una frase de Harari que la cátedra cita para esto: *el riesgo de la inteligencia artificial es que no sabemos lo que va a hacer; si lo supiéramos, no sería inteligencia artificial, sería un algoritmo.* La conclusión operativa: **la IA reduce la incertidumbre; no la elimina.**

### 1.5 Reglas contra ejemplos: si hay un `if`, no es IA

Hay problemas en las empresas que son algorítmicos, determinísticos: llega una factura, si es de tipo A va por acá, si es de tipo B por allá — es un flujo. Se programa con reglas. **Eso no es inteligencia artificial**; es programación tradicional.

¿Y cómo se determina si una transacción es fraude, o si un mail es spam? Las transacciones fraudulentas se parecen a las reales. Un filtro de spam con reglas —"si dice *príncipe nigeriano*, si vende Viagra"— lo esquiva cualquiera en dos minutos. ¿Cómo funcionaban de verdad los filtros? Vos marcabas con la banderita: "esto es spam". Eso se informaba al servidor de correo. Con millones de ejemplos etiquetados —esto es spam, esto no—, el modelo se entrenó buscando **patrones** y una distribución de probabilidad. **Nunca se le dio una regla.** Por eso los filtros de hoy son buenísimos comparados con los de hace años (y por eso a veces clasifican como spam una publicidad real de tu banco: un **falso positivo**, que corregís marcando "remitente seguro").

**Así aprendemos los humanos.** Cuando sos chico, ¿cómo aprendés a distinguir un perro de un gato? Nadie te programa "el hocico mide tantos centímetros, el ángulo de las orejas es tal". Te muestran: perro, gato, guau, miau. Con los primeros ejemplos se arma un patrón en tu cerebro, y en algún momento distinguís con precisión. **Generalizando casos particulares**, sin una sola regla.

El patrón de fraude, para que se vea la diferencia con la regla. Banco de Buenos Aires; un cliente se conecta desde Mar del Plata — se fue el fin de semana, normal. Otro hace una transacción desde Filipinas, al día siguiente desde Singapur, al otro desde Curazao. Salvo que sea un loco viajando por el mundo, es raro: probablemente hay un *proxy* atrás. ¿Qué información se le dio al modelo? **No** "si alguien se conecta desde Curazao es fraude" — vos podés irte de vacaciones a Curazao. Se le dieron casos históricos, y el modelo determinó solo que **el patrón** —tres lugares distintos con cierta frecuencia de tiempo— es sospechoso. Después habrá que ver si es un verdadero positivo o un falso positivo, pero eso es un patrón de fraude aprendido, no programado.

Y el quiebre de stock, para ver que "reglas" ni siquiera es posible en muchos casos. ¿Cuánto es "poco stock"? Depende. Una pieza que la línea de producción usa una vez al año: con cinco unidades tengo para un año, no es alerta. Helados en verano: con diez kilos me quedo sin nada en cinco minutos. No se le dice al sistema "cuando queden menos de N unidades"; se le dice "conectate al ERP, fijate todas las veces que tuve quiebre de stock, con sus previsiones y sus consumos, y **encontrá un modelo** que me anticipe los próximos". Datos y ejemplos; nunca reglas.

### 1.6 El Test de Turing, con la definición en la mano

Alan Turing planteó en 1950 un ejercicio teórico bajo la pregunta **"¿pueden pensar las máquinas?"**. Dos cortinas: detrás de una hay una persona, detrás de la otra un sistema. Yo hago preguntas —por escrito, por voz, no importa— y las dos me contestan, como en una prueba a doble ciego. Busco hacerlos pisar el palito. Si en algún momento una respuesta cualquiera me delata a la máquina, no hay IA. Pero si llega el momento en que **no puedo discernir dónde está la máquina y dónde está el humano**, estoy en presencia de una inteligencia artificial.

Ahora la pregunta que cierra la §1: **¿cuándo pasa eso?** Cuando el sistema es **capaz de aprender** y de mimetizarse con la persona — va aprendiendo, y por eso no logro distinguirlo. Ahí está la definición que la cátedra elige, y a la que vuelve cada vez: **estamos en presencia de inteligencia artificial cuando hay un sistema capaz de aprender.** Todo lo demás se deriva de ese concepto.

> 📌 **Para el parcial, si te preguntan** — *¿Cuál de estas características compartimos los humanos y las máquinas: conciencia, pensar, empatizar, aprender?*
> Aprender. Las máquinas no tienen conciencia (no saben que son máquinas), no piensan (procesan) ni empatizan (hacen creer que lo hacen). Sí aprenden: incorporan conocimiento nuevo y se reentrenan, de un modo distinto al humano pero real.

> 📌 **Para el parcial, si te preguntan** — *¿Qué plantea básicamente el Test de Turing?*
> Determinar si un sistema es capaz de aprender. El ejercicio consiste en hacer preguntas a una persona y a una máquina sin ver cuál es cuál: cuando ya no se puede distinguir a la máquina, hay inteligencia artificial — y eso ocurre cuando el sistema aprendió lo suficiente para mimetizarse. La definición de la cátedra: IA es un sistema capaz de aprender.

> 📌 **Para el parcial, si te preguntan** — *¿Qué diferencia a un modelo de IA de un algoritmo tradicional?*
> El algoritmo es determinístico: igual entrada, igual salida, resultado seguro. El modelo de IA es no determinístico: se entrenó con ejemplos, no con reglas, y produce una predicción con un nivel de precisión que se acerca a uno pero nunca lo alcanza. Si el problema se resuelve con un `if`, no es IA. La IA reduce la incertidumbre, no la elimina.

---

## 2. 🔴 La línea de tiempo: cómo llegamos hasta acá

Ocho hitos, elegidos entre muchos posibles, para entender cómo se avanzó tan rápido en los últimos años hasta el estado del arte de hoy.

```
 1950 ●── TEST DE TURING          ¿pueden pensar las máquinas?
      │
 1966 ●── ELIZA                   el primer chatbot
      │
 1980 ●── SISTEMAS EXPERTOS       replicar el razonamiento del experto (reglas)
      │
 1986 ●── MACHINE LEARNING        aprender de datos ESTRUCTURADOS
      │      ┆ "invierno de la IA"
 1997 ┆      Deep Blue vence a Kasparov
      │
 2012 ●── DEEP LEARNING           redes neuronales · datos NO estructurados
      │
 2022 ●── CHATGPT                 30/11/2022 · IA generativa para cualquiera
      │
 2024 ●── GPT-4 MULTIMODAL        pedir en un modo, responder en otro
      │
 2025 ●── IA AGÉNTICA             agentes autónomos con objetivos
```

Y cómo se anidan las cosas que la línea va presentando:

```
 ┌─────────────────────────────────────────────────────────┐
 │  INTELIGENCIA ARTIFICIAL — sistema capaz de aprender    │
 │   ┌─────────────────────────────────────────────────┐   │
 │   │  MACHINE LEARNING — aprende de datos             │   │
 │   │   ┌─────────────────────────────────────────┐   │   │
 │   │   │  DEEP LEARNING — redes neuronales        │   │   │
 │   │   │  (imagen, voz, video, lenguaje → LLM,    │   │   │
 │   │   │   IA generativa, multimodal, agentes)    │   │   │
 │   │   └─────────────────────────────────────────┘   │   │
 │   └─────────────────────────────────────────────────┘   │
 │   (aparte, y anteriores: sistemas expertos, chatbots     │
 │    de reglas — "IA" según a quién le preguntes)          │
 └─────────────────────────────────────────────────────────┘
```

### 2.1 🔴 1950 — Alan Turing

Alan Turing (1912-1954) se hizo famoso al descifrar el **código Enigma** de los nazis en la Segunda Guerra Mundial — se considera que ayudó a los aliados a ganar la guerra. La máquina con la que lo hizo era, en el fondo, una implementación de un autómata finito determinístico. Es considerado el **padre de la inteligencia artificial** tal como la entendemos hoy: en 1950 abrió un artículo con la pregunta *¿pueden pensar las máquinas?* y planteó el test que ya viste en la §1.6.

Lo que no es obvio es cuánto de lo actual responde a Turing. Los **CAPTCHA** —"no soy un robot", el texto distorsionado, "marcá los semáforos"— son un test de Turing al revés: no busco saber si la máquina parece humana, sino **si del otro lado hay una persona o un robot**, para evitar spam, bots y ataques de denegación de servicio. La sigla lo dice: *Completely Automated Public **Turing** test to tell Computers and Humans Apart*. Y toda la IA generativa, la detección de si una imagen es real o generada, la conducción autónoma — de alguna manera, todo está intentando responder al test de Turing.

Sobre su vida, con su final triste, está la película *El código Enigma* (2014). Y *Ex Machina* lleva el test al extremo: un programador es llevado a una casa aislada para hacerle el test de Turing a una androide, y la pregunta se vuelve si tiene conciencia.

### 2.2 🟡 1966 — ELIZA, el primer chatbot

Quince años después, en el MIT, el primer programa que simulaba una **conversación**: ELIZA, un terapeuta **rogeriano** (una escuela de psicología centrada en hacer sentir al paciente escuchado y comprendido). El usuario escribía frases y ELIZA respondía con preguntas o comentarios aparentemente empáticos:

```text
ELIZA: Is something troubling you?
YOU:   Men are all alike.
ELIZA: What is the connection, do you suppose?
YOU:   Well, my boyfriend made me come here.
ELIZA: Is it important to you that your boyfriend made you come here?
```

**No comprendía nada.** No tenía un LLM (*Large Language Model*, modelo de lenguaje de gran escala: la tecnología detrás de los chats actuales, que aparece más adelante) ni nada parecido: aplicaba **reglas muy simples**, como un árbol de decisión, y daba la sensación de que entendía por dónde iba la conversación. Para la época, un hito.

Una aclaración de vocabulario que hoy confunde: *chatbot* y *agente* no son lo mismo. Chatbots existen desde 1966; el chatbot tradicional es el que respondía sobre un menú estructurado y si escribías con una falta de ortografía te decía "no entiendo la pregunta". Hoy algunos llaman a un chatbot "agente conversacional", y hay agentes de baja y de alta autonomía; lo que es un agente de verdad se define en la §2.9.

### 2.3 🔴 1980 — Sistemas expertos

Un **sistema experto** es un programa que simula el **razonamiento y la toma de decisiones de un experto humano** en un dominio específico: medicina, ingeniería, finanzas, diagnóstico técnico. El primero famoso fue **MYCIN**, de la Universidad de Stanford, en los años 70: diagnosticaba infecciones bacterianas de la sangre y recomendaba antibióticos.

Cómo funciona, con un triage de guardia. El experto vuelca su conocimiento en **reglas**: si tuvo vómitos, preguntar esto; si tiene fiebre de más de 38, aquello; si es mujer, ¿está embarazada? El sistema va preguntando, acumula **hechos** (lo que el paciente respondió) y un **motor de inferencia** recorre esa especie de árbol aplicando los modos lógicos —*modus ponens*, *modus tollens*, los que viste en el paradigma declarativo de Paradigmas de Programación— hasta llegar a una conclusión. **No inventa nada ni se extralimita: sigue el camino que el experto le marcó.** Su ventaja es que lo hace mucho más rápido y sin equivocarse, donde el experto humano podría equivocarse.

Fíjense que tienen casi cuarenta años y **siguen vivos**. En salud, todos los sistemas de **autorizaciones y coberturas** son esto: "con este plan, ¿cuántas radiografías por mes autorizo?", según el plan, el riesgo, las reglas. Hoy se los llama **motores de reglas**: **Drools** (del ecosistema JBoss, en Java) es el más conocido; OpenRules, y los que traen SAP e IBM. Que sean "IA de verdad" es discutible — algunos dicen que no —, pero están en la historia y en las empresas.

### 2.4 🔴 1986 — Machine Learning: aprender de datos estructurados

A mitad de los 80 se popularizan los modelos de **Machine Learning** (aprendizaje automático): una rama de la IA que permite que un algoritmo **aprenda de los datos** y haga predicciones o tome decisiones sin estar programado explícitamente para cada tarea. Es exactamente lo de la §1.5, y se usa hasta hoy.

**La característica que lo define: trabaja con datos estructurados.** Un dato estructurado es aquel del que conozco la composición: tiene forma de tabla —fila, columna, registro—. Un Excel, una tabla de una base de datos SQL. Sé que el primer campo es *nombre* y es un texto de hasta 150 caracteres; el segundo es *DNI* y es numérico; el tercero es *CUIT*, dos dígitos, guión, ocho dígitos, guión, uno. Cuando tengo claro qué hay en cada fila y cada columna, eso es estructurado.

**Ejemplos típicos**, todos de la vida real de las empresas:

| Problema | Qué aprende el modelo |
|---|---|
| **Antifraude** | Cada transacción con su tarjeta, hora, lugar, monto — y una columna final: lícita o fraude. |
| **Quiebre de stock** | Historial de stock y consumo por material → cuándo me voy a quedar sin. |
| **Mantenimiento predictivo** | Datos de la máquina → cuándo se va a romper, para encontrar la ventana ideal de mantenimiento. |
| **Credit scoring** | Perfil e historial de créditos otorgados → si dar el crédito y por qué monto máximo. El "crédito en dos clics" de una billetera digital es esto: el monto máximo lo decide un modelo con lo que sabe de tu uso. |
| **Plan de ventas / producción** | Historial de ventas y variables de contexto → cuánto voy a vender. |

Sobre el último: no es extrapolar. "Vendí 100, 150, 200 autos; entonces 250": no, porque el presente es dinámico — cambió la ley, ahora puedo importar, hay menos cupo de exportación, cambió el tipo de cambio o el poder adquisitivo. El modelo se arma con el historial **y** esas variables.

**La metodología, en tres pasos.** Trabajar con Machine Learning es un proceso con muchos subpasos, pero se resume así:

1. **Análisis exploratorio.** Ver qué datos tengo y para qué me podrían servir. ¿Son buenos? ¿Tengo suficientes para el nivel de precisión que necesito? ¿Están **balanceadas las clases** (cuántos casos de fraude hay contra cuántos lícitos)? Acá se usan histogramas, distribuciones de frecuencias, y la **matriz de correlación** (de Pearson): qué variables se correlacionan con el resultado y **cuál mueve la aguja**. Si estoy modelando el precio de un seguro de salud según hábitos, ¿cuánto pesa ser fumador contra las demás variables? Son las variables de peso de la explicabilidad (Parte 2, §5.2).
2. **Entrenar y comparar algoritmos.** Hay muchos modelos probabilísticos y estadísticos —redes bayesianas, árboles de decisión, *gradient boosting*, los que viste en Probabilidad y Estadística— y funcionan mejor o peor según el problema: ¿es de **regresión** (predecir un valor continuo) o de **clasificación** (asignar una categoría)? Se entrenan varios y se ve cuál tiene mejor **bondad predictiva**.
3. **Testear y evaluar.** Probarlo, desafiarlo, medir a qué resultado llega, y decidir si está en condiciones de usarse.

**Quién hace esto.** En el mundo de datos hay tres perfiles: el **ingeniero de datos** (el más técnico: cómo conectarse a las bases, qué procesos corren, si va Big Data o nube, cuánta memoria), el **analista de datos o de negocio** (el que sabe qué preguntarle a los datos para que tenga sentido como problema de negocio) y, en el medio, el **data scientist**. Con qué: librerías de Python, RStudio, o herramientas **no-code** (sin programar) como la que se va a usar para el "Hola Mundo" de la unidad.

### 2.5 🟡 El invierno de la IA y 1997: Deep Blue vence a Kasparov

Desde Turing habían pasado casi treinta años sin avances que se pudieran palpar fuera de la investigación universitaria: la IA era una promesa. A ese estancamiento se lo llama el **invierno de la IA**.

En **1997** una máquina de IBM, **Deep Blue**, le ganó una partida de ajedrez a **Garry Kasparov** — número uno del mundo, uno de los mejores de la historia, "el ogro de Bakú" por su carácter. Fue la primera vez que una máquina venció a un humano en una actividad de alta cognición, y fue noticia en todo el mundo: una máquina del tamaño de una heladera, con un humano que replicaba en el tablero lo que la computadora decía, y los gestos de frustración de Kasparov. Después vinieron el **Go** —el juego chino de fichas blancas y negras, central en esa cultura y de altísima complejidad— y *Jeopardy*; hoy no queda casi juego donde la máquina no nos gane.

Ese hito **despertó el interés** y sacó a la IA del invierno. Es el mismo movimiento que la curva de Gartner de la clase 02: sobreexpectativa, caída, y una segunda oportunidad cuando la tecnología madura.

---

### 2.6 🔴 2012 — Deep Learning: redes neuronales y datos no estructurados

El **Deep Learning** (aprendizaje profundo) es un **subconjunto del Machine Learning**. La diferencia con lo anterior es de qué datos come: ya no solo datos estructurados, sino **datos no estructurados** — imágenes, video, voz, audio, lenguaje. Cuando alguien habla y yo proceso el audio, ¿qué estructura de campo y registro tiene eso? Ninguna. Una imagen borrosa, una imagen HD del cuerpo humano, del espacio, de un auto: no está estructurada. Con Machine Learning tradicional eso **no se puede hacer**; no está preparado para ese tipo de entrada. Para eso hacen falta **redes neuronales artificiales**, que intentan **emular cómo trabaja el cerebro** con un modelo matemático.

#### La neurona biológica

En el cerebro hay del orden de 80-100 mil millones de neuronas interconectadas. Cada una tiene un **soma** (el cuerpo, con el núcleo), **dendritas** (ramificaciones de **entrada**, que se conectan con otras neuronas) y un **axón** (la "cola" de **salida**, que se ramifica hacia otras neuronas). Cuando una neurona transmite un impulso eléctrico a la siguiente, eso es una **sinapsis**: así llega la información de lo que vemos a nuestro cerebro, y así aprendemos.

#### La neurona artificial: el perceptrón

Matemáticamente se emula con un modelo bastante simple, el **perceptrón**:

```
   NEURONA BIOLÓGICA                        NEURONA ARTIFICIAL (perceptrón)

   dendritas ──┐                             X1 ──W1──┐
   (entradas)  │  soma    axón               X2 ──W2──┼──▶ [ Σ (wi·xi) ] ──▶ f(activación) ──▶ y
   dendritas ──┼─(núcleo)══════▶ sinapsis    …        │         suma            sigmoidea       salida
   dendritas ──┘                             Xn ──Wn──┘       ponderada         → 0 ó 1
```

- **Entradas X1 … Xn**: los valores que llegan — equivalen a las dendritas.
- **Pesos W1 … Wn** (*weight*): cada entrada se multiplica por un peso, la importancia que se le da a esa dendrita.
- **Suma ponderada** Σ(wi·xi): X1·W1 + X2·W2 + … + Xn·Wn.
- **Función de activación**: representa al núcleo. Decide si la neurona "dispara" o no. ¿Y cómo se representa un impulso eléctrico en computación? Como todo: con **unos y ceros**. Si hay sinapsis —si se transmite el impulso a la siguiente— es un 1; si no, un 0. La función más usada es la **sigmoidea**: vale 0 para entradas bajas, y a partir de un **umbral** salta a 1 (hay otras similares, como la ReLU). Eso emula el estímulo: por debajo del umbral no pasa nada, por encima se activa.
- **Salida y**: el 0 o el 1 que va a la neurona siguiente.

> 🟢 Un paréntesis: si apagás la computadora no hay corriente, ¿dónde quedan los unos y ceros? En la **magnetización** del disco — los electrones orientados norte-sur o sur-norte; al prender, esa orientación se vuelve a leer como 0 y 1. Lo viste en Arquitectura de Computadoras.

#### La red: muchas capas de perceptrones

Una neurona sola no hace nada interesante. Una **red neuronal** es un modelo de **múltiples capas**: cada neurona le transmite a las de la capa siguiente, y así hasta la salida.

```
  Capa de     Capas ocultas                   Capa de
  entrada     (pueden ser miles)              salida
    ●─────┬──▶ ● ─────┬──▶ ● ─────┬──▶ ● ─────┬──▶ ●
    ●─────┼──▶ ● ─────┼──▶ ● ─────┼──▶ ● ─────┼──▶ ●
          ├──▶ ● ─────┼──▶ ● ─────┼──▶ ● ─────┘
          └──▶ ● ─────┴──▶ ● ─────┘
  (cada neurona conectada con TODAS las de la capa siguiente)
```

Con miles o millones de capas y de neuronas, la red puede trabajar con lo que un perceptrón solo no puede: reconocer patrones en imágenes, voz y video. Cómo se entrena una red es el algoritmo de ***backpropagation*** (propagación hacia atrás): con cada dato de ejemplo, la red se recorre hasta la salida, se mide el error, y **se vuelve hacia atrás ajustando los pesos** para minimizarlo — la misma idea de minimizar el error que viste en Estadística con mínimos cuadrados. Eso lo van a ver en detalle en Inteligencia Artificial, la materia.

#### Qué se puede hacer con esto

Todos estos ejemplos tienen redes neuronales atrás, y **ninguno se podría hacer con Machine Learning tradicional**:

- Detectar el **estado de ánimo y las microexpresiones** faciales en una entrevista: si abrís los ojos, si mentís, si estás triste, el tono de voz.
- Detectar vehículos y su flujo en una autopista; peatones en una calle; un camión desde la cámara de un auto.
- **Peritar siniestros**: una foto del auto chocado, y el modelo estima el daño.
- **Kinesiología remota** (una startup chilena): hacés los ejercicios de rehabilitación frente a la cámara, el modelo detecta tus posturas y te corrige, y el kinesiólogo ve todo después y arma la rutina.
- Desbloquear el teléfono con la **huella digital**.

#### Cuándo redes neuronales y cuándo Machine Learning

Entrenar una red neuronal es **más costoso, computacional y económicamente**, que usar un algoritmo de Machine Learning, que es bastante más trivial. La regla de la cátedra, otra vez: **no matar una mosca con un cañón**. Si el problema se resuelve con información estructurada —quiebre de stock, plan de ventas, otorgar créditos— se usa Machine Learning. Cuando hay que trabajar con voz, audio, imagen o video, redes neuronales. Desde 2012, aproximadamente, se empezó a hacer en forma masiva.

#### 2024: dos premios Nobel para las redes neuronales

En 2024 —primera vez en la historia— los Nobel de **Física** y de **Química** fueron para trabajos relacionados con IA:

- **Física:** John Hopfield y Geoffrey Hinton, por los descubrimientos fundacionales que permiten el aprendizaje con redes neuronales artificiales — entre ellos, el backpropagation. Fue polémico: muchos físicos decían "esto es computación, no física, denle un premio del MIT". Se consideró física porque esos algoritmos habilitaron avances en un montón de campos de la física.
- **Química:** Demis Hassabis y John Jumper (DeepMind, hoy de Google) y David Baker, por la **predicción de la estructura tridimensional de las proteínas** con el modelo **AlphaFold**. Una proteína se forma a partir de una cadena de aminoácidos que se pliega como un tallarín en formas que no se podían predecir; se conocía menos del 1% de las estructuras. AlphaFold predijo la forma de más de 200 millones con altísima precisión —en las imágenes, lo verde experimental y lo azul predicho se superponen casi exactos— y eso abre el desarrollo de fármacos y curas a una escala que antes no existía.

> 📌 **Para el parcial, si te preguntan** — *¿Cuál de los modelos de IA es el que utiliza el Deep Learning?*
> Las redes neuronales artificiales (las naturales están en el cerebro). Las redes bayesianas, los árboles de decisión y el gradient boosting son modelos del Machine Learning previo, que trabaja con datos estructurados; las bases vectoriales las usan los LLM. El aprendizaje profundo es, justamente, trabajar con redes neuronales artificiales de múltiples capas sobre datos no estructurados.

> 📌 **Para el parcial, si te preguntan** — *¿Qué diferencia al Machine Learning del Deep Learning?*
> El tipo de dato. Machine Learning aprende de datos estructurados (tablas: filas y columnas con composición conocida) con algoritmos estadísticos; Deep Learning es un subconjunto del Machine Learning que usa redes neuronales artificiales para aprender de datos no estructurados (imagen, video, voz, audio, lenguaje). Entrenar una red es más costoso, así que se usa solo cuando el problema lo exige.

### 2.7 🔴 30 de noviembre de 2022 — ChatGPT

Un día fácil de recordar: en pleno Mundial de Qatar, Argentina le ganó 2 a 0 a Polonia —goles de Mac Allister y Julián Álvarez— y clasificó después de la derrota con Arabia Saudita. Ese mismo día se liberó **ChatGPT**.

Es un **momento bisagra**, quizás más de lo que todavía se percibe. Antes, hacer Machine Learning o redes neuronales requería un *background*: estadística, probabilidad, álgebra, calcular el determinante de una matriz, Python o RStudio — accesible para un ingeniero en sistemas, chino básico para cualquier otra persona. Desde ese día, **cualquiera** tiene en el teléfono algo a lo que le puede pedir cualquier cosa **en lenguaje natural**, sin saber nada, incluso con faltas de ortografía y mal redactado. La IA se metió en las casas.

La velocidad de adopción no tiene precedentes. Tiempo que tardó cada servicio en llegar a **100 millones de usuarios**:

| Servicio | Tiempo |
|---|---|
| Spotify | 11 años |
| Netflix | 10 años |
| Airbnb | 8 años |
| Twitter | 5 años |
| Facebook | 4,5 años |
| Dropbox | 4 años |
| WhatsApp | 3,5 años |
| Instagram | 2,5 años |
| TikTok | 9 meses |
| **ChatGPT** | **2 meses** (y 1 millón en 5 días) |

Veinte veces más rápido que WhatsApp, que hoy nos parece que "todo el mundo lo tiene". Cuatro o cinco veces más rápido que TikTok, que ya era récord. Muchos de esos nombres son los unicornios y productos digitales de las primeras clases; ChatGPT los multiplica a todos.

### 2.8 🔴 2024 — Modelos multimodales

Después de ChatGPT: 2023, la IA generativa; 2024, se masifican los **modelos multimodales** (GPT-4 fue el primero conocido, después vinieron muchos). **Multimodal** significa *múltiples modos*: los modos son las distintas maneras de entrada que las redes neuronales permiten manejar —texto, audio, voz, imagen, video—, y multimodal quiere decir que **pido en un modo y me responde en otro**.

Un detalle de vocabulario antes de los ejemplos: **promptear no es preguntar, es pedir**. *Prompt* viene de *peticionar* —como el prompt de DOS que esperaba un comando—. Puedo preguntar "dame información sobre X", pero también puedo pedir "creame un video", "procesá estos datos".

- Texto → video: "una familia de osos pardos cenando sashimi de salmón con palillos" y sale un video casi cinematográfico (generadores como Sora).
- Video → texto: subo un video y pregunto qué ve; "un oso comiendo sashimi".
- Audio → texto: le doy un tema y me dice de quién es — detecta el patrón.
- Texto → música: "creame un tema a 50 BPM, inspirado en las montañas, para estudiar".
- Video → tablas: "analizá este video y armame una campaña de marketing estructurada en tablas para cargar en mi CRM".

Y las imágenes: desde lo lúdico —un perrito con anteojos y collar de perlas— hasta fotografías realistas donde a simple vista **no se distingue una foto profesional de una generada**. Ahí aparece lo lindo y lo feo.

**Lo feo: deepfakes y fraude.** Un video de Zelensky anunciando la rendición de Ucrania, subido a la propia televisión ucraniana hackeada: tardaron minutos en darse cuenta de que era falso — imaginá el impacto. La demostración del actor Jordan Peele haciendo hablar a Obama con lectura de labios y su voz. Messi hablando inglés perfecto. El primer caso masivo, que ya parece lejano: las fotos del Papa Francisco con una campera blanca de rapero, generadas por alguien que jugaba con la herramienta y se despertó con la polémica mundial encima. Hasta entonces nadie se planteaba que una imagen falsa se podía generar tan fácil; ahora todos sabemos que cualquiera puede.

Y el fraude, concreto y en aumento: fotos de accidentes generadas con IA para estafar a aseguradoras — la misma camioneta, intacta y con el paragolpes destruido; falsos médicos creados con IA vendiendo tratamientos en TikTok e Instagram; las denuncias de estafas habilitadas por IA generativa crecieron más de un 450% en un año según plataformas de reporte de fraude. Y el que ya te puede tocar: un audio o un video **con la voz de un familiar** pidiendo que le transfieras dólares "que después te explico". Manipulación política, incitación a la violencia. Ya no es Photoshop truchando un dibujo.

### 2.9 🔴 2025 — IA agéntica

El último hito, y el que conecta directo con el TP: los **sistemas de acción** de la clase 02 y la propuesta agéntica de la Parte II son esto.

**Un agente** es un programa que puede **percibir su entorno, tomar decisiones y realizar acciones para lograr objetivos específicos**. **IA agéntica** es la que se compone de agentes que aprenden con la experiencia, razonan y planifican estrategias **de manera autónoma**.

La palabra ayuda: *agente* viene de **agencia**, la capacidad de **agenciar** — de resolver cosas, de hacer que pasen. Un **agente de viajes**: le decís "quiero irme a la playa este verano, no más de tanta plata, en tal época" y se encarga del hotel, el avión, el micro. Un **agente de seguros** conoce tus necesidades y consigue el seguro entre varias compañías. El **manager de una banda**: "quiero tocar en los mejores lugares con la gira más optimizada" y él arma el plan. Vos das el objetivo; el agente encuentra el camino.

Lo que lo distingue de un chat: en ChatGPT preguntás, te responde, preguntás, te responde. A un agente lo **configurás** —le decís cuál es el objetivo y qué tiene que hacer— y lo dejás corriendo **en fondo**, como un proceso en segundo plano (un *demonio*), haciendo lo suyo **sin preguntarte ni esperar tu definición en cada paso**: "andá a laburar, ya sabés lo que tenés que hacer, me vas informando los resultados".

Ejemplos, de menor a mayor:

- **Un termostato.** Mira la temperatura; si bajó, activa el calor; si se pasó, lo baja; mantiene la meta. Es un **sistema de control** que se retroalimenta — viene de la electrónica, mucho antes de la IA, y lo van a ver en la materia de control de cuarto nivel (Tecnologías para la Automatización, en el plan K23).
- **Una aspiradora robot.** Objetivo: limpiar el piso. Reconoce el territorio, arma el mapa, esquiva obstáculos, y en teoría trabaja sin necesitar nada de vos.
- **Conducción autónoma.** Le das la dirección, te sentás atrás, y el auto sabe que se está quedando sin combustible y va a cargar, lee semáforos y señales. Parece ficción, pero los taxis autónomos ya operan en ciudades de Estados Unidos; quien viajó en uno lo describe así: "como un auto normal, nada más que nadie maneja; acelera rápido, al principio impresiona".

**En la empresa.** Le doy **metas** a mis agentes: "mantené la satisfacción de mis clientes en tal valor", "mantené la cadena de pagos dentro de estos rangos", "mantené el stock", "lográ un 2% más de rentabilidad en este producto". Se conectan a los distintos sistemas —tienen herramientas, APIs, acceso, *skills*— y hacen lo que tengan que hacer; yo me entero por los reportes y las alertas. Es exactamente el ERP convertido en sistema de acción.

Hablamos de **masificación** en 2025 no porque la idea sea nueva —hace años que se investiga en el MIT y en los laboratorios— sino porque **hoy hay servicios de pago** que cualquier empresa, incluso una pyme, contrata como SaaS por algunos cientos de dólares y tiene un proceso agéntico funcionando en la nube.

### 2.10 🔴 Los cinco componentes de un agente

Lo que distingue a un agente de todo lo anterior, y la grilla con la que se arma la propuesta agéntica del TP:

| # | Componente | La pregunta que responde | Qué es |
|---|---|---|---|
| 1 | **Objetivo** | ¿Qué debo lograr? | Una **meta cuantitativa**, un **KPI** (indicador clave de rendimiento — el número que mide si el objetivo se cumple): más clientes, un porcentaje, dinero, ahorro, tiempo de proceso. |
| 2 | **Modelo de lenguaje** | ¿Cómo entiendo a los humanos? | Un **LLM** atrás, como mínimo, que funciona de **interfaz con el humano** (le puedo promptear en lenguaje natural) y de **orquestador**. Las plataformas empresariales suelen ser **multimodelo**: pueden correr con GPT, Gemini, Claude, el que sea. |
| 3 | **Percibir el entorno** | ¿Qué está pasando? | Los **estímulos**: así como nosotros usamos ojos y oídos, el agente percibe por sus interfaces — APIs a bases de datos, sensores y actuadores, captura de audio, texto, imágenes y video. |
| 4 | **Memoria** | ¿Qué aprendí? | A diferencia del chatbot que cada día arrancaba de cero, el agente **va aprendiendo y mejorando con la experiencia**: memoria de corto, mediano y largo plazo. (Hoy ChatGPT, Gemini o Copilot ya te "conocen" entre sesiones; en un proceso de empresa, obviamente.) |
| 5 | **Tools** | ¿Qué soy capaz de hacer? | Las **herramientas y skills**: si quiero que mi agente de viajes me reserve el pasaje, le tengo que dar conexión a la agencia online y acceso a mi billetera para pagar. Sin tools, el agente sabe pero no puede. |

Dos criterios de diseño que salieron con los componentes:

- **Especialización.** Los agentes funcionan mejor cuanto más específicos: "vos sos el agente que responde sobre el estado del servicio; si te preguntan facturación, pasáselo al agente de facturación".
- **Jerarquía.** Como consecuencia, se arma una especie de **organigrama de agentes** — agentes que orquestan las tareas de otros, un ejército jerárquico. Es la fuerza híbrida de trabajo que quedó abierta en la Parte 2.

### 2.11 🟡 ¿Hasta dónde llegaremos? AGI y singularidad

Muchos analistas, científicos y referentes creen que la IA llegará a resolver todos los problemas del ser humano, dando nacimiento a la **Inteligencia Artificial General (AGI)** o "superinteligencia": una IA que supera a la humana en todos los ámbitos, incluyendo creatividad, adaptación al cambio y resolución de todo tipo de problemas.

Algunos autores, principalmente **Ray Kurzweil** (científico de la computación y futurista), sostienen que hacia **2045** llegaremos a la **singularidad** tecnológica: un punto en que el avance es tan rápido y profundo que transforma radicalmente a la humanidad y vuelve **imposible predecir** cómo será el mundo después. La idea divide a los expertos. La pregunta que deja la cátedra: ¿podrá la IA hacer todas las actividades intelectuales y resolver *todos* los problemas del ser humano?

> 📌 **Para el parcial, si te preguntan** — *¿Qué es un agente de IA y qué lo distingue de un chatbot?*
> Un agente es un programa que percibe su entorno, toma decisiones y realiza acciones para lograr objetivos específicos, de manera autónoma: se lo configura con una meta y trabaja en fondo sin esperar instrucciones en cada paso. Tiene cinco componentes: objetivo (un KPI), modelo de lenguaje, percepción del entorno, memoria y tools. Un chatbot solo responde a lo que se le pregunta, sin memoria ni herramientas para actuar.

---

## 3. 🔴 Cierre: jamás fue tan fácil interactuar con la tecnología

Para cerrar la línea de tiempo, el hilo que la conecta con los ERP de la Parte 1.

Interactuar con GPT o con cualquier modelo es un prompt. No hay que saber SQL para hacer un `SELECT`, ni un comando de Python o de PowerShell. Lenguaje natural — y funciona en cualquier idioma, hasta en cordobés: "che, ¿cómo hago esto?" y responde. Lo que a nivel programación era complejísimo se volvió pedir, y pedir que te lo explique como a un nene de diez años si hace falta.

Hace un par de años nadie se imaginaba eso con un ERP. Un usuario nuevo que entraba a una empresa con SAP tenía **dos meses de capacitación**: "para ver el stock, andá al menú tal, transacción tal" — con su código de letras y números. Hoy la tendencia es la **capa conversacional**: entrar al ERP y decirle "¿qué clientes tenemos que hayan comprado más de tanto?", como si fuera el micrófono de ChatGPT. Interactuamos con los sistemas de gestión, incluso los más complejos, a través de IA conversacional.

Esa es la **tormenta perfecta** de la que se habló en la primera clase: el momento bisagra en que los ERP dejan de ser sistemas de registro y se convierten en sistemas de acción — que es, exactamente, lo que la Parte I del TP tiene que diagnosticar y la Parte II tiene que proponer. La clase 05 retoma ese hilo: cómo se están moviendo hoy los ERP para incorporar todo esto, y cómo hacen las empresas para dar el salto.

Un último aviso de método, para el que quiera hacer doble clic: cada uno de estos temas daría para horas, y la materia lo mira deliberadamente a alto nivel para poder ver todo. Profundizar queda a cuenta de cada uno — y de otras materias de la carrera que lo van a desarrollar.

---

## ✅ Checkpoint — Parte 3

*(Sin respuestas: van al complemento.)*

1. ¿Por qué la cátedra dice que la máquina no "piensa" cuando la ruedita gira, y qué es lo único que sí comparte con los humanos?
2. Explicá la regla "igual o más inteligente" con el ejemplo del millón de casos de fraude. ¿Qué es un modelo sobreentrenado y por qué no empeora?
3. ¿Qué diferencia a un modelo determinístico de uno no determinístico? ¿Por qué un modelo de IA nunca llega a precisión 1?
4. "Si hay un `if`, no es IA." Explicalo con el filtro de spam y con el patrón de fraude multi-país: ¿qué se le dio al modelo y qué no?
5. Describí el Test de Turing y explicá cómo lo conecta la cátedra con la definición "un sistema capaz de aprender".
6. ¿Cómo funciona un sistema experto (hechos, reglas, motor de inferencia) y dónde siguen usándose hoy?
7. ¿Qué es un dato estructurado? Nombrá tres problemas de empresa que se resuelven con Machine Learning y los tres pasos de la metodología.
8. Explicá el perceptrón: entradas, pesos, suma ponderada, función de activación y salida. ¿Qué representa el 0/1?
9. ¿Por qué el Deep Learning es un subconjunto del Machine Learning, y cuándo NO conviene usar redes neuronales?
10. Nombrá los cinco componentes de un agente y explicá, con el agente de viajes, qué pasa si le falta el quinto.
11. ¿Qué significa multimodal, y por qué "promptear" es pedir y no preguntar?

---

## Cierre de la unidad `clase03-04`

Las tres partes cierran así: la **Parte 1** dejó el hilo de ERP listo para retomarlo en la clase 05 (nube, SaaS, tiers, adopción) y la operativa del TP; la **Parte 2** dio el marco de decisión —qué define hoy si una empresa avanza con IA—; y esta **Parte 3** dio la teoría mínima para entender de qué se habla cuando se habla de IA, hasta el agente que la Parte II del TP tiene que proponer.

Lo que queda abierto para las clases siguientes: la continuación de ERP (proyectos de implementación, business case, cómo se están convirtiendo en sistemas de acción), el "Hola Mundo" de Machine Learning con una herramienta no-code, y el bloque de sistemas de ventas, e-commerce y CRM.

---

**FIN DE LA PARTE 3 — Apunte Maestro clase03-04**
