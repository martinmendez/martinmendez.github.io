---
layout: post
comments: True
title: Cultura de post mortems sin culpas
---
Cualquiera que haya trabajado con tecnología a cualquier escala está familiarizado con las fallas. Las fallas en el mundo de la tecnología no tienen en cuenta cuan buena sea la arquitectura que diseñaste, la calidad del código que escribiste o cuan bueno sea el sistema de monitoreo que implementaste. 

Las fallas simplemente suceden. Esta es una conclusión inevitable cuando se trabaja con sistemas complejos. Pero ¿qué pasa cuando las fallas han resultado debido a las acciones (o las omisiones) de los individuos? ¿Qué deberíamos hacer con esos "humanos descuidados" que causan que cada tanto tengamos un mal día?

Si la falla es grave ¿deberían ser despedidos?. O tal vez, ¿se le debería restringir el acceso a los sistemas críticos productivos?. ¿Necesitan más capacitación?

Esta es la visión tradicional del “error humano”, que se centra en las características de los individuos involucrados. Es lo que Sidney Dekker llama la “Teoría de las Manzanas podridas” - al deshacerse de las manzanas podridas, nos deshacemos del error humano. Parece sencillo, ¿verdad?.

Pues en nuestro departamento de IT no tomamos esta visión tradicional. Nosotros queremos ver esos errores, fallas, tropiezos, etc., con una perspectiva de aprendizaje. **Tener un proceso intachable de autopsias frente a las fallas es la clave de este modelo.** No importa su tamaño, fallas grandes o pequeñas.

Tomemos el ejemplo de la industria aérea. Probablemente esta industria sea la que más ha aprendido a aprender de sus fallas. Frente a cada catástrofe aérea, la industria se toma hasta años en determinar las causas de un accidente para luego retroalimentar al sistema con mejoras que terminan beneficiando la vida de otros millones de pasajeros.

Lamentablemente en general en la industria de IT (al menos en empresas tradicionales como la nuestra) estamos lejos de alcanzar esta madurez que nos ha demostrado la industria aérea. Particularmente nuestro equipo también. Pero estoy convencido de que es el único modelo posible para alcanzar un alto nivel de excelencia en los servicios que brindamos.

**¿Y dónde reside la falta de madurez?**. En la cultura, en el compromiso de cada uno de nosotros y en comprender que si sos IT (de nuevo, no importa lo que hagas), tenes una obligación con las autopsias y con la salud de nuestro monitoreo. 
Hey man !, pará! que yo no toco producción, soy developer. A esta altura, si ya has leído mis reflexiones anteriores, sabes que todos en este equipo son reponsable de producción, en especial un developer o un arquitecto que define un sistema (y que luego soporta la operación junto con el equipo de soporte de aplicaciones, ¿ya te hablé de DevOps no?).
Hey man !, pará! que yo me ocupo de distribuir paquetes. Si, pero cuando esos paquetes no llegan a las 800 PCs porque el administrador de la red hizo un mal cambio y dejó sin distribución de packages a una parte de la red, vos sos tan reponsable como el administrador de red de entender que pasó y evitar que vuelva a suceder (documentándolo en un post-mortem). Siguiendo el mismo razonamiento si sos reponsable de la distribución de parches y no estás alcanzando el 99% de compliance porque tenes en zombie el 10% de tu infraestructura de agentes de distribución y peor aún, no estás haciendo nada al respecto, entonces a eso me refiero con un problema no técnico, sino humano, cultural, de compromiso y de capacidad profesional.

Tener un **“una cultura de Post-Mortem sin culpa”** significa que los ingenieros cuyas acciones han contribuido a una falla sean capaces de dar una descripción detallada de:

Que acciones se llevaron a cabo y a que hora,
Que efectos fueron observados,
Que expectativas tenían,
Los supuestos que habían hecho,
y su comprensión de la cronología de los acontecimientos a medida que se produjeron.
Finalmente, que puedan construir un relato detallado sin temor al castigo.

¿Por qué no habrían de ser castigados o reprendidos? Debido a que un ingeniero que piensa que va a ser perjudicado por contar los hechos que condujeron a una catástrofe en un sistema es automáticamente desincentivado a dar los detalles necesarios para obtener una comprensión del mecanismo, la patología y el funcionamiento de la falla.

Esta falta de comprensión de cómo ocurrió el accidente casi garantiza que se va a volver a repetir. Si no se repite con el ingeniero original, seguro se repetirá con otro en el futuro.

Creo que este detalle es de suma importancia para mejorar la seguridad en nuestros sistemas.

Entonces, ¿que hacemos para desarrollar esta habilidad?

Alentamos a aprender teniendo intachables autopsias de análisis de las causas raíces frente a cortes, fallas o degradaciones en los sistemas.
Por cada interrupción de servicio, alentamos a realizar una autopsia que [registramos en gitlab](http://gitlab.sinopecarg.com.ar/it-all/post-mortem-reports). Esa autopsia seguramente arrojará algún plan de acción, que registramos con un set de issues en gitlab también.
El objetivo es entender profundamente cómo una falla pudo haber ocurrido, con el fin de prepararnos mejor a nosotros mismos y evitar que ocurra nuevamente en el futuro.

Buscamos “historias escondidas”, recogemos datos desde múltiples perspectivas en las fallas, y no castigamos a las personas por cometer errores.

Para poder contar con datos, primeros hay que capturarlos, por lo tanto, perseguimos un objetivo de “medir todo lo que se mueve pero con sentido”: [*meaningful alerts & monitoring*](https://www.pagerduty.com/blog/best-practices-to-make-your-metrics-meaningful-in-pagerduty/).

El párrafo anterior implica que no importa lo que hagas en IT, tu compromiso con el [monitoreo inteligente de nuestra infraestructura](http://es.slideshare.net/mrtazz/etsy-monitoring) es fundamental. No es posible operar un datacenter a ciegas; nuestras únicas herramientas preventivas para evitar catástrofes o degradaciones de servicio no es sólo un buen sistema de alertas que nos avise cuando el avión ya ha caído, por el contrario, necesitamos conocer los comportamientos de operación normal de los sistemas con los que trabajamos para poder entender cuando algo ha comenzado a comportarse en forma diferente a su patrón habitual o cuando un cambio en un ambiente ha generado una anomalía en el comportamiento habitual esperado. Eso es ingeniería de monitoreo y si hasta hoy creiste que el responsable de monitoreo era Infraestructura, bienvenido a la dura realidad, vos también lo sos. Existen pocos profesionales en el mundo de IT que comprendan la profunidad de la complejidad del monitoreo. Si trabajas administrando, diseñando o desarrollando sistemas de IT, deberías saber que existe [Monitorama](https://vimeo.com/monitorama/videos), tu mejor lugar para aprender de los que más saben.

**En síntesis, nuestra filosofía:** en lugar de castigar a los ingenieros, les damos la autoridad necesaria para mejorar la seguridad de los sistemas (en cada una de las fases del ciclo de vida de un sistema, desde el diseño hasta el abandono) y esto permite dar cuentas detalladas de sus contribuciones frente a los fracasos.

Hacemos posible y animamos a las personas que cometen errores a ser los expertos en la educación del resto de IT en como evitar esos mismos errores en el futuro. Para eso inventamos artefactos de comunicación como gitlab post-mortem, Slack o las TechTalk. Es decir, de nada sirve que escribas un hermoso post-morten si luego no te ocupas de anunciar y compartir con resto del equipo que has aprendido algo nuevo de una caída o degradación para que otros también puedan aprender. Eso también es DevOps.

Aceptamos que siempre hay un espacio discrecional donde los humanos pueden decidir tomar acciones o no, y que el momento de juzgar esas decisiones se encuentra en los procesos de retrospectiva.

Las fallas suceden. Para entender cómo ocurren, primero tenemos que entender nuestras reacciones frente el fracaso.

Una opción es asumir que la causa única es la incompetencia y gritarle a los ingenieros que “presten mas atención!” o que deben “tener más cuidado!”.
Otra opción es tomar una mirada profunda sobre como ocurrió una falla, tratar a los ingenieros involucrados con respeto, y aprender del evento.

Es por eso que quiero que tengamos intachable autopsias en IT.
