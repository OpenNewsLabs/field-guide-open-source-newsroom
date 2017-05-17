# Capítulo 8: Abandono y desactivación

**Hello darkness, my old friend**

![](https://media.opennews.org/fieldguides/open-sourcing/yorick.jpg)

Es casi seguro que tendrás que separarte de tu proyecto. Es una parte perfectamente natural del ciclo de vida del código abierto, y no deberías sentirte mal por eso. Ahora bien, que sea normal no significa que vaya a ser fácil. Los finales no se escriben por sí solos, y los preparativos para ese momento se asemejan mucho escribir un testamento: no es agradable, pero hará que una circunstancia difícil sea mucho más llevadera si puedes prepararte para ella con antelación. Si no pones fin abiertamente a tu proyecto o te separas de él, puedes dejar a tus usuarios actuales y futuros en la oscuridad. Esto puede causar confusión o generar desconfianza hacia tu proyecto o tu organización. Piensa en todo el trabajo que invertiste en levantar el proyecto desde los cimientos; desactivarlo va a llevar más o menos el mismo esfuerzo, probablemente más. Pero no hay que temer: planificar la sucesión puede cambiar completamente la transición y hacerla más fácil. 

## Por qué abandonar del proyecto

Cualquiera que empieza un proyecto de código abierto probablemente necesitará ponerle fin, o al menos desvincularse de él. ¿Es normal estar enamoradísim@ del proyecto al principio, y luego ya no tener tiempo, o interés...  y hasta llegar a tomarle mala voluntad? Sí. Sí. Positivo. Algunas razones que podrían hacerte abandonar el proyecto: 

* Ya no tienes tiempo para dedicarle. Por ejemplo, te has retirado del desarrollo de software y ahora administras una granja bovina en Wisconsin.

* Tus necesidades originales han cambiado. Por ejemplo, ya no necesitas un scraper para extraer datos del archivo de la Comisión Federal Electoral porque te has pasado al departamento que asigna a los lectores a diferentes casas en Hogwarts. 

* Un grupo grande de colaboradores se está encargando de la mayor parte del proyecto y te gustaría traspasarles el control a ellos.

* Ya no te da alegría. Te ha agotado y necesitas delegar un poco de responsabilidades. Tienes pull requests sin evaluar. Tienes tickets abiertos y no quieres cerrarlos. Ya no usas el proyecto.

## ¿Qué camino tomar?

![](https://media.opennews.org/fieldguides/open-sourcing/telnet.gif)

Hay tres caminos que puedes tomar para separarte de un proyecto de código abierto. 

* Puedes entregarle el proyecto a otras personas que se encargarán de mantenerlo. 

* Puedes archivar o preservar el proyecto para los arqueólogos informáticos del futuro. 

* Puedes retirar tu proyecto de internet, o sea, eliminarlo. 

## ¿Cómo decidir qué camino elegir?

¿Tienes gente que pueda servir de relevo? Valora traspasarles el control del proyecto, especialmente si deseas que el público pueda seguir usándolo.

¿Crees que alguien podría beneficiarse de tu aproximación al problema que querías resolver, incluso si la solución no fue óptima? Valora preservar o archivar tu proyecto. Puedes aclarar que el proyecto ya no está recibiendo mantenimiento pero invitar a la gente a bifurcarlo, siempre y cuando no sea peligroso usar el programa.

¿El proyecto puede ser perjudicial para ti o para quienes lo usen o lean sobre él? Puede que quieras retirarlo de internet, en especial si no quieres que se te siga asociando con él.

Solo el primer camino significa que tu proyecto va a seguir actualizándose/recibiendo mantenimiento.

> Algunas razones por las que no valdría la pena actualizar o mantener tu proyecto:

> * Cuesta más que lo que vale, ya sea mantenerlo o gestionar la comunidad o darle publicidad.

> * Tú o tus usuarios han decidido usar otra herramienta. Por ejemplo, Kenneth Reitz ha lanzado FECless.py, Datos para humanos de la Comisión Federal Electoral, que es mucho mejor que tu serie de scripts de código abierto en Perl.

> * Uno de los supuestos que sustentaba el proyecto ha cambiado considerablemente, o una parte del proceso, por ejemplo, la FEC tiene una API nueva que deja sin sentido tu scraper.

## Avanzar por el camino elegido

He aquí más información sobre los tres caminos a tomar a medida que tu proyecto muere o tu participación finaliza. 

### Traspasar el control de tu proyecto

![](https://media.opennews.org/fieldguides/open-sourcing/handoff.gif)

Si tu proyecto es popular y tiene una comunidad activa a su alrededor, la mejor opción es un cambio de liderazgo. Si no tiene mucho uso, no te preocupes: salta directamente a la sección **archivar tu proyecto** o **enterrar tu proyecto**.

#### Elegir una nueva dirección

En dependencia del nivel de participación de la comunidad, puede que ya tengas colaboradores muy activos que hayan tomado la batuta.  Esos serán los mejores candidatos para reemplazarte. 

Si no tienes gente así en tu comunidad, entonces puede ser difícil encontrar a alguien.  Puedes usar el foro, lista, chat u otro canal que uses para comunicarte con tus usuarios y colaboradores para anunciar que se necesita a alguien que asuma la dirección del proyecto.  Una consideración importante es si confías en que el trabajo de tu relevo va a estar a la altura del tuyo. Al final, hacerles entrega del proyecto (cuando está ligado a ti y a tu organización) puede interpretarse como un acto de confianza.

#### Establecer las expectativas para la nueva administración

Al discutir el traspaso con los nuevos encargados, es importante comunicar las expectativas de lo que significa dirigir el proyecto. Y si has seguido las directrices de los capítulos anteriores, la mayoría de estas cosas ya estarán establecidas en la documentación y dentro de la comunidad.

Normalmente es muy fácil comunicar la mecánica de programación y del proyecto. Aunque es más difícil, más importante aún es comunicar el espíritu del proyecto y de tu liderazgo.

#### Elementos a discutir con la nueva dirección

* La meta prioritaria del proyecto

* Quién es la audiencia  

* Código de conducta

* Resolución de conflictos

* Filosofía del proyecto

#### Comunícate con tus usuarios

Con la nueva dirección es probable que haya cambios, y es importante comunicar esos cambios, o la ausencia de ellos, a la gente que usa tu proyecto. Asegúrate de explicar los cambios a tus usuarios con toda la antelación posible. Envía notificaciones varias veces como recordatorio sin que la frecuencia sea tanta que lleguen a molestar.  Y cada vez que puedas envía notificaciones por varios canales.

#### Lo que debes entregar

El traspaso del control tiene su mecánica, centrada principalmente en el acceso, la propiedad del programa y los recursos del proyecto.  Estos elementos pueden dividirse entre varias personas, o ser ya responsabilidad de alguien más.

* Propiedad del repositorio

* Propiedad de los canales de comunicación, por ejemplo, Slack, listas de correo, cuentas de Twitter

* Claves de los servidores

* Propiedad intelectual, de los logos, por ejemplo

### Archivar tu proyecto

![](https://media.opennews.org/fieldguides/open-sourcing/indy.gif)

Si no hay un grupo natural para relevarte, puedes considerar archivar el proyecto.  La tarea principal al archivar un proyecto es la comunicación.

#### ¿Qué necesito comunicarles a los usuarios actuales?

* Debes explicar que ya no se actualizará más el proyecto.

* Debes invitarlos a bifurcar el proyecto si hay características esperando a ser implementadas.

* Debes indicarles si existen otros proyectos alternativos. 

#### ¿Qué necesito comunicarles a los usuarios futuros?

* Diles: "Lo que ven es lo que hay."

* Si hay una cuenta en Twitter, fija un tuit al inicio del perfil que explique el estado del proyecto.

* [TAREA: más principios de comunicación]

#### ¿Cómo muestro que el proyecto ya no tiene mantenimiento?

* Actualiza el README con información clara sobre el estado del proyecto:

    * [Insignias](https://github.com/badges/stability-badges)

    * Mediante un mensaje como "Este proyecto ya no recibe mantenimiento"

    * Indica las consecuencias de la falta de mantenimiento, por ejemplo, puede que no se instale correctamente, que devuelva datos corruptos, etc.

* Python: En Pypi, fija el estado de desarrollo en 7 -- Inactivo

* Python: [Cómo depreciar un módulo](https://www.python.org/dev/peps/pep-0004/)

* Ruby: [Herramientas para depreciación](https://www.ruby-toolbox.com/categories/Deprecation_Tools) (es irónico que una de las herramientas de depreciación más usadas en Ruby haya sido abandonada)

* [TAREA: más consejos para otros lenguajes y plataformas]

### Enterrar tu proyecto

![](https://media.opennews.org/fieldguides/open-sourcing/yeller.gif)

En algunos casos, puede que decidas retirar tu programa de internet.  A continuación algunas cosas a considerar antes de tomar la decisión.

#### ¿Debería simplemente archivar mi proyecto?

Si respondes que sí a cualquiera de estas preguntas, entonces es posible que quieras archivarlo.

* ¿Hay gente usando el proyecto?

* ¿Está vinculado a un administrador de paquetes y se usa desde ahí?

* ¿Es útil como ejemplo o para otro propósito educativo?

* ¿Es importante para ti y tu organización por cuestiones de transparencia?

* ¿Puede servir como advertencia para otras personas?

#### ¿Por qué querría enterrar mi proyecto?

Si no respondiste que sí a ninguna de las preguntas anteriores, entonces puedes considerar enterrar tu programa. He aquí una lista de cuestiones a considerar:

* ¿Ya no quieres que se te asocie con el programa?

* ¿Tu organización quiere que el proyecto muera, quizás por cuestiones de derechos de autor?

* ¿El proyecto es dañino, o no tiene valor como se describió anteriormente?

#### Retirar tu proyecto de administradores de paquetes populares

<table>
  <tr>
    <td>Lenguaje</td>
    <td>Administrador de paquetes</td>
    <td>Comando</td>
    <td>Link</td>
  </tr>
  <tr>
    <td>Python</td>
    <td>PyPi</td>
    <td></td>
    <td>[Retirar un paquete de PyPi](http://stackoverflow.com/questions/20403387/how-to-remove-a-package-from-pypi)</td>
  </tr>
  <tr>
    <td>Node.js</td>
    <td>NPM</td>
    <td>npm unpublish</td>
    <td>[Despublicar](https://docs.npmjs.com/cli/unpublish)</td>
  </tr>
  <tr>
    <td>Ruby</td>
    <td>Ruby Gems</td>
    <td>gem yank</td>
    <td>[gem yank](http://blog.rubygems.org/2015/04/13/permadelete-on-yank.html)</td>
  </tr>
</table>


## Esta es la forma que ha tomado nuestro dolor

A continuación algunos ejemplos de cómo algunos desarrolladores han abandonado o traspasado sus programas.

## Estudio de caso:

[TAREA: estudio de caso de CSVKit]

## Estudio de caso:

[TAREA: estudio de caso de Sunlight Foundation]

## Estudio de caso:

[TAREA: estudio de caso de ProPublica]

## Ya pasó

![](https://media.opennews.org/fieldguides/open-sourcing/sunset.gif)

Ahora que has traspasado tu proyecto, tómate un momento para sentirte bien por el buen trabajo realizado y por todo lo bueno que puedes hacer en el futuro.  

Puede que te sientas culpable o irresponsable por abandonar un proyecto, especialmente si es uno de tus primeros, o uno en el que estuviste muy involucrad@, pero no desmayes. Esto pasa todo el tiempo, y el mundo sigue su curso.

### Estudios de casos

> El proyecto de Burton Street (2009) funcionó gracias a las alianzas y colaboraciones que surgieron a pesar de los recursos limitados del medio de prensa que lo creó.  Pero esta misma estructura colaborativa fue lo que lo hizo inestable a la larga.  Como un año después de que el proyecto ganara premios, algunos desarrolladores se acercaron al periódico para usar el código para crear algo parecido en un barrio que estaba lidiando con una situación similar, más al este en Carolina del Norte. Aunque la publicación estuvo de acuerdo, las circunstancias personales de los desarrolladores cambiaron, y el proyecto tambaleó. El periódico retuvo el código, y el proyecto se alojó en su sitio, a pesar de las promesas de liberar el código públicamente para cualquiera que quisiera usarlo.

> En 2014, el proyecto Burton Street desapareció completamente del sitio web del periódico, en medio de la vorágine de un rediseño. Esto pasó después de un período caótico en la redacción por deficiencias administrativas, cuando ya el equipo que había creado el proyecto originalmente había entregado el programa al periódico. El proyecto, y el código que lo hizo posible, se perdieron completamente porque no había una forma clara de preservarlo o entregárselo a otra entidad.

> La lección: Una planificación más clara del carácter abierto del proyecto hubiese marcado una gran diferencia. Mientras que algunos proyectos tienen finales naturales, este pudo haber sido mucho más útil durante mucho más tiempo. Ayudó a proporcionar una plataforma directa a un área marginada en Asheville y pudo haber servido igual en muchos otros lugares. Su final fue prematuro y no a causa de ningún plan intencional, sino por pura negligencia, planificación deficiente y falta de prioridades claras. Esto es lo que puede pasar cuando no se tiene un plan claro de abandono/desactivación.

> Para saber más sobre cómo el proyecto Burton Street usó la colaboración de varios grupos para acometer un proyecto con recursos limitados, consulta el [Capítulo 1](es/Capitulo01-Optar-por-codigo-abierto.md). > Para leer más sobre el proyecto como un ejemplo de comunicación comunitaria, consulta el [Capítulo 6](Capitulo06-Comunidad.md).
