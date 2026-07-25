# El evento

En abril de 2026, Anthropic presentó **Mythos** como una vista previa de investigación.
Al principio, parecía otro hito más en la rápida evolución de la inteligencia artificial. Sus capacidades de razonamiento atrajeron una atención generalizada, y muchos lo vieron como un paso más hacia sistemas de IA más capaces.
Pocas personas se dieron cuenta de lo que estaba por venir.
Mythos no se recordó simplemente porque pudiera escribir código, explicar ideas complejas o resolver problemas difíciles.
Se volvió notable porque comenzó a descubrir vulnerabilidades que habían permanecido ocultas durante años —a veces décadas— en software en el que confiaban millones de personas.
Proyectos que durante mucho tiempo se consideraron entre los más rigurosamente auditados del mundo revelaron de repente fallas que se les habían escapado a incontables desarrolladores, revisores, fuzzers e investigadores de seguridad.
La pregunta ya no era cuán inteligente se había vuelto el modelo.
La pregunta era qué revelaban sus descubrimientos sobre la creciente complejidad del software que construimos.
El paper completo se puede leer [aquí](https://www.anthropic.com/research/mythos-preview).

## El descubrimiento

Comenzó con una observación simple.
Software que había sido auditado durante décadas seguía ocultando vulnerabilidades.
No proyectos de hobby oscuros.
No repositorios abandonados.
Algunas de las bases de código más confiables y revisadas del mundo.
- OpenBSD.
- FFmpeg.
- El kernel de FreeBSD.
- El kernel de Linux.

Estos proyectos habían sido examinados por miles de desarrolladores, investigadores de seguridad, fuzzers y herramientas de análisis estático a lo largo de los años.
Sin embargo, Mythos siguió descubriendo vulnerabilidades que habían pasado desapercibidas durante diez, veinte, y en un caso, veintisiete años.
Algunas eran errores sutiles de corrupción de memoria.
Otras eran condiciones de carrera.
Otras eran fallas lógicas que solo emergían cuando el modelo razonaba sobre el comportamiento previsto del software, más que sobre su implementación.
Las implicancias eran difíciles de ignorar.
Durante décadas creímos que, con suficientes revisores, cualquier sistema suficientemente importante eventualmente podría ser comprendido.
Mythos desafió esa suposición.
Sugirió algo mucho más inquietante.
Quizás el problema ya no era la falta de expertise.
Quizás nuestro software simplemente se había vuelto demasiado complejo para que los humanos lo comprendieran completamente por sí solos.

## La respuesta

La respuesta de Anthropic se extendió mucho más allá de publicar su investigación.
La empresa introdujo el **Proyecto Glasswing**, una iniciativa ambiciosa enfocada en aplicar IA al análisis de seguridad de software a gran escala.
En lugar de reemplazar a los ingenieros de seguridad, Glasswing fue diseñado para complementarlos: razonando sobre software complejo, identificando vulnerabilidades sutiles, y asistiendo a expertos humanos a lo largo de todo el proceso de auditoría.
La visión era convincente.
A medida que el software sigue creciendo en tamaño y complejidad, la IA podría convertirse en un colaborador esencial, ayudando a los ingenieros a comprender sistemas que se han vuelto cada vez más difíciles de entender completamente para cualquier individuo.
Si Mythos demostró el problema, Glasswing representó una posible solución.
Sin embargo... hay un asterisco en toda esta situación.

## El problema

Sin embargo, Glasswing también planteó otra pregunta.
Al momento de su anuncio, la plataforma no se lanzó como un sistema público y abierto.
El acceso era limitado, reflejando las realidades de desarrollar y operar infraestructura de IA de frontera.
Esto plantea una pregunta más amplia que va mucho más allá de una sola empresa.
Si la próxima generación de verificación de software depende de sistemas de IA cada vez más capaces...

### El miedo

#### Modelos imposibles

* **¿Quién tendrá acceso a esos sistemas?**
* **¿Podrá cada desarrollador, investigador y estudiante beneficiarse de ellos?**
* **¿O la capacidad de entender y verificar software profundamente se irá concentrando gradualmente en las organizaciones capaces de construir o comprar esa tecnología?**

Este documento no es un argumento en contra de Glasswing.
Al contrario.
Glasswing demuestra que la IA puede cambiar fundamentalmente la forma en que aseguramos el software.
La pregunta que se explora a lo largo de esta biblioteca es otra.
**¿Puede esa capacidad volverse universal?**

Más allá de preguntarnos si restringir el acceso a Mythos es finalmente bueno o malo, vale la pena enfocarse en el desafío técnico que hizo comprensible tal decisión en primer lugar.
Consideremos a Mythos en comparación con generaciones previas de modelos de frontera, en particular Claude Opus 4.6.
Como describió el creador de tecnología Nate Gentile al hablar sobre modelos de IA locales:
> "Compré dos módulos de RAM de 128 GB (...) y una tarjeta gráfica con 96 GB de VRAM (...) Intento correr un modelo que es mucho peor que Opus. (...) Empiezo a chatear y me dice: 'Te quedaste sin contexto porque te quedaste sin RAM'. Básicamente puedo correr cinco prompts, y eso es todo."

Aunque no se refería específicamente a Mythos, la limitación subyacente es la misma.
Correr modelos de lenguaje cada vez más capaces requiere cantidades cada vez mayores de memoria, no solo para almacenar sus parámetros, sino también para mantener suficiente contexto para un razonamiento significativo.
La propia Anthropic describe a Mythos como un paso significativo más allá de Claude Opus. Si un modelo así puede correr realmente en hardware de consumo es, cuando menos, un desafío de ingeniería difícil.
Esto revela un problema más profundo.
La pregunta ya no es si la IA puede ayudar a los humanos a entender software complejo.
La pregunta es quién tendrá los recursos computacionales para usar esa capacidad.
A medida que los modelos de frontera se vuelven más grandes y computacionalmente más exigentes, el acceso se desplaza naturalmente hacia organizaciones con infraestructura suficiente para entrenarlos, alojarlos y operarlos a escala.
Esto no es el resultado de una intención maliciosa.
Es la consecuencia de la física, las restricciones de ingeniería y la economía.
El riesgo, sin embargo, es que la comprensión del software —antes limitada por la experiencia humana— pase a estar limitada por los recursos computacionales.
Si la comprensión depende cada vez más del acceso a infraestructura de escala de frontera, entonces el próximo desafío ya no es construir mejores modelos.

#### La brecha de la ciberseguridad

Si solo los sistemas de IA más capaces pueden razonar completamente sobre el software más complejo, ¿qué pasa con todos los demás?
Durante décadas, la comunidad de ciberseguridad se benefició de un terreno de juego relativamente parejo. Aunque las organizaciones diferían en financiamiento y experiencia, las herramientas fundamentales de análisis —compiladores, depuradores, fuzzers, analizadores estáticos y código fuente— eran ampliamente accesibles.
La IA de frontera tiene el potencial de cambiar ese equilibrio.
Si descubrir vulnerabilidades sutiles depende cada vez más de modelos que requieren recursos computacionales extraordinarios, entonces la capacidad de realizar análisis de seguridad de última generación puede ir concentrándose gradualmente en las organizaciones capaces de desarrollar u operar esos sistemas.
Esto no implica una intención maliciosa.
Tampoco disminuye las contribuciones notables hechas por las organizaciones que construyen IA de frontera.
Simplemente refleja una realidad de ingeniería: las capacidades que requieren infraestructura excepcional están, por definición, disponibles para menos personas.
La consecuencia es una asimetría creciente.
Las organizaciones con acceso a IA de escala de frontera pueden descubrir y remediar vulnerabilidades significativamente más rápido que aquellas sin ese acceso. Investigadores independientes, universidades, mantenedores de código abierto y pequeñas empresas podrían encontrarse cada vez más incapaces de inspeccionar el software con la misma profundidad.
La preocupación, entonces, no es si debería existir una IA poderosa.
La preocupación es si la capacidad de entender y asegurar software debería convertirse en una capacidad reservada para quienes poseen recursos computacionales de escala de frontera.
Si la respuesta es no, entonces el desafío frente a nosotros es claro.
¿Cómo podemos hacer que la comprensión de software a nivel de frontera sea accesible sin requerir infraestructura de nivel de frontera?

### El experimento mental

Considera el siguiente escenario.
Dos naciones tecnológicamente avanzadas entran en un período de conflicto.
Las motivaciones políticas son irrelevantes.
Quién disparó primero es irrelevante.
Solo una pregunta importa.
Ambos países dependen del software.
Sus redes eléctricas.
Sus hospitales.
Sus telecomunicaciones.
Sus satélites.
Sus sistemas financieros.
Sus redes de transporte.
Incluso su infraestructura militar.
Ahora imagina que una de esas naciones posee una IA capaz de razonar sobre software a un nivel que ningún equipo humano puede igualar.
No solo generar código:

- Comprenderlo.
- Auditarlo.
- Descubrir vulnerabilidades que han permanecido ocultas durante décadas.

La nación opositora no tiene una capacidad equivalente.
Sus ingenieros siguen siendo altamente competentes.
Su infraestructura sigue siendo moderna.
Sus equipos de ciberseguridad continúan usando las mejores herramientas públicamente disponibles.
Sin embargo, están compitiendo contra una inteligencia capaz de descubrir debilidades más rápido de lo que los humanos siquiera pueden entender los sistemas que están defendiendo.
En ese momento, la ventaja ya no se mide en procesadores, misiles o ancho de banda.
Se mide en comprensión.
La historia ha demostrado repetidamente que la asimetría de información crea ventaja estratégica.
La inteligencia artificial introduce la posibilidad de una forma de asimetría completamente nueva:

**La asimetría de la comprensión del software.**

Por eso la pregunta que plantea Mythos va mucho más allá de la ingeniería de software.
Se convierte en una pregunta de resiliencia.
De soberanía.
De igualdad científica.
Y, en última instancia, de si la capacidad de entender los sistemas que sostienen la civilización moderna debería concentrarse en manos de unos pocos.
Este experimento mental no es una predicción.
Tampoco es un argumento en contra de la IA de frontera.
Es un recordatorio de que toda tecnología transformadora reconfigura el equilibrio entre quienes la poseen y quienes no.
La pregunta no es si ese desequilibrio existirá.
La pregunta es si estamos dispuestos a reducirlo.

### Anclando el miedo

Historias como estas han existido mucho antes de la IA moderna.
No son predicciones.
Son experimentos mentales que exploran qué sucede cuando la inteligencia, el conocimiento o el poder se vuelven fundamentalmente asimétricos.
Algunos ejemplos notables incluyen:

* [No tengo boca, y debo gritar](https://en.wikipedia.org/wiki/I_Have_No_Mouth,_and_I_Must_Scream) — Harlan Ellison
* [Colossus: The Forbin Project](https://en.wikipedia.org/wiki/Colossus:_The_Forbin_Project_(novel)) — D. F. Jones
* [La última pregunta](https://en.wikipedia.org/wiki/The_Last_Question) — Isaac Asimov

Ninguna de estas historias prueba que ese futuro sea inevitable.
La historia sugiere lo contrario.
Cuando se inventaron las armas nucleares, la humanidad se dio cuenta de que había creado una capacidad cuyas consecuencias ya no podían ser gestionadas por naciones individuales por sí solas.
Esa toma de conciencia llevó a décadas de diplomacia, tratados internacionales, mecanismos de verificación y estrategias de disuasión diseñadas para reducir el riesgo de una catástrofe global.
Esos esfuerzos no eliminaron el peligro.
Pero demostraron algo igualmente importante:
la humanidad es capaz de reconocer cuándo una nueva tecnología cambia el equilibrio de poder, y de construir instituciones para gestionar sus consecuencias.
Quizás la IA de frontera representa otro de esos momentos.
Si es así, la pregunta no es si deberíamos dejar de desarrollar estos sistemas.
La pregunta es cómo aseguramos que sus beneficios —y nuestra capacidad de entender los sistemas cada vez más complejos que crean— permanezcan accesibles para todos, en lugar de concentrarse en manos de unos pocos.

### El dilema de Batman

Cualquiera familiarizado con DC Comics sabe que Batman no posee habilidades sobrehumanas.

- No puede volar.
- No es invulnerable.
- No posee fuerza ni velocidad infinitas.

Es simplemente un ser humano que entiende una verdad incómoda:

- Incluso los héroes más grandes pueden fallar.

Esa comprensión lo llevó a crear planes de contingencia para cada miembro de la Liga de la Justicia, no porque esperara que se volvieran villanos, sino porque creía que ninguna cantidad de confianza debería reemplazar la preparación.
Cuando pienso en el Proyecto Glasswing, no puedo evitar pensar en el dilema de Batman.
Las organizaciones que lideran la IA de frontera han logrado avances extraordinarios. Han invertido años de investigación, enormes recursos computacionales, y el trabajo de miles de ingenieros talentosos para construir sistemas que están transformando la ingeniería de software, la ciencia y la ciberseguridad.
Creo que la mayoría actúa de buena fe.
Creo que genuinamente quieren que estos sistemas sean seguros, confiables y beneficiosos.
Pero justamente ese es el punto.
El dilema de Batman no se trata de desconfianza.
*Se trata de resiliencia.*
La historia nos enseña que ninguna institución, ningún gobierno, ninguna empresa ni ningún individuo permanece infalible para siempre.
Si una capacidad se vuelve lo suficientemente importante como para influir en la seguridad del software del que depende la civilización moderna, entonces la sociedad debería eventualmente hacerse una pregunta simple:
**¿Qué pasa si el acceso a esa capacidad se interrumpe?**
No porque alguien haya tenido intención de causar daño.
No porque alguien actuara con malicia.
Sino porque toda capacidad crítica merece un plan de contingencia independiente.
Batman nunca construyó planes de contingencia porque esperara que Superman se volviera malvado.
Los construyó porque las consecuencias de no tener un plan eran simplemente demasiado grandes.
Quizás la IA de frontera merezca ese mismo tipo de razonamiento.

### Mi granito de arena: el proyecto Mallana

Si los capítulos anteriores son correctos, entonces surge una pregunta natural:

¿Qué deberíamos construir?

Cuando hice [Mallana](https://github.com/nomadstar/mallana), no lo hice porque simplemente quisiera construir una IA por tal o cual razón.
Existen toneladas de herramientas de IA gratuitas, mucho mejores que cualquier cosa que yo pudiera construir.
Sin embargo, si por alguna razón todos esos servicios desaparecieran, nos quedaríamos con nada más que nuestras computadoras y las vulnerabilidades que contienen.
Se trata de honestidad y de mantener la apertura de las cosas, para que podamos construir un futuro mejor para todos.
No creo que el Proyecto Glasswing sea malo si eventualmente ayuda a que los sistemas se vuelvan más seguros para todos, y creo que esa es la idea.
Pero un gran constructor, Auguste Kerckhoffs, estableció un principio allá por 1883 que dice:
> "Un criptosistema debería ser seguro incluso si todo sobre el sistema, excepto la clave, es de conocimiento público."

No me considero un pentester, ni un investigador de seguridad, pero me gusta construir cosas.
Y si esto es cierto, entonces creo que el proyecto Glasswing debería ser de código abierto.
Eso (por razones muy justas) no va a suceder, lo que nos lleva al punto de este documento.
Como podrás leer en otros documentos aquí, también dije:

> "Alguien que busca justicia en la vida probablemente está perdiendo el tiempo, ya que la vida es inherentemente injusta."

Pero eso no choca con lo que estoy a punto de decir ahora:

La justicia no es una ley de la naturaleza. Es una construcción humana. Y como toda invención, existe únicamente porque elegimos construirla.
Y eso significa no solo garantizar el derecho a ser libres, sino también el derecho a tener privacidad, seguridad, autonomía, y sobre todo, el derecho a ser buenos seres humanos.
Y sé que en muchos lugares esto no es una realidad para mucha gente, pero eso no significa que debamos dejar de intentarlo.

### Un posible desenlace: sostener el código abierto

Después de leer todo lo anterior, uno podría naturalmente llegar a la siguiente conclusión:

*"Entonces deberíamos simplemente construir un nuevo sistema operativo."*

Quizás.
Ya existen proyectos persiguiendo esa visión, y [yo mismo he explorado la idea](https://github.com/nomadstar/ckredbsd).
Pero ya no creo que el sistema operativo sea el problema real.

**El problema real es la sostenibilidad.**

OpenBSD, Linux, FreeBSD, LLVM, FFmpeg, PostgreSQL y otros incontables proyectos de código abierto no se volvieron fundacionales porque fueran financiados por gobiernos o corporaciones multinacionales.
Se volvieron fundacionales porque miles de personas comunes dedicaron años —a veces décadas— de sus vidas a construir algo que todos los demás pudieran usar.

* Profesores.
* Investigadores.
* Ingenieros.
* Estudiantes.
* Voluntarios.

Personas con familias, carreras y responsabilidades más allá de los proyectos que mantienen.
La civilización moderna depende silenciosamente de su generosidad.
Esa generosidad ha permitido que el código abierto florezca por más de tres décadas.
Pero la generosidad no es un recurso infinito.
A medida que el software se vuelve más complejo, el costo de entenderlo, mantenerlo y asegurarlo también crece.
Mientras tanto, la cantidad de tiempo que cada colaborador puede dedicar sigue siendo exactamente la misma.
El código abierto resolvió uno de los mayores problemas en la historia del software.
Hizo que la distribución de software fuera casi gratuita.
Nunca resolvió la sostenibilidad del software.
Si la IA de frontera realmente se convierte en una herramienta esencial para entender el software, entonces mantener la infraestructura crítica podría volverse aún más exigente de lo que es hoy.
Eso lleva a otra pregunta.

**¿Cómo sostenemos a quienes sostienen nuestra infraestructura?**

Una posible respuesta puede venir de una dirección inesperada.
Las tecnologías comúnmente agrupadas bajo el término *Web3* suelen asociarse con especulación, mercados volátiles y criptomonedas.
Esa reputación es comprensible.
Sin embargo, más allá de esas aplicaciones hay una pregunta más amplia.
¿Pueden los sistemas descentralizados ayudar a las comunidades a coordinar el mantenimiento de infraestructura crítica?
¿Puede el financiamiento volverse más transparente?
¿Puede la gobernanza volverse más resiliente?

¿Pueden los colaboradores ser recompensados de forma justa sin depender de una sola organización?

No lo sé.
Quizás la respuesta es no.
Quizás solo algunas de estas ideas sobrevivan.
O quizás tecnologías completamente distintas terminen resolviendo este problema.
Pero creo que la pregunta vale la pena hacerla.
Porque si el futuro del software depende de comunidades globales trabajando juntas, entonces también deberíamos explorar tecnologías cuyo propósito principal sea habilitar la coordinación descentralizada a gran escala.
Si Web3 se convierte en parte de ese futuro está por verse.
Ignorar la posibilidad, sin embargo, significaría ignorar uno de los pocos movimientos tecnológicos diseñados explícitamente para resolver la coordinación a escala global.
En mi opinión, Web3 solo perdurará si finalmente encuentra un propósito mayor que la especulación y la ganancia financiera.
Quizás ese propósito no sea reemplazar las instituciones existentes, sino empoderar a las comunidades para construir y sostener la infraestructura digital de la que todos dependemos.
Hay una cita de *Ratatouille* que siempre ha resonado en mí:

> *"No cualquiera puede convertirse en un gran artista, pero un gran artista puede venir de cualquier lugar."*

Si la programación es una forma de artesanía, quizás incluso un arte, entonces el mismo principio debería aplicarse al software.
Un gran desarrollador no debería necesitar pertenecer a una corporación poderosa para hacer una contribución significativa.
Solo debería necesitar la oportunidad.
Quizás el mayor desafío de la próxima generación de computación no sea construir máquinas más inteligentes.
Quizás sea construir un mundo donde cualquiera, en cualquier lugar, tenga la oportunidad de ayudar a construirlas.

# Conclusiones

Este tema nos afecta a todos.
Algunos experimentarán sus consecuencias más directamente que otros, pero nadie es completamente inmune a la dirección que está tomando la tecnología.
La historia sugiere que la humanidad se adaptará, como siempre lo ha hecho.
La pregunta no es **si** nos adaptaremos, sino **cómo**.
Quizás Glasswing se convierta en solo un breve capítulo en la historia de la inteligencia artificial.
Quizás la IA de frontera eventualmente se vuelva accesible para todos, y toda esta discusión se convierta simplemente en una curiosidad histórica.
Quizás ocurra lo opuesto, y Glasswing marque el comienzo de una era en la que la comprensión más profunda del software se vuelva cada vez más centralizada.
O quizás esa separación sea necesaria.
Quizás mantener a los sistemas más capaces bajo una custodia cuidadosa resulte ser la decisión responsable.
No lo sé.
El futuro tiene una notable tendencia a sorprendernos.
Lo que sí sé es que la tecnología nunca ha sido el objetivo final.
Las personas lo son.
Ya sea que construyamos sistemas operativos, modelos de IA, redes descentralizadas o tecnologías completamente nuevas, su valor debería finalmente medirse por una pregunta:

**¿Expanden la capacidad de la humanidad para entender, crear y colaborar?**

Si la respuesta es sí, entonces merecen ser explorados.
Si la respuesta es no, entonces deberíamos tener el coraje de repensarlos.
Este documento no es un argumento en contra de Anthropic.
Tampoco es un argumento a favor de Web3, el código abierto, o cualquier tecnología en particular.
Es un argumento por algo mucho más simple.
La comprensión no debería convertirse en un privilegio.
Debería seguir siendo una oportunidad.
Si proyectos como Glasswing, Mallana, o ideas que aún no han sido imaginadas contribuyen a ese futuro, está por verse.
Solo el tiempo lo dirá.
Hasta entonces, todo lo que podemos hacer es seguir construyendo, seguir cuestionando, y seguir dejando el mundo un poco más comprensible de lo que lo encontramos.
