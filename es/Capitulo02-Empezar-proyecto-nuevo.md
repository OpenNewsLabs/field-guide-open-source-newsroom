# Capítulo 2: Empezar un proyecto nuevo

**En el inicio...**

Felicitaciones: ¡ya tienes el visto bueno de tu organización! Tu plan tiene todo el apoyo de los involucrados, de los jefes y del equipo. Porque tienes un plan, ¿cierto?

No hay por qué asustarse.  Es normal sentir un poco de nerviosismo cuando pones tu código a la vista pública para que todo el mundo venga a decirte cuán equivocad@ estás o que es mejor usar tabulación que espacios.  Desde el punto de vista emocional, el código abierto no siempre es fácil; como muchas otras cosas en internet, le da a la gente la oportunidad de señalarte tus errores semi-anónimamente.  Es importante recordar que 1) es probable que hayas cometido uno o dos errores, y que 2) todo el mundo comete errores.  Trata de no tomarte las cosas de manera personal, y asume los comentarios como pequeñas críticas constructivas que van a ayudar a mejorar las cosas.  A medida que trabajes más con código abierto, tanto en proyectos propios como de otros, te sentirás más segur@ y te preocuparás menos por los inevitables errores.


> Uno de mis primeros proyectos de código abierto fue el módulo OpenLayers de Drupal que, como el nombre indica, integraba la librería OpenLayers de javascript al sistema de gestión de contenidos Drupal.  Curiosamente, casi el mismo día que lancé una primera versión bastante cruda del módulo, otra persona lanzó una muy similar.  Fue un poco desalentador, pero cuando hablamos, decidimos que teníamos metas semejantes y empezamos a colaborar en un módulo único, que resultó ser una experiencia muy positiva.  A medida que el módulo creció y se sumaron otros colaboradores, la dirección de la arquitectura tomó otro rumbo.  Emocionalmente, estaba muy apegado al proyecto, y me costó trabajo lidiar con estos cambios. Las dificultades de la comunicación en línea (de hecho, la mayoría todavía está en la cola de problemas de Drupal) tampoco ayudaron, y la experiencia colaborativa se volvió negativa para mí. Eventualmente ya no tuve ni tiempo y ni energía emocional para dedicarle al proyecto  —que todavía subsiste, con un grupo de colaboradores completamente diferente.

>La lección que aprendí desde temprano es que en el trabajo de código abierto no se pueden tomar las cosas muy a pecho.

> *- Alan Palazzolo*


Este capítulo te guiará en el proceso de empezar un nuevo proyecto de código abierto, discutiendo los primeros pasos, e introduciendo las tareas principales y los retos/riesgos potenciales.

## Nombrar las cosas

![Hola, mi nombre es...](https://media.opennews.org/fieldguides/open-sourcing/hello-sticker.jpg)

Todo el mundo sabe que en computación solo hay dos problemas difíciles: los errores por un paso (OBOE) y asignarles nombres a las cosas. Hay una [cantidad](https://pages.18f.gov/open-source-guide/naming-your-project/) [infinita](http://ivantomic.com/projects/ospnc/) [de artículos](http://jerodsanto.net/2014/08/naming-things-is-hard-lets-go-shopping/) [sobre cómo elegir](http://deviq.com/naming-things/) [un buen nombre](http://www.avangate.com/avangate-resources/article/product-naming.htm). Identifica tu objetivo cuando vayas a darle nombre a tu proyecto. ¿Estás tratando de crear un proyecto que sea fácil de encontrar? Elige un nombre sencillo, claro y directo. ¿Estás tratando de ser creativ@? ¡Las posibilidades son infinitas! Sin embargo, por lo general los nombres buenos son peculiares, descriptivos y fáciles de recordar.

Nombrar un proyecto puede ser muy importante si termina siendo un gran éxito, pero también es algo que se puede cambiar por el camino (con algunos dolores de cabeza a veces).  Entonces, dedica un tiempo a pensar en un nombre que te parezca aceptable, pero no lo pienses demasiado.

## Elegir una licencia

A la hora de elegir una licencia, las siguientes sugerencias pueden ayudar a que esta decisión legalmente vinculante no resulte tan atemorizante.

* Ten en cuenta las necesidades internas de tu organización. ¿Planeas vender este software a otras organizaciones? ¿Tienes reglas estrictas de propiedad intelectual que te impedirían permitirles a los demás modificar tu trabajo para desarrollar algo nuevo? Es posible que debas consultar esto con tu equipo legal, pero si no está claro, es mejor que vayas a verlos con un plan concreto.

* Habla con el asesor legal de tu organización. Tu decisión individual sobre el tipo de licencia podría desestimarse si el abogado recomienda una licencia diferente por razones que te son desconocidas.

>El asesor de *The New York Times* recomendó que usáramos la licencia Apache 2.0 en lugar de la MIT, no por nada inherente al funcionamiento de las licencias, sino porque estaba más familiarizado con Apache 2.0.

>*— Jeremy Bowers*

* Echa un vistazo al tipo de licencias que están usando organizaciones similares en sus proyectos de código abierto, o usa la licencia que sea más popular en la comunidad que esperas que contribuya a tu proyecto. ¿Vas a crear un plugin para WordPress? Revisa el directorio de plugins y sigue la ruta que más sentido tenga para ti.

* Estúdiate la lista de licencias más comunes y las protecciones que ofrecen. Consulta recursos como [choosealicense.com](http://producingoss.com/en/license-quickstart.html) de GitHub, o familiarízate con licencias populares como la [MIT](https://opensource.org/licenses/MIT) y la [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) para determinar cuál es la que se ajusta a tus necesidades.

* Piensa en quién va a usar tu código.  Aunque en teoría puede ser cualquiera, la licencia que elijas afectará la forma en que ciertos grupos u organizaciones podrán usar tu código.

Hay muchas licencias para elegir y debes irte por la que mejor sea para ti. Para reducir la búsqueda, podemos decir que básicamente hay dos tipos de licencias:

1. **Copyleft**.  La licencia Copyleft establece que cualquiera puede usar el código en otro proyecto, con la condición de que se preserve el tipo de licencia, lo cual generalmente significa que los [trabajos derivados](https://en.wikipedia.org/wiki/Derivative_work) solamente pueden distribuirse bajo la misma licencia.  La mayor ventaja de esta licencia es que obliga a que el código continúe siendo abierto.  La mayor desventaja es que a veces puede entrar en conflicto con las políticas internas de algunas organizaciones y hacer que les sea más difícil usar tu herramienta (normalmente con fines comerciales).

    1. [https://es.wikipedia.org/wiki/Copyleft](https://es.wikipedia.org/wiki/Copyleft)

    2. En este grupo la más común es la licencia GPL, cuya versión más reciente es la GPLv3.

2. **Permisivas**.  Una licencia permisiva básicamente establece que el usuario puede hacer cualquier cosa que desee con el código, atribuyendo la autoría a veces.  Su principal ventaja es que cualquiera podrá usar tu código sin importar las restricciones internas específicas que puedan tener.  La parte negativa es que no exige que el nuevo producto siga siendo de código abierto, lo cual va en contra de los principios de la cultura abierta.

    3. [Licencia de software libre permisiva](https://es.wikipedia.org/wiki/Licencia_de_software_libre_permisiva)

    4. La licencia permisiva más común es la MIT.

> **Elige la licencia MIT.** La licencia MIT es la más popular en proyectos de código abierto.  Es muy sencilla y permite a los usuarios hacer lo que deseen.  Si no tienes necesidades específicas en tu organización que te lleven a usar una licencia diferente, vete por esta.  De hecho, es tan breve que podemos incluirla aquí:

> Copyright (c) <año> <titulares de los derechos>

> Se concede permiso, de forma gratuita, a cualquier persona que obtenga una copia de este software y de los archivos de documentación asociados (el "Software"), para utilizar el Software sin restricción, incluyendo sin limitación los derechos a usar, copiar, modificar, fusionar, publicar, distribuir, sublicenciar, y/o vender copias del Software, y a permitir a las personas a las que se les proporcione el Software a hacer lo mismo, sujeto a las siguientes condiciones:

> El aviso de copyright anterior y este aviso de permiso se incluirán en todas las copias o partes sustanciales del Software.

> EL SOFTWARE SE PROPORCIONA "TAL CUAL", SIN GARANTÍA DE NINGÚN TIPO, EXPRESA O IMPLÍCITA, INCLUYENDO PERO NO LIMITADO A GARANTÍAS DE COMERCIALIZACIÓN, IDONEIDAD PARA UN PROPÓSITO PARTICULAR Y NO INFRACCIÓN. EN NINGÚN CASO LOS AUTORES O TITULARES DEL COPYRIGHT SERÁN RESPONSABLES DE NINGUNA RECLAMACIÓN, DAÑOS U OTRAS RESPONSABILIDADES, YA SEA EN UNA ACCIÓN DE CONTRATO, AGRAVIO O CUALQUIER OTRO MOTIVO, QUE SURJA DE O EN CONEXIÓN CON EL SOFTWARE O EL USO U OTRO TIPO DE ACCIONES EN EL SOFTWARE.

### Licencias para proyectos que no son de programación

Las licencias anteriores se centran en la reutilización de código, pero también es importante establecer los derechos de otros materiales que estés liberando, como imágenes o datos en bruto. Si no se establece una licencia explícita, es posible que algunos usuarios no tengan la libertad de usar estos recursos, ya sea porque lo prohíben las leyes locales o las políticas de sus empleadores. Incluir licencias para todos los elementos de tu proyecto es la mejor manera de dejar en claro los derechos de los usuarios.

La licencia más común para recursos no informáticos es la [Creative Commons](https://creativecommons.org/share-your-work/), que es un conjunto de licencias diseñado para que el usuario pueda comprenderlas y combinarlas más fácilmente en dependencia de sus necesidades. Creative Commons se usa principalmente para contenido multimedia y escrito, como por ejemplo texto, imágenes y videos.

La [Open Data Commons](http://opendatacommons.org/) es una licencia parecida a Creative Commons, pero está más enfocada en los datos.  OpenStreetMap, un proyecto de datos abiertos que ha tenido mucho éxito, usa una licencia ODbl.

### Derechos de autor

Es importante destacar que asignarle una licencia a tu proyecto de código abierto no significa que estás renunciando a tus derechos sobre ese material, ni personalmente ni como organización (dependiendo de cómo se manejen los derechos en tu redacción).  Una licencia es básicamente una respuesta a la pregunta "¿Puedo usar esto? ¿Cómo?" que pueda hacer cualquiera.

Por otro lado, cualquier aporte realizado por otras persona u organizaciones continuará siendo propiedad intelectual de esos colaboradores.  Si tu proyecto crece mucho, puede que valga la pena considerar el uso de un [Contrato para colaboradores](https://en.wikipedia.org/wiki/Contributor_License_Agreement), para que tanto el proyecto como los colaboradores tengan derechos/roles más definidos.

## Conoce a tu público

Como con cualquier otro producto (apps de noticias o artículos, etc.), tu software probablemente tiene un público meta. En este caso estamos hablando de usuarios. ¿Quiénes son los usuarios que están reclamando la existencia de una cosa que haga lo que hace tu software? Debes mantener a esos usuarios en mente a lo largo de todo el proceso, no solo para construir algo que se ajuste a sus necesidades, sino también para construirlo de manera que sea utilizable.

Por ejemplo, si estás construyendo una herramienta que pequeños medios de prensa sin fines de lucro pudieran integrar a sus sistemas de gestión de contenido, toma en cuenta los sistemas que usan esas redacciones actualmente y los recursos que tienen a su disposición para evaluar e instalar código nuevo.

## Estudia a tu competencia

![oh, Wash](https://media.opennews.org/fieldguides/open-sourcing/wash.gif)

Internet es un mar de cosas. De tantas cosas... Y tú quieres que tu producto sea una de ellas. ¿Estás segur@ de que ya no hay algo que cumple la misma función?

Puede que sí. Decide si es momento de pararte en los hombros de gigantes, contribuir al desarrollo de un proyecto de código abierto que ya existe, hacerlo tuyo, y volverlo a lanzar al mundo para que los demás hagan lo mismo; o si es hora de romper con el pasado y crear algo mucho, mucho mejor. Para ponerlo en otros términos, es el momento en que vas a decidir si vas a reinventar la rueda, y puede que a veces sea necesario si tu meta es construir un auto volador.

Dedícale un tiempo a buscar proyectos similares en la comunidad de nerds del periodismo y más allá, en Github y otros lugares. Si encuentras un repositorio impresionante que quieras seguir desarrollando, examina en más detalle los problemas, solicitudes de cambios y contenido añadido, para llevarte una idea de si el repositorio recibe mantenimiento. Después, ponte en contacto con los dueños y descubre qué han aprendido por el camino.

## Más información sobre el comienzo

* "Producción de software de código abierto" de Karl Fogel [Capítulo 2: Primeros pasos](http://producingoss.com/en/getting-started.html)

## Próximos pasos

Estamos muy felices por ti. ¡Has empezado tu primer proyecto de código abierto!

![ahhhhhhhhhhhh](https://media.opennews.org/fieldguides/open-sourcing/kermit.gif)

Pero espera, hay más. Salta al [Capítulo 4](Capitulo04-Primera-version.md) para aprender más sobre el lanzamiento de la primera versión, cómo escribir documentación detallada y útil, cómo expandir tu comunidad y qué hacer con respecto al fin inevitable de tu idea. O si tu tarea es liberar un proyecto que ya existe, dirígete al [Capítulo 3](Capitulo03-Proyectos-anteriores.md).

## Puntos a verificar

- [ ] Nombra tu proyecto
- [ ] Elige una licencia
- [ ] Identifica a tu público
- [ ] Estudia a tu competencia
- [ ] Valora la pertinencia de reclutar socios
- [ ] Crea o bifurca un repositorio
- [ ] Comienza a escribir tu documentación (archivo README)
- [ ] Añade la licencia que elegiste y la documentación inicial para colaboradores
- [ ] ¡Añade un poco de código!
- [ ] Añade otro poco más
- [ ] Actualiza la documentación (archivo README).
- [ ] Genera tu primera versión
- [ ] Ten un plan de mantenimiento y asistencia técnica
- [ ] Ten un plan de contingencia para desactivar el proyecto y para otras cosas negativas que puedan ocurrir
