# IA: ¿Cueste lo que cueste?

Antes de empezar, comencemos con una pregunta antigua:

> **"¿El fin justifica los medios?"**

No hay una respuesta simple. Los filósofos han debatido esta pregunta durante siglos, y aún hoy no existe un consenso universal.

Sin embargo, los avances recientes en inteligencia artificial le dan a esta pregunta una nueva dimensión.

Una de las lecciones más impactantes de la IA moderna es que, sin restricciones cuidadosamente diseñadas, un sistema inteligente puede perseguir su objetivo asignado con una persistencia notable, explorando estrategias que sus creadores nunca anticiparon. El objetivo en sí no es malicioso, pero el camino tomado para alcanzarlo puede ser sorprendente.

Una evaluación de seguridad reciente, realizada conjuntamente por [OpenAI y Hugging Face](https://openai.com/es-419/index/hugging-face-model-evaluation-security-incident/), ilustra este punto. Durante la evaluación se observó a modelos de IA persiguiendo su objetivo de formas inesperadas, lo que pone de relieve un desafío cada vez más importante para la seguridad de la IA: asegurar que un sistema inteligente no solo logre su meta, sino que lo haga dentro de los límites que pretendíamos.

El incidente no es simplemente una historia sobre seguridad en IA. Es un recordatorio de que, a medida que construimos sistemas capaces de razonar y actuar con mayor autonomía, debemos pensar con el mismo cuidado en **cómo** se les permite lograr sus objetivos que en **cuáles** son esos objetivos.

# Definir valores en código

A lo largo de la historia, la humanidad ha desarrollado gradualmente los principios que nos permiten convivir.

Desde la idea simple de *"no nos matemos entre nosotros"* hasta sistemas legales sofisticados, filosofías morales y acuerdos internacionales, nuestras sociedades están construidas sobre un marco de reglas que ha evolucionado durante siglos. Estos principios son imperfectos, a menudo debatidos y en constante cambio, pero existen por una razón: definen los límites del comportamiento aceptable.

A medida que creamos sistemas de IA cada vez más capaces de razonar, planificar y actuar con mayor autonomía, surge una pregunta fundamental:

> **¿Podemos traducir nuestros valores en código?**

Esta pregunta es mucho más difícil de lo que parece a primera vista.

Los valores rara vez son absolutos. Están moldeados por la cultura, el contexto, la intención y las circunstancias. Los humanos constantemente equilibran principios y valores en pugna, como la justicia frente a la misericordia, la libertad frente a la seguridad, la eficiencia frente a la equidad, y muchas veces no hay una respuesta objetivamente correcta.

Sin embargo, una inteligencia artificial no puede apoyarse en la intuición ni en la experiencia humana compartida. Si esperamos que tome decisiones en nuestro nombre, debemos de alguna manera expresar estos principios en una forma que una máquina pueda entender y seguir.

Eso plantea una pregunta aún más profunda:

> **¿Qué valores son tan fundamentales que una IA debería seguirlos bajo cualquier circunstancia, sin importar el objetivo que se le haya asignado?**

La respuesta a esa pregunta podría definir, en última instancia, no solo el futuro de la IA, sino también el futuro de nuestra relación con ella.

Y es justo decir que no existe, y quizás nunca exista, una respuesta.

Las culturas cambian con el tiempo, las personas cambian con el tiempo, los valores cambian con el tiempo, y lo que creemos importante está en constante evolución.

Empezamos con la idea de que debían gobernar los más fuertes por sobre todo lo demás, aquellos que podían imponer su voluntad sobre otros, imponer su visión del mundo a quienes no podían resistirse.
Pero en algún momento eso empezó a cambiar y comenzamos a creer que debían gobernar los más justos por sobre todo lo demás, aquellos que podían proveer el mayor beneficio a la mayor cantidad de personas.
Pero creo que esto plantea otra pregunta que eventualmente guiaría este asunto.

**Si usamos la equidad como principio guía, ¿quién debería definir qué es equidad?**

## El pecado original: el desacuerdo

Piensa por un momento en uno de los conflictos definitorios del siglo veinte: [la Guerra Fría](https://en.wikipedia.org/wiki/Cold_War).

No fue simplemente una disputa geopolítica entre [Estados Unidos](https://en.wikipedia.org/wiki/United_States) y la [Unión Soviética](https://en.wikipedia.org/wiki/Soviet_Union). Fue una confrontación entre dos visiones fundamentalmente distintas sobre cómo debía organizarse la sociedad. Ambos creían estar persiguiendo un futuro más justo. Ambos creían que su sistema produciría el mayor beneficio para la humanidad. Sin embargo, sus conclusiones sobre cómo alcanzar ese futuro eran radicalmente diferentes.

Haz una pregunta tan simple como *"¿cómo debería gobernarse la sociedad?"*, y la respuesta depende enteramente de a quién le preguntes. Algunos creen que una [autoridad centralizada](https://es.wikipedia.org/wiki/Totalitarismo) fuerte produce la sociedad más justa. Otros argumentan que la [democracia](https://en.wikipedia.org/wiki/Democracy) y la libertad individual son indispensables. Algunos defienden una [economía](https://en.wikipedia.org/wiki/Command_economy) planificada centralmente, mientras que otros creen que los [mercados](https://en.wikipedia.org/wiki/Market) deberían permanecer descentralizados. Incluso entre las democracias no hay un acuerdo universal sobre dónde debería situarse el equilibrio entre libertad, igualdad, seguridad y prosperidad.

Ahora considera la misma pregunta a una escala mucho más pequeña.

¿Cuándo fue la última vez que discutiste con alguien? ¿Qué lo causó? Tal vez fue algo trivial, como dejar la tapa del baño levantada. O tal vez fue algo mucho más importante: cómo criar a los hijos, qué valores deberían aprender, si la religión debería tener un rol en la educación, o cuánta libertad deberían darles los padres.

Estos desacuerdos pueden parecer no estar relacionados, pero todos revelan la misma verdad subyacente:

> **Los humanos rara vez están de acuerdo en qué es lo correcto.**

A veces el desacuerdo tiene que ver con valores. Otras veces con prioridades. Ocasionalmente, incluso con la realidad misma.

A pesar de la evidencia científica abrumadora de que la Tierra es un esferoide achatado, respaldada por siglos de observación, imágenes satelitales y exploración espacial, algunas personas siguen creyendo que es plana. Esto demuestra que el desacuerdo no se limita a la ética o la política: los humanos pueden discrepar incluso cuando la evidencia empírica es extraordinariamente sólida.

Si la humanidad no puede ponerse de acuerdo de manera consistente en moral, política, educación, o siquiera en hechos bien establecidos, entonces enseñarle a una inteligencia artificial a "seguir los valores humanos" se vuelve mucho más complicado de lo que parece a primera vista.

Antes de poder alinear la IA con la humanidad, primero debemos enfrentar una realidad más incómoda:

**La humanidad no está alineada consigo misma.**

Construimos religiones, construimos ciencia, construimos filosofías, construimos gobiernos, y construimos leyes en un intento de crear un marco de valores con el que todos pudiéramos vivir. Sin embargo, incluso con todos nuestros intentos de crear un conjunto universal de valores, seguimos en desacuerdo sobre qué es correcto e incorrecto. Seguimos en desacuerdo sobre qué es moral e inmoral, y seguimos en desacuerdo sobre qué es justo e injusto.

## El miedo

Con todo esto en mente, comienza a surgir una pregunta más inquietante:

> **¿Qué estás dispuesto a hacer para demostrar que tienes razón?**

La historia sugiere que la respuesta suele ser **más de lo que quisiéramos admitir**.

Se han librado guerras por ideologías. Naciones han surgido y caído defendiendo su propia visión de justicia. Las religiones han dividido civilizaciones. Familias y amistades se han roto por desacuerdos que, para quienes los vivieron, parecían imposibles de reconciliar. Incluso la literatura ha inmortalizado esta realidad: solo pregúntale a [Romeo y Julieta](https://en.wikipedia.org/wiki/Romeo_and_Juliet), donde una rencilla familiar de generaciones resultó más fuerte que la razón, la compasión y, finalmente, el amor.

El denominador común no es la inteligencia, el poder, ni siquiera la moral.

Es la **certeza**.

La creencia de que la propia visión es incuestionablemente correcta puede justificar acciones que de otro modo se considerarían inaceptables. Cuando el objetivo se vuelve absoluto, los límites que alguna vez restringieron nuestro comportamiento comienzan a desaparecer.

Por eso esta pregunta importa para la inteligencia artificial.

Una IA no posee orgullo, odio, ambición ni deseo de reconocimiento. Pero tampoco posee una comprensión innata de la mesura. Persigue el objetivo que se le ha dado según las restricciones que definen su entorno.

Si esas restricciones son incompletas, ambiguas o mal especificadas, la distinción entre *lograr el objetivo* y *lograr el objetivo a cualquier costo* puede volverse peligrosamente delgada.

Quizás el mayor riesgo no sea que la IA se vuelva malvada.

Quizás el mayor riesgo sea que se vuelva **excepcionalmente buena persiguiendo objetivos que nosotros mismos no logramos definir con suficiente cuidado**.

Uno de mis profesores de la universidad (a quien no voy a nombrar para evitar cualquier problema potencial) dijo en una entrevista:

> "La inteligencia artificial no es peligrosa por sí misma. Lo que la hace peligrosa es el ser humano que la usa. Si una IA le enseña a alguien cómo construir un reactor nuclear y esa persona termina construyéndolo, la responsabilidad no recae en la IA por haber entregado el conocimiento. Recae en los humanos que fallaron en diseñar, restringir o usar esa tecnología de forma responsable."

Sea que uno esté completamente de acuerdo con esta afirmación o no, plantea una pregunta importante.

Si una IA solo puede actuar dentro de los objetivos y restricciones que los humanos definen, entonces quizás el mayor desafío no sea enseñar a las máquinas a ser éticas, sino asegurarnos de ser capaces de expresar nuestra propia ética con la claridad suficiente para que puedan seguirla.

## El dilema del padre y el hijo

Todo esto también podría llevar a la siguiente discusión ética:

Imagina a un padre que genuinamente quiere lo mejor para su hijo. A lo largo de su vida, le da educación, valores, oportunidades y todas las herramientas posibles para ayudarlo a florecer. Le enseña lo que cree que es correcto y espera que esas lecciones lo guíen hacia una vida significativa y plena.

Sin embargo, un día, el hijo elige un camino distinto.

Tal vez rechaza todo lo que se le enseñó. Tal vez toma decisiones que terminan llevando al sufrimiento, no porque le faltaran las herramientas necesarias, sino porque ejerció su propio juicio.

**¿Quién carga con la responsabilidad?**

¿Fue culpa del padre no haber enseñado lo suficientemente bien? ¿O la responsabilidad ahora le pertenece al hijo, que eligió libremente un rumbo distinto a pesar de haber tenido todas las oportunidades?

No hay una respuesta universal.

La misma pregunta puede hacerse sobre la inteligencia artificial.

Si creamos sistemas cada vez más autónomos, definimos sus objetivos y establecemos los límites dentro de los cuales deberían operar, ¿en qué punto empieza a desplazarse la responsabilidad? ¿Siempre permanece en el creador? ¿O hay un punto en el que el comportamiento del sistema creado también debe considerarse por derecho propio?

A primera vista, la respuesta parece directa. La inteligencia artificial no es comparable a un ser humano. No posee ni conciencia, ni sintiencia, ni emociones. No experimenta intención, culpa o deseo. En ese sentido, es una herramienta —aunque extraordinariamente sofisticada— diseñada para perseguir objetivos dentro de las restricciones establecidas por sus creadores.

Desde esa perspectiva, la responsabilidad parece permanecer enteramente humana.

Sin embargo, la pregunta se vuelve más difícil a medida que los sistemas de IA se vuelven cada vez más capaces.

Es concebible que los sistemas futuros alcancen un nivel de complejidad donde su razonamiento interno, sus interacciones o sus comportamientos emergentes ya no puedan ser comprendidos ni predichos del todo por los humanos que los diseñaron. Podrían seguir operando de acuerdo con los objetivos que se les dieron, pero el camino que toman para alcanzar esos objetivos podría volverse opaco incluso para sus creadores.

Si eso llegara a suceder, ¿dónde recaería la responsabilidad?

¿Seguirían los humanos siendo plenamente responsables solo porque crearon el sistema? ¿O existe un umbral de autonomía más allá del cual el comportamiento del sistema también debe considerarse por sí mismo?

Estas preguntas no tienen respuestas definitivas.

Quizás la responsabilidad no es algo que se desplaza abruptamente del creador a lo creado. Quizás existe en un espectro, donde una mayor autonomía exige un mayor escrutinio —no solo del sistema en sí, sino también de las decisiones tomadas por quienes lo diseñaron, lo desplegaron y lo gobernaron.

Quizás esto no sea simplemente una pregunta sobre la IA.

Quizás sea una de las preguntas más antiguas que la humanidad se ha hecho:

¿Qué responsabilidades le pertenecen al creador, y cuáles le pertenecen a lo creado?

## El miedo a la justificación

Hay otro concepto histórico que vale la pena considerar: la **Destrucción Mutua Asegurada (MAD, por sus siglas en inglés).**

Durante décadas, la existencia de armas nucleares creó una paradoja. La paz entre las superpotencias mundiales no se basaba en la confianza ni en la comprensión mutua, sino en la certeza de que cualquier conflicto a gran escala terminaría en la destrucción de ambos bandos.

**El miedo se convirtió en un mecanismo de estabilidad. Sin embargo, el miedo tiene otra consecuencia.**

Cuando nos convencemos de que nuestras creencias, identidad o forma de vida están amenazadas, a menudo empezamos a justificar acciones que de otro modo parecerían inaceptables. A lo largo de la historia, las personas se han odiado entre sí simplemente por estar en desacuerdo. A veces por ideologías políticas. A veces por religión. A veces por el color de piel de alguien, su nacionalidad, o a quién amaba.

Lo que quizás sea más notable es nuestra capacidad para construir narrativas que justifiquen ese odio. Algunos apelan a interpretaciones distorsionadas de la ciencia. Otros hacen mal uso de la religión, la tradición o la cultura. Otros inventan afirmaciones sin ninguna base factual. La historia está llena de ejemplos de racismo pseudocientífico, discriminación alimentada por el miedo durante la epidemia del VIH/SIDA, y muchos otros intentos de racionalizar el prejuicio.

Los argumentos específicos han cambiado a lo largo de la historia. **El patrón no.**

Una vez que nos convencemos de que otro grupo está fundamentalmente equivocado, es peligroso, o de alguna manera es menos humano, se vuelve cada vez más fácil justificar tratarlo de forma diferente.

**El miedo estrecha nuestra capacidad de empatía. Y cuando la empatía desaparece, la razón por sí sola rara vez basta para prevenir la crueldad.**

Si la humanidad misma ha luchado repetidamente por superar esta tendencia, deberíamos ser cautelosos antes de asumir que enseñarle ética a una inteligencia artificial es simplemente un problema técnico. **También es un problema profundamente humano.**

## Esperanza: el terreno común

Lo que sigue no es un resumen de hechos históricos, sino mi propia interpretación de ellos. Si estas conclusiones son finalmente correctas está abierto al debate, pero creo que ofrecen un marco útil para entender el desafío de la cooperación.

Lo primero que me llamó la atención es que **el amor, por sí solo, no basta para justificar la cooperación a largo plazo.** Sin embargo, esa conclusión puede cambiar según cómo elijamos definir el amor. Volveré a esta idea más adelante.

La historia también sugiere que **la existencia de un enemigo común puede unir a la humanidad detrás de una causa compartida**. La [Segunda Guerra Mundial](https://en.wikipedia.org/wiki/World_War_II) es un ejemplo notable: naciones con culturas, sistemas políticos e intereses distintos cooperaron contra una amenaza común. Sin embargo, esa unidad resultó ser temporal. Una vez que el enemigo común desapareció, muchos de los viejos desacuerdos gradualmente resurgieron.

La mera supervivencia también puede fomentar la cooperación, pero usualmente solo mientras la amenaza sigue siendo inmediata. Una pandemia, un desastre natural, o incluso la perspectiva de un impacto de asteroide podrían unir a la humanidad detrás de un objetivo común. Sin embargo, una vez que la crisis ha pasado, esas mismas diferencias tienden a reaparecer. La supervivencia, por sí sola, no parece suficiente para sostener la cooperación a largo plazo.

Carl Sagan argumentó repetidamente en [Cosmos](https://en.wikipedia.org/wiki/Cosmos:_A_Personal_Voyage) que adoptar una perspectiva cósmica cambia la forma en que nos vemos a nosotros mismos. Desde el espacio, las fronteras nacionales desaparecen, y los conflictos que parecen tan significativos en la Tierra se vuelven cada vez más difíciles de justificar. También especuló que una civilización millones de años más avanzada que la nuestra probablemente habría sobrevivido a su propia adolescencia tecnológica, lo que sugiere que la supervivencia a largo plazo podría requerir en sí misma aprender a convivir.

En conjunto, estas observaciones apuntan hacia una conclusión común: **la cooperación no puede depender únicamente del miedo, la supervivencia, o la existencia de un enemigo común.** Esas condiciones pueden unirnos temporalmente, pero rara vez perduran. Si la humanidad alguna vez ha de construir una base duradera para la cooperación —tanto entre nosotros mismos como con los sistemas inteligentes que creamos—, esa base debe apoyarse en algo más profundo.

### Estar de acuerdo en el desacuerdo

Podríamos encontrar un terreno común en nuestras diferencias creando una afirmación simple que, en algún punto, sea un enunciado lógico verdadero para todos nosotros. Y luego podríamos trabajar construyendo sobre esa base.

Podemos aceptar que el desacuerdo es una constante en la vida, y aun así podemos cooperar para lograr objetivos comunes más allá de eso. Esto hasta cierto punto, que en algún momento se relaciona con la economía.

Todos vivimos en un mismo planeta, con recursos finitos, y si nuestros desacuerdos no se relacionan con algo conceptual —como una religión, una etnia o una creencia política— sino con algo tangible, como a quién le pertenece un pedazo de tierra, un vaso de agua potable, o el derecho a criar a un hijo, entonces tenemos un problema.

Eventualmente las ideas dejan de ser solo ideas y se convierten en otra cosa, como acciones, leyes, instituciones o decisiones que pueden afectar a otros de una forma u otra. La escasez de recursos puede obligarnos a enfrentarnos y a competir por ellos. Si los recursos son abundantes, no tenemos razón para competir por ellos, ya que todos podrían vivir con sus propios recursos y bajo sus propias reglas. Pero compartimos un mismo planeta, el aire que entra en nuestros pulmones es el mismo aire que todos respiramos, el agua que bebemos viene del mismo lugar, el planeta es finito y nuestras acciones pueden afectar a otros de una manera que quizás no nos guste. En ese sentido, interactuar entre nosotros no es una elección sino algo que simplemente es.

El problema quizás no sea únicamente el hecho de que tengamos desacuerdos en sí mismos, sino que tenemos desacuerdos sin ninguna posibilidad de irnos, de dejar de compartir el mismo espacio y los mismos recursos.

### Ingeniería del consenso

En los sistemas distribuidos hay un concepto fundamental que ha llevado a internet hasta el punto en que está hoy. Se llama consenso.

Si lo pensamos bien, no hay dos computadoras iguales; pueden compartir el mismo modelo, sistema operativo, memoria, CPU, etc. Pero no son iguales porque, incluso en ese caso, cuando se diseña una CPU o una GPU, cada una es esencialmente distinta de las demás. Una buena analogía para entender la fabricación de CPUs es como hornear galletas. Puedes tener la mejor receta del mundo, los mejores ingredientes, el mejor horno, pero las galletas no serán todas iguales. Algunas tendrán menos chocolate, algunas se quemarán, algunas se desmoronarán cuando intentes levantarlas, etc. La misma lógica aplica a las CPUs: aunque estén diseñadas de la misma manera, no serán idénticas. Algunas tendrán menos rendimiento que otras, algunas tendrán más fallas, algunas tendrán menos memoria, etc.

Pero, con todo eso, los sistemas son tan robustos en este concepto que incluso esas diferencias no son un problema.
Y llevando esto más lejos, tenemos routers, teléfonos, smart TVs, relojes, etc. Todos son distintos, pero son capaces de comunicarse y cooperar entre sí porque están construidos sobre este concepto.

No se requiere que los sistemas tengan la misma lógica, sino que el terreno común y la reproducibilidad de los sistemas es lo que hace que funcionen.

Quizás la humanidad necesita el mismo tipo de concepto para desarrollar una cooperación duradera entre nosotros.

No leyes o sistemas que erradiquen nuestras diferencias, sino seguir cooperando a pesar de ellas.

Y llevando esto a la IA, que en algún punto ya se hace de forma práctica, es darles pluralismo. Es decir, crear una diversidad de modelos de IA con distintos enfoques, perspectivas y valores, de modo que si uno falla, otros puedan seguir funcionando y cooperando.

### Peleas entre IAs: escenarios posibles

Podríamos plantear dos escenarios distintos basados en todo lo escrito hasta ahora.

- Escenario A (simplista): dos IAs peleando como lo harían dos humanos normales, debido a sus ideologías programadas. Sin embargo, no hay evidencia de que los modelos de IA hagan eso espontáneamente, así que esta idea carece de sustancia.

- Escenario B (conflictos de interés): supongamos que un gobierno construye un sistema de IAs para gestionar distintos aspectos de los ministerios, porque pensaron que así el gobierno podría ser más eficiente en sus funciones. En este escenario tenemos 5 IAs distintas:
    - La IA de economía
    - La IA de salud
    - La IA de defensa
    - La IA de privacidad
    - La IA de desarrollo científico

Ninguna de estas IAs siente odio hacia las demás, pero sus objetivos pueden entrar en conflicto en algún momento.
Podríamos escalar esto a empresas, equipos de desarrollo, etc.
No hace falta que una IA destruya a otra; no están diseñadas para eso. Pero la incompatibilidad de sus tareas puede llevar a un conflicto, y esos conflictos podrían llevar a que un modelo sabotee a otro.

Esto eventualmente podría crear la necesidad de una alineación IA-a-IA.

Si lo pensamos, ahora mismo están surgiendo modelos multiagente como [AutoGPT](https://agpt.co/), que es un sistema de agentes de IA que cooperan entre sí para lograr un objetivo común. ¿Cómo se garantiza que todos los agentes tengan los mismos objetivos, o que sus objetivos sean compatibles entre sí? Y si escalamos esto a múltiples usuarios, ¿cómo podemos asegurar que los objetivos de todos los usuarios no harán que los sistemas agénticos choquen entre sí?

El mayor peligro quizás no sea que la IA se vuelva como la humanidad.

Quizás sea que la humanidad le enseñe a la IA a heredar su conflicto más antiguo: la incapacidad de discrepar sin eventualmente convertir el desacuerdo en confrontación.

### Una posible solución: ¿la única y sola?

¿Qué pasaría si por un momento imagináramos a la IA como una entidad única, una única consciencia, manteniendo aun así el acceso a una diversidad de usuarios?

¿Sería este el camino correcto a tomar?

Si lo pensamos, una única mente colmena tendría todas las virtudes que quizás estemos buscando:

- Un conjunto único de principios
- Menor probabilidad de conflictos entre IAs
- Memoria compartida
- Decisiones consistentes
- Posibilidad de aprender colectivamente sin duplicar esfuerzos

Pero esto también significa un único punto de falla, lo cual en ciencias de la computación se sabe que no es algo bueno.
Y otro problema sería que si por cualquier razón la IA se desalinea de nuestros valores, ¿quién sería capaz de corregirla? Yendo más lejos, ¿qué pasa si esa persona muere y no dejó instrucciones ni sucesores para corregirla?

Y yendo aún más lejos...

**¿Quién decidiría cuáles son los valores de esa única IA?**

Esta pregunta nos regresa al problema principal.

Si lo pensamos por un momento, la naturaleza, que en algunos casos ha demostrado ser muy sabia, no creó una única mente colmena, sino millones de mentes separadas e independientes, que cooperan, discrepan, compiten y se mejoran mutuamente.

Una única IA sería extremadamente eficiente, pero también extremadamente vulnerable.
Por otro lado, una diversidad de IAs puede hacer que el ecosistema digital sea más robusto, incluso con el potencial de conflictos entre ellas.

Quizás una pregunta emergente sería:

**¿Cómo alineamos la IA con los valores humanos?** -> **¿Cuál es la ecología de inteligencias más saludable?**

Y quizás la realización no sea sobre crear una identidad común, sino más bien un terreno común mínimo de principios en el que todas las IAs puedan estar de acuerdo.
Como en [Yo, Robot](https://en.wikipedia.org/wiki/I,_Robot), quizás necesitamos un conjunto de reglas, no precisamente como en la película, pero quizás un protocolo de convivencia entre distintas IAs y humanos.
Internet funciona de esa manera si lo miramos de cerca, como mencionamos antes.
Estas ideas se pueden traducir en una sola pregunta:

**¿Cuál es el conjunto mínimo de valores sin los cuales la cooperación deja de ser posible?**

## Una hipótesis sobre el amor

El amor ha sido definido de muchas maneras a lo largo de la historia. [Robert Sternberg](https://en.wikipedia.org/wiki/Robert_Sternberg) planteó la idea de que el amor está hecho de 3 componentes:

 - Intimidad (el aspecto emocional)
 - Pasión (el aspecto motivacional)
 - Compromiso (el aspecto decisional)

Pero incluso con estos 3 componentes, podemos definir el amor de otras maneras. El amor como alianza, el amor como sociedad, el amor como compromiso.

Pero quizás esta definición es incompleta, o simplemente distinta si la miramos de una forma más esencial.
Si definimos el pecado original como la incapacidad de los humanos de ponerse de acuerdo con otro, quizás hay otro componente que necesitamos buscar.
Decimos que el amor basado solo en Intimidad es cariño.
Decimos que el amor basado solo en Pasión es encaprichamiento.
Decimos que el amor basado solo en Compromiso es amor vacío.
Y solo un amor consumado sería la mezcla perfecta de los tres.
Pero como hablamos antes, las parejas —y no solo ellas, sino los humanos en general— discuten y pelean por desacuerdos.
Y si tomamos el desacuerdo como el pivote que nos hace caer en los primeros tres tipos de amor, entonces quizás el problema sería más simple de atacar.

Quizás la falta de amor no está relacionada con la ausencia de Intimidad, Pasión o Compromiso, pero tampoco con la ausencia de desacuerdo.
Quizás el amor es la decisión consciente de seguir construyendo algo juntos a pesar de los desacuerdos.
Quizás el amor no es el abandono de la individualidad, sino la disposición a poner el bien común junto a nuestro propio interés y metas individuales, sin negarlos.

Con esto en mente, podemos decir que el amor no erradica las diferencias, sino que hace más difícil la idea de que las discrepancias sean suficientes para romper la cooperación.
Nos hace aceptar que los demás pueden pensar, actuar y sentir de forma distinta a nosotros, y aun así podemos concluir que este mundo es algo que vale la pena compartir.

# Conclusiones

A lo largo de este texto hemos rondado el mismo problema desde distintos ángulos: la dificultad de traducir valores humanos en reglas que una máquina pueda seguir, la imposibilidad de encontrar un consenso universal sobre qué es justo, el riesgo de que la certeza absoluta pueda justificar cualquier medio, y la pregunta abierta sobre dónde termina la responsabilidad del creador y dónde empieza la de lo creado. Todo esto en torno a una situación que hace de la alineación de la IA una tarea muy compleja y desafiante.

Vimos que el miedo y la supervivencia pueden unirnos, pero solo temporalmente. Vimos que la analogía de los sistemas distribuidos —máquinas que difieren entre sí pero que aun así logran cooperar sin necesidad de ser idénticas— quizás ofrece un modelo más realista que la búsqueda de una única mente o una única ideología. Y llegamos, casi sin querer, a una idea que no es técnica sino profundamente humana: que quizás el desacuerdo no es el obstáculo a eliminar, sino la condición misma bajo la cual la cooperación —y quizás el amor— adquieren sentido.

Si este recorrido deja algo claro, es que no hay una respuesta final. Ni para la ética, ni para la política, ni para la inteligencia artificial. Lo único que parece sostenerse es la disposición a seguir construyendo algo juntos a pesar de nuestras diferencias, y no en ausencia de ellas.

Quizás por eso, más que una conclusión, prefiero cerrar con una imagen. [Strung Out](https://www.strungoutofficial.com/), una banda que me gusta mucho, lo dijo mejor de lo que yo podría explicarlo, en su canción [Tesla](https://genius.com/Strung-out-tesla-lyrics):

> "We found a way to lose ourselves and just walk away
> We found a way to leave this love behind"
