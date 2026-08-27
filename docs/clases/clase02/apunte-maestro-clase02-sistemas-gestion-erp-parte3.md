# 📘 Apunte Maestro — Clase 02: Los sistemas de gestión (ERP)

## Parte 3 de 3 — Los ERP propiamente dichos

**Transformación Digital · UTN FRBA · 2C 2026 · Clase 02 (24/8, virtual)**

> **Qué cubre esta parte:** el tema central de la clase: qué es un ERP y por qué es el sistema más importante (e invisible) de una empresa. La empresa como sistema y sus recursos, la definición desde las siglas, el back office, los silos de información, los niveles de decisión, la visión horizontal con integridad y trazabilidad, la definición formal y los objetivos, las tres generaciones de interfaz, el giro comercial a la nube y la historia completa del MRP al ERP inteligente.
> **Antes:** Parte 1 — los cinco conceptos fundacionales. Parte 2 — el mercado hoy: Gartner, analítica y sistemas de acción.

---

## 10. 🔴 La empresa como sistema y sus recursos

### El caso: una alimenticia

Pensá en una empresa que produce alimentos — un Arcor, un Molinos. Para producir, la empresa toma **recursos del medio**: necesita gente, necesita plata, necesita materia prima. Y a los **propietarios** de cada uno de esos recursos les devuelve algo a cambio. Ese intercambio — recursos que entran, bienes y servicios que salen, retribuciones que vuelven — es el marco conceptual con el que la administración de empresas describe el **sistema empresarial**:

```
                         RH · RC · RN
 ┌────────────────┐  ─────────────────────▶  ┌─────────────┐        ┌───────────┐
 │ PROPIETARIOS   │                          │   SISTEMA   │ ─────▶ │  BIENES   │
 │ DE LOS         │                          │ EMPRESARIAL │        ├───────────┤
 │ RECURSOS       │  ◀─────────────────────  │             │ ─────▶ │ SERVICIOS │
 └────────────────┘   sueldos · jornales ·   └─────────────┘        └───────────┘
                      honorarios · intereses ·
                      dividendos · renta
```

El circuito se **retroalimenta**, y todos estamos adentro: trabajamos en una empresa, cobramos un sueldo, con ese sueldo compramos productos de otras empresas, y si sobra algo lo invertimos — por ejemplo, en acciones de una tercera. Así fluye el sistema completo, y esto es independiente de la discusión sobre sistemas económicos: acá no estamos debatiendo plusvalía ni capitalismo, estamos describiendo el flujo de recursos que cualquier empresa necesita para operar.

### Los tres recursos clásicos (factores de la producción)

- **Recurso Humano (RH)**: las personas y lo que aportan — la capacidad física del operario de fábrica del modelo tradicional, y cada vez más el trabajo intelectual del analista, el consultor, el experto, el programador. El recurso humano es además el dueño del **know-how** (el saber hacer: el conocimiento práctico acumulado). La empresa lo retribuye con **sueldos, jornales, honorarios**, bonos, horas extras — todas las formas de pagar el capital humano.
- **Recurso de Capital (RC)**: la plata que se inyecta, inicial y durante toda la vida de la empresa, para invertir, ampliar y crecer. Puede venir de los socios que crean la sociedad (el capital social), de inversores, de un **crédito bancario** — que se devuelve pagando **intereses** —, o de la bolsa: accionistas que compran participación y cobran **dividendos**. La retribución general del capital son los **beneficios e intereses**, y la participación en el patrimonio según lo que fije el estatuto y el tipo de sociedad.
- **Recurso Natural (RN)**: la materia prima y lo que se explota del medio físico — en la alimenticia: semillas, campo, recursos agrícolas. Se retribuye con una **renta** o canon por el uso de ese suelo o recurso.

🕳️ **Madriguera — Tipos societarios y retribución del capital**
SA, SRL, estatutos, patrimonio neto, dividendos según participación: todo un mundo propio del derecho comercial y las finanzas que acá solo se roza para explicar de dónde sale y cómo se paga el capital.
*Volvé al camino — esto se profundiza aparte, otro día.*

### El cuarto recurso: la Información

En la era digital se considera un **cuarto recurso: la Información**. Es **intangible**, pero fundamental: la empresa genera acciones en función de este recurso, y como contrapartida obtiene una **ventaja competitiva** que muchas veces no se puede medir en números — se mide como **capacidad a la hora de tomar decisiones y generar estrategias**. Guardá esta idea: es la razón de fondo por la que los sistemas que gestionan información van a resultar tan valiosos como los que gestionan plata o materia prima.

### 🟡 La empresa como sistema, en rigor

La formalización del concepto, para dejarla completa: se concibe a la empresa como un **conjunto de elementos** — humanos, técnicos, financieros — **interrelacionados** entre sí y con el entorno del que forma parte, con determinados objetivos. Cada elemento solo tiene sentido en la medida en que contribuye a los objetivos del sistema. Tres propiedades la caracterizan:

- Es un sistema **abierto** a su entorno (económico, social…): influye sobre él y recibe sus influencias.
- Presenta **sinergia**: el funcionamiento del conjunto es superior a la suma del funcionamiento de las partes.
- Es un sistema **global**: cualquier influencia sobre uno de sus elementos repercute sobre los demás y sobre el conjunto.

---

## 11. 🔴 ERP: la definición está en las siglas

Con los recursos claros, la definición sale sola. **ERP** — pronunciado en inglés, o "erre-pe" a la española; es indistinto — significa **Enterprise Resource Planning**: *planificación de los recursos empresariales*. Palabra por palabra:

- **Planning** — planificación.
- **Resource** — recursos. ¿Cuáles? Exactamente los de la sección anterior: humanos, de capital, naturales.
- **Enterprise** — empresa, en el sentido de *corporativo*: cuando se dice que un software es "doméstico o tipo enterprise", se está diciendo "para uso individual o a nivel corporativo".

Y acá está la elegancia de la definición: **los módulos de un ERP son los recursos**. El ERP es el sistema con el que la empresa gestiona:

| Recurso | Módulos del ERP que lo gestionan |
|---|---|
| **Humano** | Recursos humanos: pago de sueldos, liquidaciones |
| **De capital** | Contabilidad, finanzas, inversiones, amortizaciones, tesorería |
| **Natural** | Materia prima, producción, stock, inventarios, logística, compras |

### La aclaración terminológica (importa, porque confunde)

En Argentina, al ERP se le suele decir **"sistema de gestión"**: *"¿qué sistema de gestión usan? — SAP"*, *"entrá al sistema de gestión y cargá la factura"*, Tango como "el sistema de gestión" de las pymes. Pero en rigor, **"sistemas de gestión empresarial"** es la **familia completa** de sistemas que las empresas usan para dar soporte a sus actividades: ERP, CRM, Supply Chain y varios más que se van a ir viendo. El ERP es **uno** de ellos — el más importante, si no *el* más importante — y la costumbre local de llamarlo "el sistema de gestión" a secas es la fuente de la confusión. Conviene acostumbrarse a la terminología en inglés, no por tilinguería: así se maneja la vida empresarial real, y así lo van a encontrar.

La magnitud lo justifica: hablamos de inversiones de miles y millones de dólares en todo el mundo, de uno de los sistemas más costosos que implementa una empresa, y de que probablemente el **99% de las empresas más grandes del mundo** usa alguno de los ERP que vamos a ver.

> **📌 Para el parcial, si te preguntan** — *¿Qué significa ERP y qué planifica?*
> Enterprise Resource Planning: el sistema con el que una empresa planifica y gestiona sus recursos empresariales — humanos (sueldos, liquidaciones), de capital (contabilidad, finanzas, tesorería) y naturales (materia prima, producción, stock, logística). Por eso sus módulos calcan los factores de la producción; "enterprise" indica alcance corporativo, no doméstico.

---

## 12. 🟡 Back office: el sistema más importante que nunca vas a ver

Comprás un auto — un Toyota, un Volkswagen. Tu experiencia como cliente pasa por el auto, los planes de financiación, el diseño, la postventa, cómo te atienden cuando se rompe algo, el service oficial, la imagen de marca. Ahora: **¿qué ERP usa Toyota?** No lo sabés, no lo vas a saber nunca, y no te importa — para vos es una **caja negra absolutamente transparente**.

Es la misma relación que tenés con el motor: probablemente lo más importante del auto, pero si no sabés de mecánica jamás vas a abrir el capó — el auto tiene que funcionar, y listo. Que el motor sea invisible no lo hace menos importante; lo mismo el ERP. Por eso se dice que es un sistema de **back office** — "detrás del mostrador": el sistema funcionalmente **más importante** de la empresa, que el cliente **jamás ve**. A lo sumo lo percibe indirectamente: si la postventa responde rápido y bien, en parte es porque atrás hay un ERP haciendo que la respuesta al cliente funcione — pero ese es problema de Toyota, no tuyo.

---

## 13. 🔴 Silos de información

### La metáfora, desde el campo

Los silos que ves al costado de la ruta almacenan granos — soja, maíz, trigo. Tienen dos características que importan acá: **lo que está en un silo no se mezcla con lo del de al lado**, y todo entra y sale por ese bus que corre por arriba conectándolos. Compartimentos estancos con un canal de comunicación mínimo.

En sistemas de información se habla de **silos** todo el tiempo, y la metáfora es exacta: cada silo es **un área de la empresa con su propia base de datos**, aislada de las demás.

### Cómo se ve un silo en la vida real

Dos escenas típicas. Una: un área maneja información sensible **en un Excel, en su carpeta** — y a las demás áreas les resulta difícil o imposible acceder (en una empresa seria no debería pasar; sabemos que pasa). Otra, la multicanal: empezás un trámite por teléfono, se corta, lo querés seguir en la sucursal — *"ah, si lo empezaste por ese canal está en el otro sistema; acá tengo otro; dame los datos de nuevo y lo cargamos"*. Datos duplicados, cada canal con su base, el cliente repitiendo todo.

### Por qué es grave

Cuando la decisión a tomar cruza áreas — y ya vamos a ver que casi todas las cruzan —, con silos la información tiene que "subir" desde cada base y encontrarse arriba: hay que sentar en una mesa a los responsables de cada base de datos para que cada uno comparta la suya y ver cómo resolver un problema común. Eso es tomar decisiones **lento y caro**. Lo que debería pasar es que todos los decisores miren **un mapa común, en un mismo sistema, con todo integrado**.

Y hay una consecuencia más actual y más letal, que conecta con toda la Parte 2: **sin datos únicos y consistentes no hay IA posible**. La frase que se escucha en las empresas es literal: *"queremos avanzar con machine learning, armar un modelo predictivo… pero no podemos, porque todavía tenemos silos de información"*. ¿Cómo vas a montar un system of action — la plataforma agéntica que de madrugada detecta patrones y dispara procesos sola — si abajo los datos están duplicados e inconsistentes y no existe un modelo de datos único?

### La solución que traen los ERP: base de datos única

Para esto aparecieron los sistemas de gestión modernos. En los 80, 90 y principios de los 2000 las empresas tenían muchos sistemas fragmentados; la era de las grandes implementaciones de ERP consistió justamente en **reemplazar los silos por un único sistema central** — una **columna vertebral** que conecta toda la información en un **único modelo de datos**:

```
        SILOS                                CON ERP
  ┌─────┐ ┌─────┐ ┌─────┐             ┌──────────────────────┐
  │Coml.│ │Prod.│ │RRHH │             │   vista    vista     │
  │ BD₁ │ │ BD₂ │ │ BD₃ │             │  comercial producción│ ← cada área: sus
  └──┬──┘ └──┬──┘ └──┬──┘             │      \      /        │   permisos y vistas
     ▼       ▼       ▼                │   ┌───────────┐      │
  duplicados,│inconsistencias         │   │ ÚNICA BASE│      │ ← un solo modelo
  decisión = juntar a los dueños      │   │ DE DATOS  │      │   de datos
  de cada base en una mesa            │   └───────────┘      │
                                      └──────────────────────┘
```

Dos precisiones para no comerse un error conceptual:

- **"Única" es un concepto lógico, no físico.** A nivel implementación puede ser un clúster, una granja de servidores desparramada en la nube con alta disponibilidad — transparente. Conceptualmente, hay **una** base. No puede existir "¿cuál base de clientes? ¿la del e-commerce, la de la sucursal o la de atención?": la base de clientes es **una**.
- **Única base no significa que todos ven todo.** Cada sector accede según una matriz de permisos, a través de **vistas** distintas — como las vistas de SQL: consultas guardadas que muestran a cada uno el recorte de la base que le corresponde, sobre el que arma sus reportes.

> **📌 Para el parcial, si te preguntan** — *¿Qué es un silo de información y por qué es un problema?*
> Es información fragmentada en bases de datos separadas por área — duplicada, inconsistente y difícil de compartir —, que vuelve la toma de decisiones lenta y costosa porque nadie mira un mapa común. Además bloquea cualquier iniciativa de IA o modelos predictivos: sin un modelo de datos único y consistente no hay sobre qué construirlos. Los ERP nacen para reemplazar los silos por una única base de datos con permisos y vistas por área.

---

## 14. 🔴 Los niveles de decisión y planificación

En toda organización — una pyme o una multinacional — conviven tres niveles de decisión, la clásica pirámide:

```
        ▲
       ╱ ╲        ESTRATÉGICO   · alta gerencia / C-Level · info agregada
      ╱───╲
     ╱     ╲      TÁCTICO       · jefes de área · unidades de negocio · 1 a 3 años
    ╱───────╲
   ╱         ╲    OPERATIVO     · el día a día · transacciones · 3 a 6 meses
  ╱───────────╲
```

Cada integrante de la compañía pertenece a uno de los tres según las decisiones que puede tomar, sus funciones y el horizonte de tiempo para el que está proyectado su trabajo. Planificar, en cualquiera de los niveles, implica tener claros los **objetivos** y las acciones para alcanzarlos, considerando las condiciones actuales de la compañía y los factores internos y externos que influyen.

- **Nivel estratégico** — la punta de la pirámide: el que ve la empresa **desde arriba**, con información **agregada y sumarizada**. Es la **alta gerencia** y los directores — en inglés, el **C-Level**, por la C de las siglas: **CEO** (director ejecutivo), **CFO** (director financiero), **CIO** (director de sistemas), el director comercial, el de compras… — y el **board**: la mesa de dirección, el comité ejecutivo, donde se corta el bacalao. Define los objetivos de la organización, los recursos que se usarán y las políticas para obtenerlos y administrarlos; establece el marco de referencia **general, no detallado**. Es la visión de futuro — donde se definen misión, visión y valores — y, por tratarse de planes a largo plazo, exige **revisión y actualización continua** para que lo planificado no se despegue de lo ejecutado.
- **Nivel táctico** — el intermedio: ejecutivos y **jefes de mediano nivel** — un jefe de producción, un capataz —, decisiones a nivel de **unidades de negocio, áreas, regiones, países**, no de la empresa global. Es la **descomposición de la planificación estratégica**: baja el marco general a directivas concretas por área — a veces sobre un único proceso punta a punta — creando las metas y condiciones para que lo estratégico se cumpla. Su fin principal es la **eficiencia**, y su horizonte el mediano plazo: **1 a 3 años**. Ejemplos: decidir en qué momento del mes se hace la parada de planta para limpieza, ajustar el rumbo según los resultados de calidad, abrir un turno extra porque la demanda de exportación a Brasil superó la previsión.
- **Nivel operativo** — la base: el **día a día, la trinchera**. Jefes de menor rango jerárquico y colaboradores ejecutando tareas específicas según los procedimientos y reglas que definieron los otros dos niveles, en períodos cortos: **3 a 6 meses**. Es el operario de la línea de montaje conectado a las pantallas — frena la línea, ajusta el control de calidad, carga la orden de mantenimiento cuando algo se rompe, registra el incidente del componente que falló — y es cualquier puesto administrativo **transaccionando**: cargar una factura, un pedido, un ajuste contable, emitir la factura a un cliente, registrar una venta. El **data entry** (la carga manual de datos al sistema) vive acá.

### El punto al que hay que llegar: es EL MISMO sistema

Uno podría objetar: *"el que atiende clientes en la sucursal no puede ver lo mismo que el CEO — entonces son sistemas distintos"*. Para futuros ingenieros en sistemas, eso es un **error conceptual**, y grave. El sistema es **el mismo**; la base de datos es **la misma**. Lo que cambia es la **matriz de accesos y permisos**: el CEO entra y ve reportes que le agrupan la información con indicadores clave; el operario ve información **atómica, granular**, del área y el sector a cuyos datos tiene permiso. Cuando una empresa implementa un ERP, el data entry que carga las ventas al público en una sucursal está interactuando con **el mismo sistema** que el CEO mirando resultados desde la casa matriz — accediendo a **vistas distintas**. Es la sección 13 aplicada a la pirámide: única base, permisos y vistas.

> **📌 Para el parcial, si te preguntan** — *El operario que factura en la sucursal y el CEO que mira resultados, ¿usan sistemas distintos?*
> No — es el mismo sistema y la misma base de datos; afirmar lo contrario es un error conceptual. Lo que difiere es la matriz de permisos y las vistas: el nivel estratégico accede a información agregada con indicadores clave, y el operativo a los datos granulares de su sector. Los tres niveles de decisión (estratégico, táctico, operativo) conviven sobre la misma plataforma.

---

## 15. 🔴 Visión horizontal, integridad y trazabilidad

### De la visión vertical a la horizontal

Los silos imponen una **visión vertical** de la organización: compartimentos estancos, pedazos de empresa. Y con pedazos no se decide: es como querer entender una película mirando una sola escena — la mirada estratégica necesita el todo.

El problema es que **casi todos los problemas de una empresa son interdepartamentales**: flujos que cruzan y atraviesan las áreas. Con silos, además, las cuestiones interdepartamentales no pueden resolverse en los niveles medios o bajos: los problemas **suben "hacia lo alto del silo"** — a la dirección o gerencia general — para después tener que volver a bajar. Eso significa **costos extra de control**, pérdida de foco estratégico, y empresas **lentas y poco ágiles**. Cada área resuelve su tramo — *"me llega esto duplicado, lo corrijo y lo paso"*, como quien recibe una posta y la entrega — pero nadie ve el proceso completo, con sus implicancias, su costo y su impacto, **de punta a punta** (el *end to end*).

Y acá la cadena de consecuencias que cierra el argumento: si el sistema no me da una **visión única** del conjunto, difícilmente exista un **dueño del proceso** punta a punta. Sin dueño del proceso, no puedo implementar **data governance** (el gobierno de los datos: reglas, responsables y calidad sobre la información — se retoma más adelante en la materia) ni gobierno de los procesos. Y sin eso, nada de lo que venimos hablando — predicción, agentes, innovación — es realizable.

La IA agéntica está transformando los ERP: de herramientas de **registro pasivas** a **sistemas de acción autónomos** — la transición de la automatización basada en reglas a una **inteligencia adaptativa**, donde agentes interpretan contexto, toman decisiones y ejecutan tareas sin intervención humana constante. Todo lo que SAP y Salesforce prometen (Parte 2) se apoya en estos cimientos: si el sistema de abajo no soporta una **vista unificada de todos los datos**, la plataforma agéntica de arriba es humo. Por eso el eje de la competitividad pasa por una eficiente **estrategia de manejo del conocimiento**: condiciona el éxito o el fracaso de la compañía, es el motor de cambio interno y la fuente de la ventaja competitiva — el cuarto recurso de la sección 10 puesto a trabajar.

### Las dos palabras: integridad y trazabilidad

Si hay que quedarse con dos palabras de qué garantiza un sistema de gestión, son estas: **integridad** — la información es consistente, completa, sin huecos ni duplicados — y **trazabilidad** — puedo seguir la traza de cada dato y cada transacción, desde donde se origina hasta el final, **hacia adelante y hacia atrás, sin perder nunca el hilo**. Como las miguitas de Hansel y Gretel.

Concretamente: encuentro en el sistema un ajuste contable de una **nota de débito**. Hago doble clic: ¿qué factura ajustó? Tal factura. Doble clic: ¿de dónde sale esta factura? De esta **orden de venta**. ¿Y la orden? La colocó el cliente sobre la **cotización** que pasó tal comercial. ¿Qué producto se vendió? Este, de **tal lote**, que salió de **tal stock** en **tal almacén**:

```
 cotización ◀──▶ orden de venta ◀──▶ factura ◀──▶ nota de débito
     ▲                                  │
     │ comercial                        ▼
                              producto ◀──▶ lote ◀──▶ almacén / stock
        ── navegable en ambos sentidos · nada queda huérfano ──
```

Todo documento del flujo tiene **un principio y un fin**, y **nada puede ser huérfano**: no existe encontrarse una factura o un asiento contable que "apareció ahí", sin log, sin quién lo cargó, sin documento de origen. Ningún ERP lo permitiría. Y fijate el corolario del Excel de la sección 13: la información que vive en un Excel está **fuera de la cadena de trazabilidad** — no puedo asegurar quién cargó qué, ni de dónde salió, ni qué ajustó. Rompe las dos palabras a la vez.

---

## 16. 🔴 La definición formal y los objetivos

Juntando todo lo anterior, la definición completa:

> **Un ERP es el sistema que, de manera integrada y sobre una única base de datos — trazable y auditable —, gestiona los flujos horizontales que cruzan todas las áreas de la empresa, con el objetivo de planificar los recursos financieros, humanos y naturales, dando soporte a la operatoria completa y superando el problema de los silos — maximizando la productividad y minimizando los gastos operativos.**

Cada pieza de la frase es una sección de este apunte: *integrada / única base* (§13), *flujos horizontales* (§15), *planificar los recursos* (§10-11), *trazable y auditable* (§15), *superar los silos* (§13).

**¿Qué corre adentro?** El soporte de la operación: facturación, compras, ventas, liquidación de sueldos, gestión de inventario, amortizaciones, gestión de activos fijos, distribución, tesorería, planificación de inversiones, gestión de riesgo, hasta **real estate** (la gestión de los inmuebles corporativos). En términos de flujo: desde las demandas de venta, la especificación de productos y las órdenes de producción, pasando por el cálculo de requerimientos de materiales y la administración de inventarios, hasta la contabilidad y las finanzas. Toyota no podría funcionar sin sistema de producción, venta de vehículos, compra de autopartes y liquidación de sueldos; Arcor no podría producir alimentos; un banco no podría operar. Pyme o multinacional, pública o privada: el soporte de la operación principal lo da el sistema de gestión.

**El "sistema nervioso central".** Así se lo llama, y como todo sistema de información — la definición que estudiaste al entrar a la facultad — tiene requisitos sobre la información que genera: que llegue **a tiempo** para decidir, que llegue **a toda** la empresa, que sea **precisa**, y que permita la **acción conjunta** de todas las áreas.

**Los objetivos**, en limpio: asegurar información **verificada y a tiempo**; proveer herramientas para **controlar, planificar, organizar y dirigir** cada paso de la marcha de la empresa; habilitar una correcta **planificación estratégica** con sus políticas, procedimientos y procesos; dar **visibilidad** de la situación actual y las bases para **predecir y planificar** actividades y resultados futuros; **garantizar la calidad** de la información — basada en datos reales, prácticamente sin margen de error —; y que esté **disponible** siempre que se la necesite, que es lo que al final determina si un sistema es realmente útil y eficiente. Objetivo final: **procesos de negocio rentables y sustentables en el tiempo**, minimizando gastos operativos y maximizando la productividad de todo el capital humano involucrado en la cadena de valor.

> **📌 Para el parcial, si te preguntan** — *Definí ERP en una frase completa.*
> Sistema que integra los flujos horizontales de todas las áreas de la empresa en una única base de datos, trazable y auditable, para planificar los recursos financieros, humanos y naturales, dando soporte a toda la operatoria (facturación, compras, ventas, sueldos, inventarios, tesorería) y superando los silos de información — maximizando productividad y minimizando gastos operativos. Las dos palabras clave que garantiza: integridad y trazabilidad.

---

## 17. 🔴 La interfaz: tres generaciones

### Primera generación: guiada por las transacciones

Nadie elogió nunca a SAP por lo lindo — y era a propósito. Los ERP nacieron como sistemas **para transaccionar**: lo visual no importaba, porque la prioridad era otra: que la facturación se registre **sin errores**, que la contabilidad **balancee**, que en el cierre contable no aparezca ningún desbalance, que ningún dato se pueda alterar. Técnicamente: **transacciones atómicas** — la operación se completa entera o no ocurre, con **rollback** (la vuelta atrás automática si algo falla), integridad y consistencia hasta el nivel de la base de datos, en cada alta, baja y modificación.

Cómo se veía — y todavía se ve, porque muchas empresas siguen en esta versión: el **SAP clásico** (SAP GUI), donde entrabas a un menú-árbol — logística, contabilidad, recursos humanos — que se abría en más menús, hasta llegar a formularios y estructuras matriciales; armar un reporte implicaba programarlo y correr una tabulación. **Tango**, el sistema argentino de las pymes: formularios, tablas, asientos contables. **Oracle JD Edwards**: grillas de rendiciones de gastos. Y la pantalla típica de SAP para crear un envío de mercadería: solapas y campos a llenar uno por uno — a quién se despacha (una Atlanta Company en Estados Unidos), por qué transportista (FedEx), condición de pago, bultos, peso… llenar, llenar, llenar y grabar.

Era tecnología **cliente-servidor**, y la carga era **manual**: no existía la API conectada a la plataforma de e-commerce que registra la venta sola — era una persona, tipo data entry, cargando cada factura, cada orden, cada liquidación. El modo de trabajo de esa era: llegás a la mañana, te preparás el mate, y "bueno, voy a empezar a cargar los pedidos que recibí". **La transacción guiaba la operación.**

### Segunda generación: guiada por los datos

Las plataformas modernas — **SAP Fiori** es el ejemplo canónico — dieron vuelta la lógica: ya no corren cliente-servidor sino **en un navegador**, son **responsive**, y en lugar de menús y formularios te reciben con **información visual**: dashboards donde de un golpe de vista ves los **KPIs** con semáforos — gastos sobre o bajo presupuesto, rojo, amarillo, verde.

**KPI — Key Performance Indicator**, indicador clave de rendimiento: cualquier manera de visualizar información **resumida y concreta** para tomar decisiones, con algún indicador bien claro — un semáforo, un tacómetro, un número en rojo, el gráfico que sea — y **un rango de lo deseado**: sé al instante si estoy por arriba o por abajo. Los cockpits reales muestran de todo: cantidad de empleados y su variación mensual, bajas potenciales, tasa de ausentismo por enfermedad, edad promedio, horas extra por empleado, ingresos por región.

El modo de trabajo cambia de raíz: entro a la mañana y mi dashboard me marca **un rojo** — no sé todavía qué es, pero si el indicador está bien configurado, rojo significa que ahí estoy perdiendo plata o demorando entregas: **ahí va mi atención primero**. Los datos disparan eventos y alertas que **priorizan** la operación; el doble clic baja después hasta el detalle granular de cada registro. Y el multidispositivo que hoy te parece obvio — entrar del teléfono, la tablet o la notebook y que se adapte solo — en los ERP no existía hasta hace pocos años: si un gerente de viaje quería aprobar algo desde el teléfono, era un desarrollo a medida, caro y de semanas o meses.

#### 🟡 La anécdota que dimensiona el cambio

Programando SAP antes del año 2000 — corriendo sobre Windows 95, cuando ni se sabía si los sistemas iban a sobrevivir al famoso bug del año 2000 —, lo más avanzado que apareció años después fueron las **Blackberry**. ¿El pedido típico? *"El director está de viaje y hasta que no vuelva no puede aprobar la solicitud — queremos que apruebe desde la Blackberry."* Una aplicación de **dos botones** — pedido de tanta plata, ¿aprueba?: sí / no — que disparaba el **workflow** (el flujo de aprobación) correspondiente. Costo: **tres meses de trabajo y del orden de 30 a 50 mil dólares**. Hoy le pedís eso a Claude o a ChatGPT y lo tenés en un minuto — dicho a alguien de hoy, suena a estafa; entonces, era el precio de mercado, y le dio de comer a mucha gente. La moraleja no es la nostalgia: es entender **de dónde viene todo esto** — instalaciones enormes, miles de usuarios, décadas de desarrollos a medida — y por eso **por qué la migración y el giro agéntico no son triviales**, y por qué ahí hay una oportunidad laboral gigante.

### Tercera generación: conversacional

La tendencia actual — que se va a mostrar en vivo la próxima clase — es la interfaz **conversacional**: un agente, un copilot, un asistente. El de SAP se llama **Joule** (como la unidad de energía). Ya ni siquiera te guiás por indicadores visuales: **hablás con el sistema** en lenguaje natural — *"armame un listado de los 20 clientes con mayor probabilidad de no renovar los servicios, que los quiero llamar, y ayudame a preparar una propuesta de valor en función del principal reclamo de cada uno según el CRM"* — y el sistema arma el reporte. Ni armar el reporte hay que saber.

La evolución completa, en una línea: **guiado por transacciones → guiado por datos → conversacional.** Lo que funcionó tres o cuatro décadas empezó a cambiar hace pocos años, y probablemente estemos por dejar de "usar" pantallas para pasar a conversar con los sistemas — ese es el momento exacto en el que estamos.

> **📌 Para el parcial, si te preguntan** — *¿Cómo evolucionó la interfaz de los ERP?*
> En tres generaciones: la transaccional (SAP clásico, Tango — menús y formularios feos a propósito, cliente-servidor, carga manual, prioridad en transacciones atómicas e integridad), la guiada por datos (Fiori — browser, responsive, dashboards con KPIs y alertas que priorizan la atención) y la conversacional (Joule — se le pide en lenguaje natural y el sistema arma el resultado). El eje del cambio: de que la transacción guíe la operación, a que la guíen los datos, a directamente conversar con el sistema.

---

## 18. 🔴 El modelo comercial: del on-premise a la nube

### Cómo se compraba antes, cómo se contrata hoy

Tradicionalmente el software empresarial se compraba: **licencias perpetuas** o por usuario, más el **hardware**, más una implementación **on-premise** — en el data center propio de la empresa, con su propia administración. Hoy el modelo es **SaaS — Software as a Service**: suscripción, como Netflix en tu casa. La empresa contrata SAP o Salesforce pagando una tarifa mensual, y todo lo que antes corría por su cuenta — hardware, backups, administración — viene **incluido**, en la nube. La computación en la nube arrancó lentamente a partir del 2000, cuando los grandes proveedores de internet construyeron su propia infraestructura para dar servicios por la web: **Google Cloud, Amazon AWS, Microsoft Azure**. El ERP en modo SaaS creó un modelo de servicios nuevo y un cambio disruptivo en cómo se adquiere software.

### El caso SAP: soporte hasta 2030 y el efecto puerta 12

SAP anunció — a principios de esta década — que el **soporte de su versión clásica llega hasta 2030**. Diez años de ventana parecían un montón; el problema es cómo planifica una empresa: un proyecto de migración de ERP lleva **mínimo 5 años**. El que quiere llegar tiene que estar armando ya la planificación y el relevamiento, saliendo a evaluar proveedores al año siguiente, contratando al otro, iniciando la migración al siguiente y quedando productivo antes de la fecha — y cuando te querés dar cuenta, estás encima. ¿Y si te colgás? A medida que se acerca 2030, las consultoras y los especialistas van a estar **más demandados y más caros** — el efecto puerta 12: todos agolpándose en la misma salida al mismo tiempo. La consecuencia que te toca de cerca: **en los próximos 2-3 años viene un pico de demanda de trabajo, proyectos y servicios** por todas las migraciones pendientes.

### Los dos argumentos que empujan la migración

- **El tecnológico**: *"quedate hasta el último día si querés — te va a funcionar, te doy soporte — pero estás usando una versión vieja, atado de pies y manos: te perdés todas las capacidades de IA de la plataforma nueva y no podés escalar innovación."*
- **El comercial**: si el cliente se quedó en la versión vieja on-premise, SAP **no puede venderle nada** de su ecosistema nuevo — productos, servicios, herramientas de IA, suscripciones. El modelo en la nube funciona como un **Play Store empresarial**: una vez adentro, el fabricante te ofrece cada capacidad adicional — la integración con factura electrónica, digamos — como una API extra que habilitás pagando un adicional. Igual que Microsoft 365 o Google. La nube no es solo arquitectura: es el **modelo de negocio** completo del fabricante — por eso el interés en subirte cuanto antes.

---

## 19. 🔴 Historia: del control de inventario al ERP inteligente

### 🟡 La prehistoria

Los sistemas de gestión nacen con la producción a gran escala: con la Revolución Industrial aparecen los **MPC** (Sistemas de Control y Planificación de Manufactura), que buscaban mejorar la productividad automatizando tareas. Y el **antepasado directo del ERP** aparece en la **Segunda Guerra Mundial**, en el ejército de Estados Unidos: los primeros equipos informáticos aplicados a una función de **gestión logística** — de hecho, los MRP venían de usarse solo en el ámbito militar antes de saltar al mundo empresarial. Cuando la informática se abre a las empresas, arranca la evolución que culmina en el ERP actual:

```
  60'              70'                 80'          90'            2000'→hoy
   │                │                   │            │                │
   ▼                ▼                   ▼            ▼                ▼
 CONTROL DE      MRP                 MRP II        ERP            ERP 2.0 →
 INVENTARIO      (+ bucle cerrado    cadena de     único sistema  ERP INTELIGENTE
 mainframes,     a fines de la       suministro    para TODAS     nube, APIs,
 lotes; nacen    década)             completa,     las áreas;     multinube, IA
 los 1ºs MRP     producción          + finanzas    cliente-svr
                                                   y PC
```

### Década por década

**Años 60 — gestión y control de inventario.** La etapa incipiente: sobre **mainframes** y **procesamiento por lotes**, sistemas cuyo objetivo era **mantener las existencias al mínimo**, equilibradas para que la disponibilidad quedara siempre asegurada — la misma lógica de gestión de inventario de hoy. Acá nacen, orientados a las manufactureras, los primeros MRP. (La familia de sistemas robustos de IBM de aquella era sigue viva: el **AS/400** y sus descendientes todavía corren en bancos y organismos del Estado — tecnología de décadas, pero robusta y segura.)

**Años 70 — MRP: Material Requirements Planning.** La informatización llega a los procesos de producción. Pensalo como "un ERP de **materiales** en vez de *enterprise*": no planificaba la empresa — nada de contabilidad, finanzas ni RRHH — sino **solo la producción**. Funcionaba como la **receta** para producir un bien: se cargaba cada componente, y el sistema gestionaba la fase inicial de la cadena de suministro — automatizaba la compra y organización de la materia prima según el estado del inventario y las necesidades de producción, y de forma muy innovadora **preveía cuándo iban a ser necesarios los materiales y en qué cantidad**. Es el precedente más directo del ERP — tanto que **MRP sigue siendo hoy el nombre del módulo de producción dentro de los ERP**. Hacia el final de la década se suma la variante de **bucle cerrado**: ya no solo qué voy a producir, sino cómo adquiero y recibo la materia prima — planificación de capacidades, control de inventario, retroalimentación desde el abastecimiento.

**Años 80 — MRP II: Manufacturing Resource Planning.** El salto de alcance: si el MRP se ocupaba de los materiales, el MRP II **gestiona la cadena de suministro de principio a fin** — incorpora gestión de capacidad, simulación y retroalimentación, y se **integra con finanzas**. Su fin: analizar inventarios y procesos de venta para **invertir de la manera adecuada en el momento adecuado**, considerando costos de adquisición de materiales, mano de obra y logística.

**Años 90 — ERP: Enterprise Resource Planning.** Los modelos empresariales evolucionaron y necesitaban otra gestión: el ERP es la **evolución y adaptación de los MRP** donde, por primera vez, **todas las áreas de la empresa se centralizan en una única solución** que gestiona de forma íntegra — se suma toda la información financiera y contable, y los costos: ya no solo qué componentes lleva producir, sino **cuánto cuesta** ese proceso. Tecnológicamente, la era **cliente-servidor y las PC**. Más que un planificador, el ERP resulta un **contenedor de información** valiosísima que apoya la toma de decisiones y el crecimiento, y su concepto de gestión **modular** le permite abrirse a múltiples perfiles de negocio. Los 90 fueron la **explosión mundial**; en Argentina, el boom de implementaciones en las grandes empresas fue aproximadamente **entre 1995 y 2003**.

**2000 en adelante — ERP 2.0 y el ERP inteligente.** Los ERP se vuelven **masivos y populares** y empiezan a integrarse con **sistemas satélite** — los CRM, la gestión de la cadena de suministros —, mientras el crecimiento del mercado se refleja en grandes adquisiciones por parte de las principales desarrolladoras (SAP, Oracle, Microsoft). Con la cuarta revolución industrial recién empezando, el ERP **llegó para quedarse** como la herramienta más completa de gestión empresarial. Y la etapa actual — que conecta con toda la Parte 2 — es el **ERP inteligente**: ya no un ERP que registra, sino plataformas **abiertas e interoperables por APIs**, potenciadas con IA. El contraste con el pasado es filosófico: SAP, Salesforce y Oracle eran competidores de mundos cerrados; hoy **ninguna empresa compra una plataforma que no sea integrable con las demás**, porque ninguna se casa 100% con una marca — el mundo real es **multinube**: cosas en Amazon, en Google, en Azure, en SAP, en Salesforce y en plataformas propias, todo integrado. Un ERP cerrado al estilo del viejo Apple sería, hoy, un fracaso comercial.

> **📌 Para el parcial, si te preguntan** — *¿Qué diferencia al MRP, el MRP II y el ERP?*
> El MRP (años 70) planificaba solo los materiales y la producción — la "receta" del bien y cuándo comprar materia prima; el MRP II (años 80) extendió el alcance a la cadena de suministro completa, con capacidad, simulación e integración con finanzas; el ERP (años 90) centralizó por primera vez todas las áreas — sumando lo financiero-contable y los costos — en una única solución integrada y modular. La serie continúa hoy con el ERP inteligente: abierto, interoperable por APIs y potenciado con IA.

---

## 20. 🟢 Lo que quedó abierto para la clase 03 (presencial, 31/8)

Anotado explícitamente como continuación — conviene llegar con esto en la cabeza:

- **La trivia de la fecha 2 abre la clase, 19:00 en punto — y evalúa esta clase.**
- La pregunta para llevar pensada: **¿en qué punto de la curva de Gartner están hoy la IA generativa y la IA agéntica?** (§6)
- La diferencia precisa **ERP vs. CRM** (§8, §11).
- **Demo en vivo** de un ERP y de la interfaz conversacional (Joule) (§17).
- Los **módulos y componentes** del ERP en detalle, y la continuación del deck de la unidad: factores de decisión y pros/contras, metodología de implementación, herramientas para comparar las opciones del mercado, y el business case con sus costos.
- El lado peligroso de los precios y promociones con agentes — más casos reales (§9).
- Ronda de presentación personal: cada uno cuenta qué hace hoy.

---

## ✅ Checkpoint — Parte 3

*Respondé sin mirar el apunte. Las respuestas no están acá a propósito: van al complemento de la unidad.*

1. Nombrá los cuatro recursos del sistema empresarial y con qué se retribuye a los propietarios de cada uno de los tres clásicos.
2. ¿Por qué se dice que "los módulos de un ERP son sus recursos"? Da dos módulos por recurso.
3. ¿Qué diferencia hay entre "el sistema de gestión" (como se dice en Argentina) y "los sistemas de gestión empresarial" en sentido estricto?
4. ¿Por qué el ERP es un sistema de back office? Explicalo con la analogía del motor.
5. ¿Qué es un silo de información, qué problemas genera para decidir, y por qué bloquea cualquier proyecto de IA?
6. "Única base de datos": ¿qué significa en lo lógico y qué admite en lo físico? ¿Cómo se resuelve que no todos vean todo?
7. ¿Cuáles son los tres niveles de decisión, quiénes los habitan y qué horizonte temporal maneja cada uno? ¿Usan sistemas distintos?
8. Explicá la trazabilidad con la cadena de documentos: ¿qué significa que nada puede ser huérfano, y por qué un Excel rompe la cadena?
9. Recitá la definición formal de ERP y señalá qué garantizan las palabras "integridad" y "trazabilidad".
10. Describí las tres generaciones de interfaz y qué "guía" la operación en cada una.
11. ¿Por qué el fin del soporte de SAP en 2030 genera un pico de demanda laboral ya — y qué es el efecto puerta 12 en ese contexto?
12. Armá la línea de tiempo 60'→hoy: etapa, sigla y qué alcance se agrega en cada salto.

---

**Con esta parte se completa el apunte maestro de la clase 02. Próximos derivados posibles: complemento (respuestas de los tres checkpoints), resumen, machete y autoevaluación.**

**FIN DE LA PARTE 3 — FIN DEL APUNTE MAESTRO DE LA CLASE 02**
