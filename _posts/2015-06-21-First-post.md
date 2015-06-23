---
layout: post
title: Here we go...
---
En los últimos 2 años, mucho me han escuchado referirme a algunos conceptos como: Lean, DevOps y Agile.

Por otro lado, también durante el mismo período mucho de estos términos se han vuelto casi una moda en ciertos ambientes de IT. Especialmente Agile en entornos de desarrollo de software y DevOps en lo que concierne a la gestión de la infraestructura y el acercamiento entre los equipos de operaciones y desarrollo.

Sin embargo, a veces no es fácil identificar cual es la relación entre ellos o que viene primero o cual es la práctica y cual es el principio.

Al igual que la práctica de Kanban, Lean proviene de los conceptos de manufactura o producción delgada desarrollados por Toyota.

Lean es un principio de mejora continua que tiene por objetivo identificar y eliminar en todo proceso productivo lo que se conoce como “desperdicio” (Muda). De acuerdo a los principios Lean, los desperdicios provienen de alguna sobrecarga en el flujo o ciclo de trabajo (Muri) o de irregularidades en el flujo mismo (Mura).

El trabajo de IT es un ciclo productivo, por lo tanto, desde hace ya unos años existe una gran tendencia en la optimización de IT a través de prácticas Lean. De hecho Kanban es una de ellas.

El único objetivo que tiene Lean es lograr ciclos productivos que sean capaces de entregar el máximo valor al cliente utilizando para ello los mínimos recursos necesarios (delgado o ajustado).

Lean se focaliza en eliminar 8 clases de desperdicios:
* Sobreproducción.
* Tiempo de espera
* Transporte
* Exceso de procesados
* Inventarios
* Procesamiento inapropiado
* Defectos
* Potencial humano subutilizado

Eliminando el desperdicio, mejora la calidad y se reducen el tiempo de producción y el costo. Las herramientas lean (en inglés, ‘ágil’, ‘esbelto’ o ‘sin grasa’) incluyen procesos continuos de análisis (llamadas kaizen en japonés), producción pull (‘disuasión e incentivo’, en el sentido del término japonés kanban), y elementos y procesos «a prueba de fallos» (poka yoke, en japonés), todo desde el genba japonés o área de valor o sea el lugar donde el cliente consume el material o servicio que se le entrega desde la cadena de producción.

Lean se focaliza en optimizar el proceso productivo de extremo a extremo que crea valor para los clientes - desde la idea inicial hasta la recogida de los beneficios que pueda entregar dicho proceso productivo.

Los principios Lean se centran en la optimización del flujo más que cualquier otra cosa: identificar los cuellos de botella en el proceso que deben ser retirados y actividades que generan desperdicios y que necesitan ser identificadas y evitadas.

Todo muy lindo Martín, ¿pero dónde están esos 8 desperdicios en IT?, bueno, déjame darte algunos ejemplos:

**Sobreproducción:** hacer más de lo necesario en forma temprana. Muy evidente en el desarrollo de software, desarrollar más funcionalidades que las que el cliente realmente necesita (incluso cuando él sea quien las pide). Otro ejemplo de sobreproducción en IT, instalar aplicaciones que son abandonadas o poco usadas y que igualmente tenemos que mantener; hacer complejos desarrollos BI para uno o dos usuarios sin tener claro si hay un real impacto de valor en la organización; hacer abusos en el uso o mal uso de herramientas de IT que obligan a un escalabilidad innecesaria.

**Reprocesamiento o exceso de procesados:** un clásico en IT y si no le preguntan a Javier con BI. Reiteradas idas y vueltas entre el desarrollador y el cliente debido a que la especificación está llena de inconsistencias o incertidumbres.

**Tiempo de espera:** otro clásico de IT. Estamos plagados de tiempos de espera y generamos otros cientos tiempos de esperas dentro del equipo y a nuestros clientes. Interrupciones asociadas con la toma de decisiones, ausentes o malas especificaciones, procesos de cambios que obligan a detenernos a la espera de una ventana de cambio, dependencias entre los equipos de IT que no son tenidas en cuenta y generan tiempos de espera (ej. necesito un servidor y se lo tengo que pedir a infraestructura). Clientes esperando semanas o meses por falencias en la gestión del inventario.

**Inventarios:** cualquier acumulación que genere IT a la espera de algún procesamiento o solución son potenciales generadores de desperdicio que atentan a la eficiencia del ciclo productivo. Funcionalidades a la espera de ser implementadas, backlog de tickets no resueltos con usuarios en espera de ser atendidos. Inventario de alertas y errores en fallas de procesamientos nocturnos que deben ser reprocesados nuevamente al día siguiente en forma manual.

**Transporte:** cualquier flujo de información que pase entre varios intermediarios con el riesgo de mala interpretación es un potencial generador de desperdicios. El “ticket volador” que da vueltas por diferentes grupos de resolución dentro de IT hasta encontrar quien realmente lo resuelve es otro ejemplo de desperdicio de transporte.

**Defecto:** todo defecto es un desperdicio por definición pues introduce falencias en cualquier proceso productivo, re-trabajo y tiempos de espera. Cualquier falla en un sistema es un desperdicio.

**Procesamiento inapropiado:** existen varios ejemplos en IT sobre este desperdicio, uno típico que aplica a Help Desk o mesas de ayuda es cada ticket mal resuelto que es reclamado por el usuario y que debe ser vuelto a procesar generando re-trabajo. La ausencia de análisis de causas raíces (se acuerdan de Post Mortem sin culpa?) generar la repetición de fallas que obligan a IT a atender el mismo problema más de una vez en forma sucesiva.

**Potencial humano subutilizado:** todo componente del proceso productivo que trabaje subutilizado (incluso por cuestiones de conocimiento) es un desperdicio que debería evitarse. Todo conocimiento no capturado que obligue a generarlo cada vez que sea necesario, es desperdicio.

Lean es toda una cultura de mejora continua, centrada en el flujo más que en cualquier otra cosa. Se base en descubrir cuellos de botellas en forma permanente y desperdicios y removerlos. Solo cuando todos los involucrados en el proceso (en nuestro caso todo IT) se involucran seriamente en este modo de pensar existen los pilares para desarrollar prácticas como Kanban, Agile o DevOps.

**¿Y por qué son importantes estas prácticas en IT?**

Principalmente porque nos otorgan dos cosas: escalabilidad a mismo o menor costo y un ataque directo a la entropía generada por las problemáticas del crecimiento que comentaba antes en la sección de “Los comienzos”.

**¿Y como se implementan?**

Transformando nuestra cultura, nuestras reuniones, nuestras prácticas habituales hacia una mirada crítica permanente de cómo hacemos las cosas, cuales son nuestros cuellos de botellas y cuales actividades no aportan real valor por grandes o pequeñas que sean.

**DevOps: la parte soft**

Desde que comenzó a sonar el término DevOps se ha dicho incansablemente que se fundamenta en la capacidad de comunicación y colaboración de los equipos. Estoy muy de acuerdo con esa idea y creo que por ello también es muy difícil darle una definición clara al término DevOps. Estas capacidades de los equipos no son cosas que se puedan graficar, que suelen ser difíciles de medir pero que funcionan como abono de una tierra fértil para que un montón de nuevas cuestiones técnicas puedan suceder en los equipos de IT.

Entonces, ¿qué queremos decir que estas cosas son centrales para desarrollar una cultura DevOps? Comunicación? Tenemos correo electrónico, mensajería instantánea, control de versiones, sistema de tickets, mil formas de comunicarnos. Así que nos comunicamos, ¿verdad? ¿Colaborar sobre qué?.

Vamos a dejar estas dudas un poco de lado y vayamos a un ejemplo.

Tu eres un desarrollador y estamos por lanzar una nueva funcionalidad en el Portal de Proveedores. En este punto los desarrolladores maduros se comienzan a hacer algunas preguntas:

¿Qué podría salir mal con esta funcionalidad?

¿Cuáles son sus modos de fallo?

¿Qué indicadores o alertas nos dirán que algo anda mal?

¿Qué umbrales de métricas serán las adecuadas?

¿Si debo despertar a alguien? ¿qué tiene que hacer? ¿cómo debe proceder?

¿Qué indicadores nos dirán que todo funciona adecuadamente?

¿Cómo vamos a manejar los fallos cuando se producen?

¿Confío realmente en mi diseño? ¿Confío en los recursos sobre el cual está montado?

¿El failover soportará esta nueva funcionalidad?

¿Generaré algún impacto no previsto?

¿Cómo vuelvo atrás? ¿con qué esfuerzo?

…

Y por supuesto la mejor:

¿Cómo puedo cubrir adecuadamente todas estas preocupaciones y aún así construir la funcionalidad requerida en un período de tiempo razonable para que tenga valor para el negocio?

Todas estas preguntas son oportunidades para una buena comunicación y colaboración entre desarrollo y operaciones. Hay un montón de lugares donde el código golpea el metal, donde los  comportamiento hacen sonar las alarmas, y en el que lo "normal" reúne las condiciones de "contingencia".

¿Quiénes van a tener esas conversaciones? Lo ideal es que tanto desarrolladores y operaciones ataquen el problema aportando su propia experiencia y perspectivas pero en forma conjunta. Y lo ideal, todas las perspectivas tendrán el mismo peso en acercar una una solución que cubra las cuestiones de disponibilidad, rendimiento, escalabilidad, confiabilidad y facilidad de mantenimiento, teniendo todo en cuenta al mismo tiempo.

Esa es la colaboración de la que estoy hablando.

Los mejores chicos “ops” que conozco entienden el valor de conseguir funcionalidades en producción en un tiempo razonable, y quieren ayudar a ese proceso en todo lo que puedan.

Los mejores desarrolladores que conozco entienden lo que significa construir una función que sea la vez operable y fácil de mantener en producción, y también están abiertos a sugerencias sobre cómo hacerlo adecuadamente.

Y los mejores equipos conocen ambos los límites de sus perspectivas tradicionales, porque han logrado hablar y aprender entre sí todo el tiempo.

Imaginen ahora como se vería un comité de cambios donde en lugar de ser un interrogatorio del tipo: ¿tenes el ok del usuario? ¿analizaste el impacto? ¿documentaste?, etc etc, tanto el desarrollador junto con alguien de infraestructura presenten sus “respuestas DevOps” frente a un pasaje a producción.

DevOps no es Puppet, Chef, Ansible, SCCM, Jenkins, NewRelic, Leankit o scripting. Todas esas son herramientas que se suceden en forma natural como respuesta a una filosofía de trabajo que intenta en forma continua evitar desperdicios, que evita hacer las cosas mas de una vez, que pretende disponer de métricas para la toma de decisiones inteligente. Sin el mindset previo, sin que el equipo no desarrolle la filosofía requerida, los resultados siempre serán limitados (como nuestro caso testigo de Kanban, aunque de nuevo, no podemos despreciar todo el aprendizaje que el intento nos deja).

DevOps al igual que Lean es una filosofía que refunda los principios organizativos de cualquier área de IT.
