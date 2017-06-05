# Capítulo 7: Administración de versiones

Cuando sigues una cobertura en vivo en un sitio web, normalmente miras la hora a la que se publicó cada post individual para ver si los periodistas todavía están actualizando la historia o si ya terminó. De esa misma forma, la gente que está considerando usar tu software quiere saber si tu proyecto todavía está vivo (si sigue mejorándose) o muerto (si ya no se actualiza).  Para ello buscarán la fecha de publicación de tu versión más reciente del programa, y una hoja de ruta que les diga cuándo y cómo planeas seguir mejorándolo.

Cuando publicas una versión nueva del programa para que otras personas la instalen y la usan, ese proceso se conoce también como "lanzar" o "empujar" una nueva versión.

El trabajo de mejoramiento de un programa puede ser lento y bastante invisible para los demás (dentro y fuera de tu redacción). Publicar y actualizar la hoja de ruta y publicar versiones nuevas le dará más visibilidad a tu trabajo, ayudará a crear un cronograma colaborativo con otras personas, y persuadirá a otras redacciones para usar tu programa.

## Números de versiones

Es casi seguro que querrás asignar [números de versiones](http://producingoss.com/en/development-cycle.html#release-numbering) a las diferentes versiones de tu programa. Esta práctica fija expectativas para tus usuarios, desarrolladores y robots, y le permite a la gente gestionar sus dependencias sin arruinar nada. Por regla general, siempre debes actualizar el número de versión del proyecto cuando actualices tu código.

Un formato de numeración común es el ["versionamiento semántico"](http://semver.org/), que usa una secuencia de tres números, como v1.5.2.

El primer número se refiere a la versión "principal" y deberá incrementarse cuando los cambios introducidos pudieran arruinar el trabajo de alguien si cambiase a la nueva versión. Por ejemplo, si estás en la versión v1.5.2 y cambias el nombre de una parte de la API, deberás incrementar la versión de v1.5.2 a v2.0.0. Esta nueva versión "principal" indicará que los usuarios no podrán acceder a la versión mejorada sin actualizar el resto del código.

El segundo número es la versión "secundaria" y deberá incrementarse cuando añadas nuevas funcionalidades sin modificar las que ya existen. Si por ejemplo añades una función nueva de asistente, deberás incrementar la versión de v1.5.2 a v1.6.0. Esto indicará que el proyecto tiene características nuevas, y que los usuarios pueden mejorar su versión sin riesgo alguno usando el mismo código que ya tienen.

El tercer número es la versión de "parche" y deberá incrementarse cuando arregles errores o refactorices las cosas por detrás del telón.

Normalmente una versión principal 0 (ej. v0.5.0) indica que el proyecto está todavía en los inicios de su desarrollo, y publicar una versión 1.0 indica que el proyecto ya es más maduro. Pero no hay reglas específicas para esto. Algunos proyectos empiezan saltando rápidamente hacia versiones más adelantadas, mientras que otros permanecen durante años como v1.0. En lugar de ponerle demasiada atención a estas reglas, mejor concéntrate en comunicar claramente en tu documentación qué es lo que ha cambiado y hacia dónde se dirige el proyecto en el futuro.

Para leer otra aproximación a la numeración de las versiones, consulta las [ideas de Jeremy Ashkenas al respecto](https://gist.github.com/jashkenas/cbd2b088e20279ae2c8e).

## Unas cuantas sugerencias profesionales para informar sobre nuevas versiones

* Después de publicar una nueva versión, verás un incremento de las preguntas y la comunicación (solicitudes de asistencia de parte de los usuarios, propuestas de asociación, preguntas sobre la posibilidad de que añadas nuevas características, etc. Es una consecuencia natural de la publicidad).

* Mantén públicamente visible una página web que indique claramente cómo acceder a las notas asociadas a la nueva versión y al paquete y al código fuente para la versión más reciente, así como instrucciones para instalarlo, y que contenga (o esté hipervinculado) a los problemas más importantes ("problemas conocidos"), ej. cosas con las que el usuario debe tener cuidado (riesgos de pérdida de datos o advertencias tipo "vas a tener que poner empeño en el paso 4").

## Hoja de ruta y planificación de versiones

¡Anuncia públicamente el estado de tu proyecto! Incluso si has decidido dejar de darle mantenimiento (ver [Capítulo 8](Capitulo08-Abandono-desactivacion.md)). Es algo que puede suceder, y está bien informárselo al mundo. Mantener a los usuarios actualizados te ayudará a pedir ayuda realmente útil de tus colaboradores:

Ejemplos de hojas de ruta:

* [Hoja de ruta de Zulip](https://zulip.readthedocs.io/en/latest/roadmap.html)

* [TAREA: más ejemplos de hojas de ruta]

De vez en cuando es buena idea conversar con algunos de tus usuarios para preguntarles qué deberías incluir en la hoja de ruta.

### Usar código abierto en tu propio medio de prensa

No dejes que la edición de código abierto de tu programa se aleje demasiado de lo que en realidad usas en tu redacción. Si lo haces, esto podría:

* Reducir los beneficios que obtienes del uso que hagan otras personas (informes de errores y parches). 

* Hacerte más torpe a la hora de mantener un buen historial utilizable.

Esto significa que por defecto deberías [usar la versión de código abierto en tu propia redacción](https://en.wikipedia.org/wiki/Eating_your_own_dog_food), y que deberías dedicarle más tiempo a tu proyecto para realizar revisiones y publicar nuevas versiones.

## Consistencia versus velocidad

Es posible que pienses que hay gente que desearía ver una versión nueva todas las semanas (y de hecho las hay). Pero si planeas seguir mejorando un proyecto, lo más importante es demostrar consistencia en la atención que le pones. Valora qué tiene más sentido para tu proyecto y para tu equipo: ¿versiones basadas en períodos de tiempo (ej. cada dos meses), o en nuevas características (tratar de terminar de incorporar una característica dada antes de lanzar la próxima versión)?

> "Las fechas de entrega no son arbitrarias: son una promesa que nos hacemos a nosotros mismos y a nuestros usuarios para poner riendas a las infinitas posibilidades que podrían incluirse en cada versión. (...) Mientras más frecuentes y habituales sean las nuevas versiones, menos importante será que contengan una característica dada. Si no se llega a incluir en esta, se incluirá en la próxima que se lance en unos meses. Cuando los lanzamientos son impredecibles o infrecuentes o demasiado espaciados, hay más presión para lograr incluir una característica más porque va a pasar mucho tiempo antes de que salga la siguiente versión. Los retrasos engendran más retrasos." - [WordPress](https://wordpress.org/about/philosophy/)

[TAREA: más estudios de casos sobre la gestión de nuevas versiones]

## Puntos a verificar

La lista de puntos a verificar para una nueva versión podría incluir:

* [ ] Higieniza secretos e información personal identificable (consulta el [Capítulo 4](Capitulo04-Primera-version.md))

* [ ] Haz un resumen de los cambios que has hecho desde la última versión (usa los registros en el sistema de control de fuente, como Git, y haz una búsqueda en tu rastreador de errores), poniendo énfasis en los cambios que solucionan vulnerabilidades de seguridad o que necesitan que tus usuarios cambien su flujo de trabajo o su configuración de software/hardware.

    * ¡USA MARCADORES! Si le asignas marcadores a los problemas y a los cambios añadidos será mucho más fácil revisar qué ha cambiado. ([Ejemplo](https://github.com/wp-cli/wp-cli/milestone/48?closed=1))

* [ ] Haz una lista de problemas conocidos importantes en esta versión en particular (vincula cada problema con el error en cuestión contenido en tu rastreador público de errores).

* [ ] Haz una lista con los nombres de todos los que colaboraron en esos cambios. Decide si esto va a incluir, para ti, la gente que participó enviando reportes de errores, contenido de la lista de correo, etc. ([Ejemplo](https://github.com/github/hub/issues/1355))

* [ ] Añade hipervínculos para que los usuarios tengan acceso a la lista completa de cambios desde la última versión

* [ ] Incrementa el número de versión

* [ ] Crea un paquete nuevo basado en la versión actual de tu código

* [ ] Publica el resumen, la lista de problemas conocidos, la lista de colaboradores y los hipervínculos (en su conjunto, las "Notas de la nueva versión") en una página web pública (como el blog de tu proyecto) y compártela con tu comunidad de usuarios (haciendo un anuncio en la lista de correos, en Twitter, etc.)

* [ ] Actualiza la hoja de ruta
