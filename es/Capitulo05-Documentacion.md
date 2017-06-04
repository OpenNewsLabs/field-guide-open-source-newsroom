# Capítulo 5: Documentación

![](https://media.opennews.org/fieldguides/open-sourcing/why.gif)

La mayoría de los desarrolladores se ha visto en la posición de tener que actualizar o mejorar un proyecto que ya existe, para descubrir rápidamente el costo de tener que dilucidar cómo es que funciona el código. La documentación asociada a un programa es esencial para reducir ese costo, y muchos reconocemos que incluso trabajar con código escrito por nosotros mismos un tiempo atrás puede sentirse como si estuviéramos trabajando con código escrito por otra persona.

La documentación es como un manual de usuario para tu proyecto: explica cuándo usarlo, cómo usarlo y cómo arreglarlo si se rompe. También pude incluir información sobre cómo contribuir al proyecto o cómo comunicarse para hacer preguntas.

Una buena documentación es la mejor manera de convencer a los demás de que usen tu producto porque quita las barreras para acceder al programa y les da independencia a los usuarios para resolver problemas por sí mismos. Debe estar contenida en un archivo navegable, para que sea fácil encontrar los temas que incluye incluso cuando no esté muy bien organizada. No necesita ser perfecta para poder usarla.

También podemos encontrar documentación en lugares menos comunes. Por ejemplo, los comentarios incluidos en el código son un tipo de documentación.

El proceso de escritura de la documentación también puede ser una forma útil de asegurar la calidad de tu programa. Revisar los componentes del proyecto y los casos de uso te da la oportunidad de detectar debilidades en tu código. Piénsalo como una forma de ayudarte a ti mism@ en el futuro, y a todo aquel que use tu programa.

## Cómo dar los primeros pasos

Antes de empezar a documentar tu proyecto puede resultar útil responder estas preguntas:

*Qué:*

Uno de los pasos iniciales en la documentación es definir su alcance: qué se va a documentar, que escapa de sus límites y dónde puede encontrarse más información sobre los temas que no cubre, cuál es el nivel de detalles correcto, etc.

*Dónde:*

Hay muchas opciones de hábitat para la documentación de tu proyecto: GitHub, el sitio web del proyecto, [Read the Docs](https://readthedocs.org/), etc. Aquí un ejemplo de [Tarbell en Read the Docs](http://tarbell.readthedocs.io/en/latest/).

[TAREA: más sobre el alojamiento de la documentación]

*Quién:*

La audiencia de tu proyecto podría ir más allá de los usuarios. Podría incluir editores o administrativos que estén evaluando el proyecto para uso futuro, o desarrolladores interesados en colaborar. Identificar a tu audiencia te ayudará a moldear el uso de términos técnicos y ejemplos.

Aquí algunos elementos a tener en cuenta:

* **Siempre es mejor definir las expectativas lo más temprano posible**—en la vida y en tu proyecto de código abierto. De entrada, tu documentación debería responder a la pregunta: "¿Qué necesito saber para usar este proyecto?" También es útil incluir un estimado del tiempo que crees que tomará echarlo a andar. [Aquí](https://pantheon.io/blog/still-maintained) un ejemplo.

* **Evita usar vocabulario técnico, y si lo haces, explícalo.** Incluye enlaces a la documentación de las dependencias, las librerías externas y los términos técnicos. Un glosario (ej. [el glosario de Github](https://help.github.com/articles/github-glossary/)) también puede evitarte tener que explicar la terminología. Siempre es buena práctica evitar usar chistes internos y referencias culturales muy enrevesadas que no todo el mundo va a comprender. Por ejemplo, aunque las referencias a *The Big Bang Theory* le den un toque refrescante a tu documentación para los fans de ese show, resultarán confusas para quienes no lo hayan visto. Eso no significa que los ejemplos y la documentación tengan que ser secos, pero es importante no perder de vista a la audiencia.

* **Piensa en todas las necesidades de la comunidad.** Una buena documentación reconoce que la audiencia tiene diferentes niveles de necesidad de detalles. Algo que podría resultar útil es identificar diferentes grupos de audiencia y separarlos a la hora de preparar la documentación. Por ejemplo, podrías separar en secciones diferentes la información para usuarios y para administradores (ej. [Proyecto Panda](http://pandaproject.net/docs/)).

* **Recomienda una Infraestructura.** Ejecutar código en tu máquina de desarrollo es muy diferente a ejecutarlo en fase de producción. Sería útil incluir una sección aparte dedicada a la infraestructura que se recomienda, despliegue de código, puesta en marcha de la caché, etc. Para ver un ejemplo de esto, consulta el [Proyecto Kinto](http://kinto.readthedocs.io/en/stable/configuration/production.html).

* **Especifica los prerrequisitos.** Si tienes prerrequisitos muy específicos para tu proyecto, describe la forma de consultarlos, y no asumas que el lector conoce la configuración de su propia máquina. (Por ejemplo, si necesitas una versión particular de la libraría instalada y tu script de configuración no puede con ella, documenta cómo revisar eso.)

Aquí otras notas sobre cómo manejar la documentación:

* **Que sea específica, pero asequible y atractiva** y no des por sentado demasiadas cosas sobre los posibles colaboradores y sus niveles de habilidades (o expón esas suposiciones).

* **Recuerda que tu proyecto no es exclusivamente de programación**, y que la gente puede contribuir de otras formas, por ejemplo, aportar ideas y perspectivas.

### Escribe un README

Un punto de partida común para la documentación es un archivo README (LÉEME) ubicado en la raíz del proyecto con información para que los usuarios puedan empezar a usar el programa. Suele ser un archivo Markdown (un tipo de formato de texto del que hablaremos más adelante) o un archivo de texto simple.

Generalmente, todo proyecto de código abierto debe incluir un README. Es lo primero que leerá la mayoría de los desarrolladores para familiarizarse con un proyecto. (Y si estás iniciándote en código abierto, leer los README de otros proyectos es un muy buen primer paso).

He aquí la información que generalmente contienen estos archivos:

1. Qué es el proyecto y qué hace

2. Cómo instalarlo

3. Cómo ejecutarlo

4. Cuáles son los planes futuros y cómo colaborar

5. Créditos y referencias

Este [artículo](http://dpb.bitbucket.org/what-goes-in-a-readme.html) de David Prager Branner es una excelente guía breve para escribir un buen README. No hay un único estándar para los README, pero al menos tocar la información enumerada anteriormente ayuda.

> Muchos proyectos usan Markdown, un lenguaje ligero de formateo de texto, para darle estructura semántica a sus README. Para empezar a usar Markdown, consulta esta [guía de Github](https://guides.github.com/features/mastering-markdown/).  Es recomendable cambiar el nombre de tu README a README.md si estás usando Markdown, ya que servicios como Github interpretarán y mostrarán mejor el contenido.

Sin embargo, no hay una regla rígida que diga que tu documentación tiene que estar en un archivo README. Simplemente piensa en el README como un punto de partida para la información que necesitarán los usuarios. Algunos proyectos alojan su documentación en el sitio web del proyecto o en un sitio como [Read the Docs](https://readthedocs.org/), que proporciona organización y buscabilidad. Sin embargo, si vas a alojar tu documentación en otro lugar, es recomendable que incluyas un vínculo a ella en tu README. La librería [agate](https://github.com/wireservice/agate) es un buen ejemplo de un proyecto con un README mínimo hipervinculado a la información más importante del proyecto.

### Crea un archivo CONTRIBUTING.md

Este archivo explica cómo la gente puede colaborar con tu proyecto. Sitúalo en lo más alto de la jerarquía de tu repositorio. Aquí [algunos ejemplos](https://github.com/nayafia/contributing-template).

Un gran beneficio de esta perspectiva al usar GitHub es que [GitHub añadirá un vínculo](https://github.com/blog/1184-contributing-guidelines) a este documento cuando alguien añada un problema o envíe un pull request. ([Ejemplo](https://github.com/swcarpentry/git-novice/blob/gh-pages/CONTRIBUTING.md))

### Usa los comentarios sabiamente

La documentación del proyecto cae en tres categorías: documentación para ti mism@, documentación para otras personas que estén trabajando en el mismo proyecto, y documentación para cualquiera que desee usar tu código.

La mejor opción para la tuya son los comentarios insertados en el código y buenos nombres de variables. Todo desarrollador se ha preguntado al menos una vez al ver un trabajo propio pasado: "¿En qué estaba pensando yo cuando escribí esto?" Tu yo futuro te agradecerá el tiempo que dediques a incluir comentarios en el código.

Además de explicar el "qué", los mejores mensajes que se incluyen al añadir código a un repositorio son los que explican el "porqué". No dependen de que recuerdes el contexto ni repiten lo mismo que hace el código sin añadir ninguna información adicional. He aquí un ejemplo de comentarios en función de documentación:

```
// Mal comentario
// Se divide el tiempo entre 24.623 y se convierte a entero
var dias = parseInt(tiempo / 24.623);

// Comentario y código mejor escritos
const HORAS_DIA_MARCIANO = 24.623;
// Calcula la cantidad de días completos en Marte
var diasEnMarte = parseInt(tiempoTranscurridoEnMarte / HORAS_DIA_MARCIANO);
```

Los comentarios también ayudan a las demás personas que están trabajando contigo en la base de código a usarla mejor. Se pueden usar para establecer directrices claras de reutilización del código y fijar las expectativas a un nivel granular en el programa.

Puede que sea más cómodo escribir comentarios muy breves sobre tu código, pero asegúrate de que sean lo suficientemente descriptivos como para resultar útiles a alguien que no esté familiarizad@ con el proyecto. Por ejemplo, puede que quieras escribir como comentario `// función de subdivisión`, pero eso no dice mucho. Un comentario breve como `// subdivide una cadena de caracteres introducida por el usuario en nombre y apellido` será más útil para quienes traten de entender tu código.

### Prepara tu infraestructura para varios idiomas

Escribir la documentación en varios idiomas incrementará el alcance de tu proyecto. Pero la mayoría de nosotros no hablamos más que un par de idiomas como mucho. Documenta cómo alguien puede aportar documentación en otro idioma.

## Ejemplos y tutoriales

Las especificaciones integrales de API pueden ser útiles al tratar de depurar errores o realizar otras tareas específicas, pero no sirven muy bien de punto de partida para usuarios no familiarizados con tu código. Las aplicaciones prácticas reales de tu proyecto le pueden dar a los usuarios una idea de lo que puede hacer tu herramienta y los familiariza con el funcionamiento de tu programa.

Algunos proyectos, como [csvkit](https://csvkit.readthedocs.io/en/540/tutorial/1_getting_started.html), incluyen tutoriales introductorios sencillos. Otros, como [d3](https://github.com/d3/d3/wiki/Gallery), pueden incluir una lista de posibles casos junto al código que los hace funcionar. Elex ofrece [algunos ejemplos](http://elex.readthedocs.io/en/stable/index.html) de diferentes niveles de complejidad: un [tutorial introductorio](http://elex.readthedocs.io/en/stable/tutorial.html), ["recetas" breves de código](http://elex.readthedocs.io/en/stable/recipes.html) para patrones de uso comunes y vínculos a [implementaciones](http://elex.readthedocs.io/en/stable/index.html#elex-projects-and-implementations) completamente desarrolladas.

### Mejores prácticas para código de muestra

Los mejores ejemplos suelen ilustrar un solo concepto o mostrar claramente los pasos individuales de un proceso. Recomendamos describir el objetivo o el resultado que se espera obtener al inicio del código de muestra, como en este [tutorial de jsFiddle](http://doc.jsfiddle.net/tutorial.html#first-fiddle-hello-world-goodbye-world).

El código de muestra debe ser fácil de ejecutar para los usuarios, y los datos y recursos que se usen en él también deben ser fáciles de obtener. Muchos repositorios de código abierto incluyen [archivos de muestra](https://github.com/nprapps/mapturner/tree/master/examples) para que los usuarios no tengan que buscar recursos por su cuenta. 

Cuando un proyecto tiene una configuración complicada o necesita de la compra de licencias externas, poner un servidor de demostración a disposición de los posibles usuarios les permite probarlo antes de decidir invertir en él su tiempo y dinero. Cuando Vox Media incorporó un servidor de prueba para [Autotune](https://github.com/voxmedia/autotune), observaron un incremento del interés en el proyecto. 

Un servidor de prueba (demo) como el de Mozilla para su [proyecto Kinto](http://kinto.readthedocs.io/en/stable/tutorials/first-steps.html) puede facilitar la escritura de código de muestra para puntos de entrada de la API que los usuarios pueden ejecutar fácilmente. Otros ejemplos semejantes: [Zulip](https://github.com/zulip/zulip-gci/blob/master/request-remote-dev.md) y [Dreamwidth](http://hack.dreamwidth.net/) ofrecen instalaciones remotas para los nuevos colaboradores de forma gratuita.

### ¿Cómo decido qué ejemplos mostrar?

Es imposible prever y documentar todos los casos de uso de tu proyecto. La clave está en construir cimientos que sean suficientes para que los usuarios nuevos puedan empezar a trabajar. Comienza describiendo un caso de uso típico de tu proyecto. [Census Reporter](https://github.com/censusreporter/censusreporter#getting-data-from-our-api-the-basics) prevé cuáles serán algunos de los puntos de entrada más usados de su API y describe cómo construir variaciones de las consultas.

No temas invitar a tu base de usuarios a contribuir con sus propios ejemplos también. La [galería de muestra de d3.js](https://github.com/d3/d3/wiki/Gallery) incluye cientos de ejemplos creados por usuarios y cubre varios temas, conceptos y niveles de experiencia.

## Testear tu documentación

Si tienes tiempo y recursos, puedes realizar algunas pruebas para determinar qué ejemplos sería más útil mostrar. Los desarrolladores de una herramienta en el Washington Post escribieron un borrador inicial de la documentación y se dedicaron a observar el uso que sus "testeadores beta" hacían de la documentación para realizar determinadas tareas. Esto reveló diferentes suposiciones hechas por los usuarios y casos de uso que pudieron incorporarse entonces en versiones subsiguientes de la documentación.

## Documentar la depuración de errores

¿Qué haces cuando tu código no funciona de la forma que esperabas? ¿Revisar los registros de errores? ¿Activar la generación de un registro verboso? Hay todo tipo de sugerencias que les puedes dar a los usuarios de tu proyecto.  Una buena sección de depuración de errores debe contener lo siguiente:

* ¿Dónde están ubicados los registros?

* ¿Hay diferentes niveles de registro? En caso afirmativo, ¿cómo se cambia de uno a otro?

* ¿Hay errores que se pueden encontrar con frecuencia?

Las secciones sobre depuración de errores, como la mayoría de las secciones de la documentación, no deberían ser prescriptivas. Aunque incluir tus detalles de herramientas y configuración como ejemplo puede resultar útil, la documentación no debería suponer el uso de ninguna herramienta o configuración de entorno específicos.

## Ten en cuenta el manual de estilo

Muchos medios de prensa tienen un manual de estilo (AP, NYT, etc.), que los creadores del proyecto deben conocer a la hora de establecer el formato de cualquier texto que vaya a incluirse, si fuera necesario. Tu equipo también podría tener guías de estilo para otras áreas, como programación, diseño y documentación. Asegúrate de compartir esos documentos y de establecer expectativas para los colaboradores. Es mucho más fácil revisar e incorporar una característica nueva si ya se ajusta (o se ajusta bastante) a los estándares que has establecido.

Ejemplos de guías de estilo para programación:

* [Guía de programación](http://codeguide.co/)
* [Guía de estilo para JavaScript de Airbnb](https://github.com/airbnb/javascript)
* [Guías de estilo de Google](https://google.github.io/styleguide/)



## Gestionar la deuda de la documentación

A medida que tu proyecto se expande y tu programa crece, puede que la documentación y el programa comiencen a desfasarse. A medida que más personas empiecen a usar tu código, te darás cuenta de que empezarán a aparecer lagunas en tu documentación. Estas tareas pendientes en la documentación se conocen como deuda de la documentación.

En el equipo del Estudio de Narración de Vox Media, la deuda de la documentación se rastrea igual que las tarjetas Trello y cuando se acumulan 30 tarjetas, el equipo [fija un día](https://storytelling.voxmedia.com/2016/7/29/12299564/on-building-a-culture-of-documentation) para actualizar la documentación. Establecer un sistema de actualización de la documentación que se ajuste a tu forma de trabajo es importante para garantizar que no deje de ser útil.

El equipo de Visuales de NPR y el Instituto de Noticias Sin Fines de Lucro (Institute for Nonprofit News, INN) aprovechan el proceso de capacitación de sus nuevos empleados para paliar la deuda de la documentación. El equipo de Visuales de NPR les pide a sus nuevos miembros leer el [documento de configuración](http://blog.apps.npr.org/2013/06/06/how-to-setup-a-developers-environment.html) y actualizarlo con cualquier cambio que puedan encontrar por el camino. INN invita a sus nuevos empleados a revisar la [documentación del equipo](https://github.com/INN/docs/blob/master/staffing/onboarding/sample-onboarding-plan.md) y a enviar sugerencias de cambios cuando detecten áreas que puedan mejorarse.

> Como parte de mi empleo, hay un proyecto al que dedico tiempo en martes alternos para hacer correcciones e introducir actualizaciones. Así se agiliza el proceso y se acostumbra a todo el equipo a esperar actualizaciones con esa frecuencia. *— Mallory Busch*

## Puntos a verificar

- [ ] Decide qué alcance tendrá la documentación
- [ ] Decide dónde deseas alojar la documentación
- [ ] Decide para quién vas a escribir la documentación (usuarios, nuevos colaboradores, colaboradores de experiencia, etc.)
- [ ] Escribe un archivo README que contenga:
    - un resumen del proyecto
    - instrucciones de instalación
    - cómo ejecutar el proyecto
    - planes futuros para el proyecto
    - cómo colaborar con el proyecto (o un vínculo a tu archivo CONTRIBUTING)
    - créditos
- [ ] Si la documentación va a alojarse en otro lugar, incluye un README mínimo que vincule a ella
- [ ] Comenta tu código
- [ ] Escribe mensajes claros al enviar código para combinar
- [ ] Documenta las diferencias entre la ejecución de código de desarrollo y código de producción
- [ ] Escribe código o tutoriales de muestra
- [ ] Documenta los recursos para depuración de errores (registro, errores frecuentes, cómo ejecutar comprobaciones)
