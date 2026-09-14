# 📘 Apunte Maestro — Clases 03-04: Cierre de ERP e introducción a la IA

## Parte 1 de 3 — Cierre del hilo ERP: nube, SaaS, mercado y adopción

> **Unidad:** `clase03-04` — clase 03 (31/8, presencial) y clase 04 (7/9, virtual), unificadas porque la 03 abrió dos hilos —el cierre de ERP y la introducción a la IA— y la 04 los terminó. Se ordenan por tema, no por fecha.
> **Esta parte** cierra lo que la clase 02 dejó abierto sobre sistemas de gestión y captura toda la operativa del TP. Las Partes 2 y 3 son el hilo de inteligencia artificial.
> **Marcas:** 🔴 central-evaluable · 🟡 secundario · 🟢 mencionado al pasar · 🕳️ madriguera (tangente que no hace falta seguir).

---

## 0. 🔴 Información operativa de la unidad

**Propuesta de TP — fecha límite corrida.** La entrega de la propuesta ya no es el 7/9: el límite duro es **antes de la clase 05 (14/9)**, y cuanto antes mejor. Qué se entrega y cómo, en la §1.

**Grupos.** Quedaron **siete grupos**, de cuatro y de cinco integrantes. Se abrió un **foro "TP grupal"** en el aula virtual: cada grupo ve solo su hilo, las respuestas quedan registradas para todos los integrantes y llegan como alerta. Las consultas del TP van por ahí, **no por mail** — el mail se acepta, pero rompe el hilo compartido.

**Clase 05 (14/9).** Virtual, en horario normal, con el docente conectado desde el exterior. Probabilidad declarada del 90%; si se complicaba por fuerza mayor, el aviso llegaba el domingo a más tardar. Si no hubo aviso, hay clase. El plan tiene una clase de margen, así que una suspensión no recorta temario.

**Trivia también en las presenciales.** No es solo para las virtuales: en las clases presenciales también se juega, y funciona como doble chance —participación y puntualidad a la vez—. Reglas prácticas: **una sola cuenta por persona** (no vale entrar dos veces como en el bingo con varios cartones), y **siempre el mismo nombre y apellido** en Quizizz, porque la tabla de posiciones se arma cruzando ese alias con el registro del curso; si cambiás de nombre entre fechas, el cruce hay que hacerlo a mano.

**Cambio de orden del calendario.** La clase 04 no fue "Subsistema de Ventas": se usó para cerrar el quiz y dar completa la introducción a la IA. El orden original se recupera en la clase 05: primero lo que quedó de ERP (cómo es un proyecto de implementación, cómo se están moviendo los ERP para incorporar IA) y después ventas, e-commerce y CRM. Además vienen lunes sin clase (21/9 y 12/10), así que el cuatrimestre se acorta rápido.

**🟢 Antecedente de la materia.** Esta materia es la misma que antes se llamaba *Sistemas aplicados a la gestión empresarial* (y antes, *Sistemas integrados de gestión*): cambió el nombre y se renovó buena parte del contenido, pero no es una segunda parte ni una continuación. Quien haya cursado la versión anterior debería consultar en el departamento si el sistema la cuenta como otra electiva.

---

## 1. 🔴 El TP integrador, explicado en detalle

Esto amplía lo que ya conocés del enunciado: acá está el **criterio** con el que se va a validar tu caso y corregir tu entrega.

### 1.1 Las dos fotos

El TP tiene dos partes y son dos fotos distintas de la misma empresa:

| | Parte I | Parte II |
|---|---|---|
| **Qué es** | La **foto actual**: diagnóstico | La **foto futura**: propuesta |
| **Pregunta central** | ¿Qué usan hoy, cómo llegaron hasta acá, dónde aprieta el zapato? | Si me contratan como consultora, ¿qué le propongo para modernizar e innovar? |
| **Naturaleza** | Investigación: no hay mucho que inventar ni discutir, es relevar | "Ficción" en el sentido de **propuesta**: nadie va a verificar si la empresa la compraría o cuánto costaría |
| **Se apoya en** | Las clases sobre sistemas de gestión (el primer bloque de la cursada) | Las clases de transformación e IA (el segundo bloque) |

Las dos partes van **en paralelo con la cursada**: la primera entrega coincide con el fin del bloque de sistemas de gestión, la segunda con el fin del bloque de IA. Muchos términos de la consigna que hoy no están claros se van a ir dando clase a clase — no es motivo para frenar la elección del caso.

**La Parte II depende de la Parte I.** Si el diagnóstico dice que todo funciona perfecto y la empresa no necesita nada, no hay a quién venderle transformación digital. Los *pain points* (puntos de dolor: dónde el sistema actual falla, queda chico o frena al negocio) que encuentres en la Parte I son exactamente las oportunidades sobre las que se construye la Parte II. Ejemplos típicos de lo que aparece: "el sistema a medida servía para 1.000 empleados y ahora son 3.000", "la empresa empezó a exportar y el sistema no lo soporta", "funcionó bien diez años pero no tiene nada de IA ni de productos digitales para dar el próximo paso".

> 💡 Hubo un caso en cursadas anteriores de un grupo que hizo el TP sobre una empresa familiar del interior y, terminado, se lo presentó de verdad al director financiero de la empresa. La Parte II es propuesta, no ejercicio de fantasía.

### 1.2 "Alto nivel, siempre"

Es la instrucción más repetida de toda la unidad. Nada de esto va en el TP:

- Acceder a la base de datos, ver datos reales, ver logs.
- Arquitectura: qué motor de base de datos, qué versión, cuántos nodos, si es una granja de servidores.
- Programación de ningún tipo.

Lo que sí va, y en la dosis justa: **el stack tecnológico en dos párrafos y un gráfico simple**. Del estilo "tienen tal sistema en la nube con tal proveedor" o "lo tienen instalado en servidores propios", "los usuarios entran por un portal en React y atrás corre tal ERP". Suficiente para entender la foto; cualquier detalle más es sobrecarga que no se evalúa.

### 1.3 Empresa entera o un área

El enunciado dice "una empresa o el área de una empresa". El criterio para elegir es el tamaño:

- **Pyme, startup, emprendimiento:** se puede abarcar **completa**, porque un análisis de alto nivel cubre toda la empresa sin esfuerzo — típicamente hay un solo sistema de gestión (facturación, ventas, compras, algún proceso de RRHH) que maneja una persona o un equipo chico para toda la organización.
- **Empresa grande** (un banco, una petrolera, una automotriz, un marketplace): abarcarla entera sería gigantesco —cientos o miles de procesos—. Se toma **un área o un proceso**: control de calidad en la línea de montaje, compras a autopartistas, la red de distribución. Un solo proceso de un área grande termina siendo tan complejo como una pyme entera.

Cada grupo tiene libertad, con el único criterio de que el recorte cumpla el objetivo del trabajo.

### 1.4 Cómo se consigue la información

Tres caminos, todos válidos:

1. **Un integrante trabaja (o trabajó) ahí** y accede a la información directamente. Es el caso más común.
2. **Un conocido** (familiar, amigo, ex compañero) que trabaja en la empresa: se le hace una entrevista breve, por mail o por WhatsApp, con una guía de preguntas. Tipo encuesta, dedicándole un rato.
3. **El caso es público** y la información se consigue por fuentes abiertas.

La empresa se puede **anonimizar**: "una pyme de la industria textil que comercializa en Argentina" con nombre ficticio es perfectamente aceptable si no se quiere exponer el caso real.

### 1.5 La guía de preguntas del diagnóstico

Lo que hay que averiguar, en el orden en que conviene preguntarlo:

1. **Sistemas principales** que usan y **desde cuándo** — ¿es una implementación reciente o la tienen hace muchos años?
2. **Por qué eligieron eso.** ¿Fue una decisión propia por costo, porque se adaptaba a los procesos, porque alguien lo recomendó? ¿O es una empresa global y la casa matriz impuso el sistema?
3. **Qué opciones evaluaron.** Poner SAP, poner algo local, o desarrollar a medida (ver §2).
4. **Cómo fue la implementación.** Acá hay dos extremos: "salió andando, casi sin retoques" o "estaba previsto para seis meses y llevó tres años, hubo que cambiar todo, nadie se ponía de acuerdo". La pregunta concreta es *qué tan doloroso fue el proyecto*. Y si el sistema fue natural para el negocio o hubo que **adaptarlo mucho**.
5. **Dónde aprieta el zapato.** Los pain points, ya sea porque la empresa los cuenta o porque el grupo los detecta analizando.

### 1.6 El filtro: si vive en un Excel, no sirve

Además de los filtros del enunciado (sistema integrado con el core del negocio, la contabilidad o una base centralizada; sin silos ni bases aisladas), hay uno explícito y frecuente: **una empresa que lleva la gestión en planillas de Excel queda descartada**. No porque lo que hace esa empresa no sea valioso, sino porque no hay ningún sistema de gestión que analizar — y el TP es sobre eso.

### 1.7 La propuesta: qué se entrega ahora

La "propuesta de TP" es **un párrafo** por grupo, subido en el espacio *subir propuestas* del aula virtual (o por mail, pero en el aula queda registrado que se cumplió). El objetivo es que el docente **valide** el caso: no hay casos buenos o malos, la validación sirve para confirmar que con ese caso se va a poder ver lo que el trabajo necesita.

Qué tiene que decir el párrafo:

- Qué empresa (o qué tipo de empresa, si es anónima) y qué proceso o área.
- Cómo van a conseguir la información (integrante, conocido a entrevistar, caso público).
- Lineamientos básicos de lo que ya saben: "usa Tango para la gestión y además vende por e-commerce con una integración con Shopify / Magento / Mercado Libre".

**Si el grupo no está seguro, presentar dos o tres opciones** —plan B, plan C— y el docente recomienda cuál conviene tomar según lo que se va a ver en la cursada. Si el caso ya está firme, se describe, se recibe el OK y se arranca.

### 1.8 La primera entrega es un checkpoint

La entrega de la Parte I no es un examen parcial ni tiene recuperatorio. Es un **checkpoint**: se recibe devolución, y lo que esté flojo o mal encaminado se corrige **para la entrega final**. La idea es ir tanteando para llegar bien al final, no evaluar dos veces.

> 📌 **Para el parcial, si te preguntan** — *¿Qué caso NO sirve para el TP, aunque la empresa sea importante?*
> Un caso donde no haya un sistema de gestión integrado con el core del negocio, la contabilidad o una base centralizada: gestión en Excel, aplicativos aislados para una sola tarea, o bases sin trazabilidad. Tampoco sirve un recorte demasiado grande (una corporación entera) ni demasiado chico (un área minúscula). El TP analiza un sistema de gestión sobre un proceso *core*, a alto nivel.

---

## 2. 🟡 Comprar o desarrollar a medida

Esta es una de las preguntas del diagnóstico (§1.5, punto 3), y merece su propio criterio porque aparece en casi todos los casos.

### El caso: un fabricante de satélites

Pensá en una empresa que fabrica satélites. ¿Cuántos ERP hay en el mercado especializados en fabricar satélites? Probablemente ninguno. Sus procesos no se parecen a los de ninguna otra empresa —la contabilidad quizás sí, pero el resto es tan particular que un sistema generalista adaptado a fuerza terminaría deformado—. Ahí **sí** tiene sentido invertir en desarrollar un sistema de gestión propio. Y hay un plus: si después se lo puede vender a otro fabricante de satélites del mundo, la inversión se convierte en un **producto**.

### El criterio general

Ese caso es la excepción. La regla, y es lo que te va a decir cualquier vendedor de ERP, es que **desarrollar a medida es reinventar la rueda**:

- La contabilidad, la liquidación de sueldos, la facturación son procesos **estándar**, iguales para todas las empresas, resueltos hace décadas. No hay nada que inventar.
- La intuición de "es más barato hacerlo nosotros que pagar un producto caro" falla cuando se suman **horas de desarrollo, inversión, tiempo de esas personas y riesgo**: termina siendo mucho más caro.
- Por eso hoy es **raro** que una empresa se mande a desarrollar su sistema de gestión. Cuando pasa, es por procesos de **nicho** que ningún producto cubre.

> 📌 **Para el parcial, si te preguntan** — *¿Cuándo tiene sentido desarrollar un sistema de gestión a medida?*
> Solo cuando el negocio tiene procesos de nicho tan particulares que un ERP generalista quedaría deformado al adaptarlo. Para procesos estándar (contabilidad, sueldos, facturación) desarrollar a medida es reinventar la rueda y, sumando horas, inversión y riesgo, sale más caro que comprar.

---

## 3. 🔴 On-premise, nube y SaaS: tres cosas distintas

En la clase 02 quedó plantado que el mercado pasó del on-premise a la nube y que hoy el ERP se contrata como SaaS. Acá se abre esa idea, porque encierra una trampa que la trivia ya explotó: **"estar en la nube" y "ser SaaS" no son lo mismo.**

### 3.1 El caso: el Cyber Monday con el sitio caído

Años atrás era casi una tradición: llegaba el Cyber Monday (o el Black Friday en Estados Unidos), un día de promociones masivas, y a media mañana el sitio de e-commerce tiraba error. La explicación de la empresa: "no esperábamos tanta visita". Pensalo un segundo: invertiste en publicidad para que **todo el mundo** entre el mismo día, y no te preparaste para recibir el triple de tráfico. Era un error de planificación, pero también era un límite técnico real: con la infraestructura de entonces, agrandar la capacidad para un solo día era imposible.

Hoy esa misma empresa entra la noche anterior a la consola de su proveedor de nube y dice "triplicá la capacidad de esto por 24 horas". Si paga mil dólares por mes, ese día le cuesta quinientos extra; terminada la promoción, vuelve al tamaño original. Esa diferencia es el tema de esta sección.

### 3.2 On-premise: la instalación propia

**On-premise** (*en las instalaciones*; a veces se dice "on-prem") es tener el sistema instalado en **servidores propios**: comprar el hardware, armar el data center y administrar todo. La empresa es dueña de la instalación: compra la licencia del ERP, la configura como quiere y la corre en su propia infraestructura.

Hace años era la única opción. Hoy es **muy raro** que una empresa nueva arme su propio data center. Las que siguen on-premise lo hacen por razones puntuales: **temas regulatorios** (ciertos bancos, un banco central) o de seguridad en casos específicos.

### 3.3 La nube y los hiperescaladores

Un **hiperescalador** es un proveedor de nube de escala mundial: data centers propios distribuidos en todos los continentes, capacidad prácticamente ilimitada y cumplimiento de los estándares regulatorios y de seguridad más exigentes de cada país. Para empresas en Argentina y Latinoamérica son tres: **Google Cloud, Microsoft Azure y Amazon AWS**. No son los únicos —en Asia, por ejemplo, Alibaba también es proveedor de nube; y acá hay telcos que dan servicios de nube a clientes chicos—, pero son los tres que compiten por las empresas.

Los tres son **world class** (*de clase mundial*, nivel *enterprise*): preparados para cumplir los estándares legales y de seguridad de todos los países, al punto de que gobiernos, empresas de defensa y bancos corren sobre ellos. Cada uno vende sus argumentos —Google, por ejemplo, la resiliencia de sus data centers duplicados bajo tierra en todos los continentes—, pero a efectos prácticos son un **commodity**: los tres son equivalentes.

Y acá aparece algo que en la clase 02 no estaba: **la implementación de un ERP es una triple competencia**.

```
      ¿QUÉ ERP?                  ¿QUIÉN LO IMPLEMENTA?              ¿DÓNDE CORRE?
 ┌───────────────────┐      ┌──────────────────────────┐      ┌────────────────────────┐
 │ SAP · Oracle ·    │      │ Partners implementadores  │      │ Azure · AWS · Google   │
 │ Dynamics · …      │ ───▶ │ (Accenture, KPMG,         │ ───▶ │ Cloud                  │
 │                   │      │  consultoras de nicho)    │      │                        │
 └───────────────────┘      └──────────────────────────┘      └────────────────────────┘
   compiten entre sí           compiten entre sí                compiten entre sí
                                                                 "¿Ya elegiste SAP?
                                                                  Ponelo en MI nube:
                                                                  te bonifico X, te
                                                                  regalo Y por un año"
```

Cuando una empresa decide "vamos a implementar SAP", detrás del fabricante y del partner implementador se meten Amazon, Google y Microsoft a competir por dónde va a correr esa instalación: "si lo hacés en mi nube tengo tal costo y te bonifico tal cosa", "si lo ponés en Azure te doy Office 365, Copilot y Power Automate gratis por un año". Los partners implementadores se explican en la §5.

### 3.4 La ventaja real: flexibilidad y escalabilidad

Volvé al Cyber Monday. Con una implementación on-premise que **quedó chica** —la empresa creció, compró otra, se multiplicó por cinco— hacer un *upgrade* significa salir a comprar hardware de nuevo: servidores, memoria, base de datos, y casi rehacer la instalación. Costosísimo. En la nube es entrar a la consola de administración y decirle a la máquina virtual "duplicá la memoria", "agregale alta disponibilidad", "aumentá la concurrencia": **unos clics, segundos**. Y al revés también: si la demanda baja, se achica y se paga menos.

Esa es la ventaja principal de implementar en la nube, y es la respuesta que espera la cátedra: **flexibilidad y escalabilidad** respecto del on-premise.

Lo que **no** es la ventaja, aunque suene intuitivo: que la nube "siempre es más barata". Amazon no es barato; ninguno de los tres lo es. Lo que decide es el **caso de negocio**: cuando ponés en la balanza el hardware, el mantenimiento, la administración y el riesgo, a cierta escala la nube conviene. Pero hay un caso donde no: la empresa que ya tiene hardware comprado hace unos años, que todavía sirve y está amortizado. Ese hardware es un **costo hundido** (ya lo pagaste, no lo recuperás decidas lo que decidas): implementar ahí tiene costo cercano a cero, mientras que la nube sí cobra. Así que "siempre más barato" es falso.

### 3.5 Por qué las empresas se resistían a la nube (y por qué cambió)

El cambio masivo a la nube tiene apenas unos diez años, y al principio la resistencia fue fuerte. Tres argumentos, y cómo se dieron vuelta:

**Seguridad.** "No voy a poner toda mi información confidencial en la nube, ¿qué pasa si la roban?". La respuesta de los hiperescaladores: cumplimos todos los estándares — y tu instalación on-premise también está expuesta: un empleado infiel puede entrar a la noche y romper todo, como en las películas.

**Catástrofes.** Una empresa de agroquímicos de Pergamino tenía su data center armado en la planta. Vino una inundación grande y el data center quedó **literalmente bajo el agua**: una semana entera sin poder operar. Una inundación, un terremoto, un incendio — cualquier catástrofe natural. Los sistemas en la nube están distribuidos en múltiples nodos: si uno cae, se prende el otro.

**Política y jurisdicción.** Cuando la migración a la nube empezó a masificarse en Argentina, coincidió con la **estatización de las AFJP** (las administradoras privadas de jubilaciones, reestatizadas en 2008). Esas administradoras tenían acciones en muchas empresas grandes, y al pasar al Estado, el Estado pasó a poner directores en esas empresas. El razonamiento de muchas compañías fue: "si mis datos están en la nube, en algún momento el Estado, con el que tengo un conflicto de intereses, va a poder acceder a ellos". Y la vuelta de tuerca: si un juez argentino ordena que ciertos datos sean accesibles y el servidor está físicamente en Estados Unidos, el juez no puede pedirlos. La nube era, para algunos, una forma de quedar fuera de alcance; para otros, un riesgo de quedar demasiado a mano.

Hoy la percepción se invirtió: se considera **más seguro** tener los datos en una nube privada de uno de los tres grandes que administrar el control propio. El grueso de las empresas ya está ahí; las excepciones son regulatorias.

### 3.6 SaaS es un modelo de servicio, no una tecnología

Acá está la distinción que confunde. Tener el ERP "en la nube" es una decisión **tecnológica**: dónde corre. **SaaS** (*Software as a Service*, software como servicio) es una decisión **comercial**: qué comprás.

Para implementar SAP —o cualquier ERP— hay dos caminos:

```
 ¿CÓMO ADQUIERO EL ERP?
 │
 ├── LICENCIA + IMPLEMENTACIÓN PROPIA
 │     Compro licencias. La instalación es MÍA: yo la configuro, yo me encargo
 │     del backup, los parches, las actualizaciones, si se llena el disco.
 │     ├── on-premise: en mis servidores
 │     └── en la nube de un hiperescalador → "nube privada": sigue siendo mi instalación,
 │                                            solo cambió dónde corre
 │
 └── SUSCRIPCIÓN — SaaS
       No compro licencias: compro un SERVICIO. Pago una suscripción mensual
       (por usuario, por sociedad, según el proveedor) y el proveedor se encarga
       de TODO lo de atrás. → "nube pública".
```

El argumento de venta del SaaS es: "vos te dedicás a fabricar; olvidate de administrar el sistema, yo lo hago". El proveedor —una consultora, o directamente el fabricante— se encarga de la nube, el **backup**, el ***disaster recovery*** (recuperación ante desastres: que el sistema vuelva a funcionar después de una caída grave), el hardware, el disco, los **parches** (correcciones de software) y las **actualizaciones**. Se paga, por ejemplo, cien dólares por usuario por mes, y todo eso viene incluido.

La analogía es Netflix: no comprás una licencia de algo que tenés que instalar y mantener; pagás una suscripción, la cancelás cuando querés, y mientras tanto el catálogo se actualiza y sigue siendo compatible con los dispositivos nuevos sin que hagas nada.

**Quién usa cada modelo.** Las grandes empresas, por sus características, suelen necesitar **implementación propia** (aunque corra en la nube). Del segmento medio para abajo, la tendencia es fuerte hacia **SaaS**: un valor fijo por mes y nada que administrar. Y la tendencia general del mercado apunta hacia ahí.

> 🕳️ **Madriguera — IaaS y PaaS**
> SaaS tiene dos hermanos que aparecen como distractores: **IaaS** (*Infrastructure as a Service*: alquilás servidores virtuales, disco y red, y vos instalás todo encima — la "implementación propia en la nube" de arriba es esto) y **PaaS** (*Platform as a Service*: alquilás una plataforma lista para desplegar aplicaciones sin administrar servidores). La materia solo usa SaaS.
> *Volvé al camino — esto se profundiza aparte, otro día.*

### 3.7 La regla del "siempre"

Una regla de examen que vale para toda la cursada: en una pregunta de opción múltiple, **toda opción que empiece con "siempre" es falsa**. Como viste en Lógica, "siempre" es una tautología —tiene que valer en todos los casos— y en la realidad siempre hay una excepción. "La nube es siempre más barata": falsa (§3.4). "Un modelo predictivo asegura la rentabilidad": falsa, porque ningún modelo de inteligencia artificial llega a precisión 1 — ni el que desbloquea tu teléfono con la huella (99,99%), ni el piloto automático de un avión, ni el robot de una cirugía; si fuera 1, no sería inteligencia artificial, sería un algoritmo determinístico. Eso se desarrolla en la Parte 3. Las promesas de "10% de ganancia en dólares asegurada" de los cursos de trading son la versión callejera del mismo error.

> 📌 **Para el parcial, si te preguntan** — *¿Cuál es la principal ventaja de implementar un sistema de gestión en la nube?*
> Flexibilidad y escalabilidad respecto del on-premise: la capacidad se agranda o se achica en minutos desde la consola del proveedor, sin comprar hardware ni rehacer la instalación. No es "siempre más barato": a cierta escala conviene, pero una empresa con hardware amortizado (costo hundido) puede implementar on-premise a costo cercano a cero.

> 📌 **Para el parcial, si te preguntan** — *¿Qué diferencia hay entre tener un ERP en la nube y contratarlo como SaaS?*
> Estar en la nube es una decisión tecnológica (dónde corre); SaaS es un modelo de servicio (qué se compra). Con licencia e implementación propia, la instalación es de la empresa y ella la administra, corra on-premise o en la nube de un hiperescalador. Con SaaS no se compran licencias sino una suscripción por usuario o por sociedad, y el proveedor se encarga de la infraestructura, el backup, el disaster recovery, los parches y las actualizaciones, como Netflix.

**🟡 Lo que la trivia dio por sabido de la clase 02.** Las otras preguntas de la fecha 2 recortaron tres ideas de la clase anterior, que conviene tener frescas en una línea cada una: la función principal de los **systems of action** es representar el estado actual en tiempo real y tomar decisiones autónomas a partir de IA (a diferencia de registrar datos históricos o facilitar la interacción); la característica que consiste en conocer todo el ciclo de vida de un dato o documento es la **trazabilidad**; y la consecuencia directa de los **silos** es que los problemas suben hasta la dirección y después tienen que volver a bajar, con costos extra de control.

---

## 4. 🔴 El mapa del mercado ERP: tres tiers

En la clase 01 apareció la tabla de los *tiers* como un mapa para reconocer nombres. Acá se le pone criterio: **qué define que un ERP esté en cada capa**, y por qué eso importa para elegir.

```
              ┌───────────────┐
              │    TIER 1     │  SAP · Oracle · Microsoft Dynamics
              │  world class  │  Alcance global. Localizados para casi todos los
              ├───────────────┤  países. Los más complejos y costosos de implementar.
              │    TIER 2     │  Totvs · Epicor · Infor · …
              │  segmento     │  Grandes, pero sin alcance tan global, o enfocados
              │  medio        │  en ciertos segmentos o regiones.
              ├───────────────┤
              │    TIER 3     │  Tango · Buenos Aires Software · Softland ·
              │  local /      │  Bejerman · Calipso · Odoo · …
              │  pymes        │  Creados localmente, orientados a pymes.
              └───────────────┘  En cada país son otros.
```

**Tier** (*capa*, en inglés) es simplemente el nombre de cada nivel.

### 4.1 Tier 1 — world class: el secreto está en la localización

Los tres grandes, para las empresas más grandes del mundo y las multinacionales:

- **SAP**, el líder. Según la propia empresa, la gran mayoría de las **Fortune 500** (el ranking de las 500 empresas más grandes de Estados Unidos) usa SAP.
- **Oracle**, que fue comprando los productos que le seguían a SAP y los unificó en su suite.
- **Microsoft Dynamics**, más presente en el segmento no tan grande pero considerado world class: presencia en todo el mundo, todos los idiomas. La mayoría lo conoce por su **CRM**, pero Dynamics es también ERP, heredero de productos que Microsoft fue adquiriendo (Great Plains entre ellos).

Qué significa **world class** para un ERP, y por qué es más que "grande": estos sistemas están **localizados** para casi todos los países del mundo. Localización no es solo idioma y moneda —aunque también: SAP corre en chino, en japonés con pictogramas, en ruso—. Es **procesos y legislación local**: qué normas aplican, cómo son las retenciones y percepciones de impuestos, cómo se es agente de retención, cómo se emiten y validan facturas ante **ARCA** (el organismo recaudador argentino, ex AFIP). Todo eso viene preparado para cada país. Ese alcance global es exactamente lo que los hace **los más complejos de implementar y los más costosos**.

### 4.2 Tier 2 — el segmento medio

Empresas grandes, pero sin el alcance global de las tres de arriba, o enfocadas en ciertos segmentos o regiones. Algunos nombres:

- **Totvs**, brasileño — el único de origen latinoamericano de esta capa para arriba, bastante usado en todo el mundo.
- **Epicor**, muy usado en Estados Unidos y Canadá.
- **Infor**, presente en la Fórmula 1 (Ferrari).

Hay muchos más; en los casos del TP van a aparecer otros.

### 4.3 Tier 3 — local, orientado a pymes

Los creados localmente y orientados a pymes. En Argentina: **Tango** (probablemente el ERP argentino más conocido, usado por muchas pymes y no tan pymes; creció con clientes en Uruguay y Paraguay), **Buenos Aires Software (BAS)**, **Softland**, **Sistemas Bejerman** (incluso con soluciones para estudios jurídicos y contables), **Calipso**, y **Odoo**, que es **open source** (código abierto: el software se puede usar y modificar libremente, sin licencia propietaria) y se usa cada vez más. Si nos vamos a Brasil o a otro país, la lista es otra.

### 4.4 El caso: el sistema que quedó chico

Una empresa que gestiona la administración y recaudación de barrios privados, dentro de un grupo grande de real estate. Compró **Buenos Aires Software** cuando era chica. Hoy administra alrededor de **noventa sociedades** y mueve, en facturación, algo comparable a una ciudad. Y BAS tiene un límite técnico: el identificador de sociedad es de **dos dígitos**. Solución de emergencia: **dos bases de datos**. Consecuencia: **duplicidad de datos, sin trazabilidad** — exactamente el silo que un ERP existe para evitar. Están mirando migrar a Dynamics.

Es un caso de manual para la Parte I del TP, y muestra un patrón que se repite: se compra un sistema pensado para cierto tamaño, el negocio crece y el sistema **no acompaña el ritmo**. Es un *happy problem* —el problema de crecer, mejor que el inverso: comprar algo grande y tener que achicarse—, pero un problema al fin: en algún momento el sistema empieza a traer más problemas que soluciones.

> 📌 **Para el parcial, si te preguntan** — *¿Qué hace "world class" a un ERP de Tier 1, y por qué son los más caros?*
> Alcance global: están localizados para casi todos los países, no solo en idioma y moneda sino en procesos y legislación (normas, retenciones, facturación ante el organismo recaudador local). Esa cobertura los vuelve los más complejos de implementar y, por eso, los más costosos.

---

## 5. 🔴 Adopción: comprar tecnología no es usarla

Esta idea apareció en la clase 01 y vuelve con fuerza porque explica **cómo funciona el negocio** de los ERP y de la IA, y por qué tanto proyecto termina en nada.

### 5.1 El caso: SAP con un solo módulo

Una empresa compra SAP. Gasta una fortuna en licencias. Dos años después está usando **un solo módulo**: contabilidad. ¿Y BTP (la plataforma tecnológica de SAP para integraciones, extensiones e IA), todo lo demás que pagó? Nada. Un día viene Oracle con una buena propuesta y la empresa piensa: "lo que tenemos en marcha es poco, migrarlo es fácil". Y se va.

Ahora la versión contraria: el proveedor logra que la empresa **le saque el jugo** a todo. Contabilidad, ventas, compras, RRHH, la parte analítica, la IA. Si mañana quiere irse a otro, tiene que rehacer todo lo que funciona bien: la migración cuesta el doble, o más. No es "rehén", pero está muy cerca.

### 5.2 Qué es adopción y por qué le importa al proveedor

**Adoptar** una tecnología es **usarla de verdad**, sacarle el jugo, no tenerla ociosa como un armatoste. Y ese es el objetivo real del proveedor, por dos razones:

1. **Barreras de salida.** Cuanto más se usa el sistema, más caro es irse. Un cliente que solo usa contabilidad tiene barreras de salida bajas; uno que corre toda la operación encima, altísimas.
2. **Caso de negocio.** Sin adopción no hay valor. Gastar en tecnología porque está de moda —"ante los accionistas tenemos que mostrar que estamos en IA"— y después seguir haciendo el mismo proceso con los mismos problemas no tiene sentido. Lo que está de moda tiene que tener un **caso de negocio** detrás.

Y adopción es difícil. Implementar cada cosa, que el usuario se acostumbre, encontrar el caso donde tiene sentido: es tiempo, y suele ser más trabajo del implementador que del fabricante.

### 5.3 El ecosistema: fabricante, partner y comisión

El fabricante —SAP, Oracle, Microsoft— **vende la licencia**. Mientras el cliente la paga, está contento. Quien tiene que lograr la adopción es otro: el **partner implementador** (o simplemente *partner*). Son las consultoras —Accenture, KPMG, las grandes; y las de nicho, más chicas y enfocadas— que integran la **red de partners** del fabricante: el canal oficial, autorizado a vender licencias y dar servicio, como las **concesionarias oficiales** de una marca de autos.

Cómo se sostiene: el partner cobra una **comisión** (un *fee*) cuando vende licencias como intermediario, y a cambio se espera que agregue valor: convencer al cliente, mostrarle la **hoja de ruta** de todo lo que podría usar, empujar la adopción de toda la suite. De ahí la tensión permanente entre fabricante y partner: "ya le vendimos la licencia a este cliente — ¿por qué no le estás quemando la cabeza con todo lo nuevo que podría usar, la inteligencia artificial, lo que sea?".

Eso explica el negocio de las consultoras con SAP, y también la triple competencia de la §3.3: fabricante, partner y proveedor de nube son tres actores distintos que cobran por separado.

### 5.4 Lo que ya pagaste y no usás: Power Automate

Un ejemplo de adopción en chiquito. **Power Automate** es la herramienta de automatización de Microsoft; viene incluida en las licencias de Microsoft 365, que tienen prácticamente todas las empresas, y casi ninguna la explota. Cuando una empresa dice "necesitamos comprar una herramienta de automatización", la respuesta de Microsoft es "¿qué vas a comprar, si ya tenés esto y no lo estás usando?". Para lo básico anda bien. Cuando se complica —conectores *premium* que exigen otra licencia— la pyme empieza a hacer trucos para esquivar el costo y ahí se vuelve tosco. Es un caso pequeño del mismo patrón: la tecnología está comprada; lo que falta es adopción.

> 📌 **Para el parcial, si te preguntan** — *¿Qué es la adopción de una tecnología y por qué es el objetivo del proveedor?*
> Adopción es usar de verdad lo que se compró: implementar los módulos, que los usuarios los usen, sacarle el jugo. Al proveedor le importa porque la adopción profunda levanta las barreras de salida —irse a un competidor cuesta el doble— y porque sin adopción no hay caso de negocio: se gastó por moda y se sigue con los mismos procesos y los mismos problemas.

---

## 6. 🟡 RPA: el auge que se desinfló, y la lección para la IA

**RPA** (*Robotic Process Automation*, automatización robótica de procesos) es software que automatiza tareas repetitivas imitando lo que haría una persona frente a la pantalla: abrir un mail, bajar un adjunto, subirlo a una carpeta, copiar datos de un formulario a otro.

### 6.1 El boom

Hace unos años fue el gran tema: robotizar, automatizar procesos. Tres plataformas lideraban: **Blue Prism** (británica), **UiPath** (de origen rumano, hoy en Estados Unidos) y **Automation Anywhere**. Power Automate de Microsoft llegó después, más simple. Las empresas compraban plataformas de **miles de dólares**.

### 6.2 Qué salió mal

Dos cosas, y las dos se repiten hoy con la IA.

**Matar una mosca con un cañón.** Los casos de negocio eran simplones: "recibo un mail con un adjunto y lo tengo que subir a este drive". Para eso, una plataforma de miles de dólares que una persona resuelve en dos segundos. Las plataformas estaban pensadas para cosas muchísimo más complejas, y la mayoría no entendía bien para qué las estaba implementando.

**Automatizar procesos que no estaban definidos.** Este es el problema de fondo. Cuando se iba a relevar el proceso con el usuario, la conversación era así: "cuando llega una factura, si es de un cliente de Bahía Blanca hay ingresos brutos con convenio multilateral, entonces pregunto… ah, pero si viene de Carlos tengo un arreglo, y si viene de Juan abro un Excel…". Miles de excepciones, atajos artesanales, arreglos personales. Volcar eso a una automatización daba un desastre, porque **los procesos no eran determinísticos**: no se podían plasmar en una regla.

Un proceso automatizable es uno que se puede escribir como un flujo cerrado: llega una factura → si es de responsable inscripto, hacer esto; si no, aquello → esperar la autorización del director → cuando llega la segunda firma, disparar. Claro, sin excepciones sueltas. Si el proceso real es "depende", no hay nada que automatizar todavía.

El resultado fue mucha desilusión, muchos proyectos fracasados, y esas empresas de RPA hoy reconvertidas hacia IA. El RPA todavía existe, montado sobre la IA, pero los grandes proyectos de robotización ya no se ven.

### 6.3 La lección que se traslada a la IA

Es la misma lección, y va a volver en la Parte 3:

- **Automatizar sobre el caos maximiza el caos.** Poner IA o automatización encima de un proceso que abajo está desordenado no ordena nada: amplifica el desorden.
- **Los modelos se alimentan de datos.** Un modelo predictivo entrenado con datos **duplicados, inconsistentes, incompletos** genera un monstruo que va a andar mal. La calidad de lo que sale depende de la calidad de lo que entra.

> 📌 **Para el parcial, si te preguntan** — *¿Por qué fracasaron muchos proyectos de RPA, y qué tiene eso que ver con la IA?*
> Porque se compraron plataformas caras para casos triviales, y sobre todo porque se intentó automatizar procesos que no estaban definidos: llenos de excepciones y atajos artesanales, no determinísticos, imposibles de plasmar en reglas. Con la IA pasa lo mismo: automatizar o entrenar modelos sobre procesos caóticos y datos inconsistentes maximiza el caos en lugar de resolverlo.

---

## ✅ Checkpoint — Parte 1

*(Sin respuestas: van al complemento.)*

1. Una pyme importante lleva toda su gestión en planillas de Excel. ¿Por qué queda descartada como caso de TP, aunque el negocio sea interesante?
2. Un grupo eligió un banco como caso. ¿Qué tiene que hacer con ese caso para que sea abarcable, y por qué?
3. Explicá la diferencia entre "implementar el ERP en la nube" y "contratar el ERP como SaaS" usando el mismo ERP en los dos ejemplos.
4. "La nube es siempre más barata que el on-premise." Explicá por qué es falso y qué es un costo hundido.
5. ¿Por qué una empresa argentina, alrededor de 2010, podía rechazar la nube por motivos políticos y no técnicos?
6. ¿Qué es la localización de un ERP, y qué relación tiene con que los Tier 1 sean los más caros de implementar?
7. En el caso de la empresa de barrios privados, ¿cuál fue la señal técnica concreta de que el sistema había quedado chico, y qué consecuencia tuvo sobre los datos?
8. ¿Por qué a SAP le conviene que un cliente use todos los módulos y no solo contabilidad? Nombrá los dos motivos.
9. ¿De qué vive un partner implementador y qué se espera que aporte a cambio?
10. ¿Qué tienen en común un proyecto de RPA sobre un proceso lleno de excepciones y un modelo de IA entrenado con datos duplicados?

---

## Qué viene en la Parte 2

El hilo de IA, arrancando por el debate: ¿la IA nos vuelve menos inteligentes? Humanos aumentados o reemplazados, la ingeniería de prompts, la economía de tokens, la autonomía de los agentes y la supervisión humana, y explicabilidad, ética y caja negra.

---

**FIN DE LA PARTE 1 — Apunte Maestro clase03-04**
