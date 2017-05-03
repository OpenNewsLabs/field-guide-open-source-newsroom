# Capítulo 3: Liberar un proyecto anterior

**Nunca es demasiado tarde**

![He cometido un gran error](https://media.opennews.org/fieldguides/open-sourcing/error.jpg)

En el [Capítulo 2](Capitulo02-Empezar-proyecto-nuevo.md) vimos cómo comenzar un proyecto nuevo de código abierto. Obtuviste el visto bueno para liberarlo desde el principio, y aprendiste mucho por el camino sobre la importancia de conocer el público de la herramienta, asegurarte de que ya no hubiese una mejor solución en el mundo, y los beneficios de trabajar en público.

O no.

Quizás tú o tu organización ya habían comenzado a trabajar en un proyecto de software *sin* hacerlo público desde el principio. No sería un caso aislado. La mayoría de los proyectos comienzan con código cerrado.

Eso no quita que todavía haya otras personas que puedan beneficiarse de tu trabajo. Lo que es más importante, incluso así puedes beneficiarte de las ventajas de liberar el código de tu aplicación, o parte de tu base de código en forma de librería.  Lo único que necesitarás es un poco de preparación y convencer a tu organización de que hacer esta transición es algo positivo.

## Qué esperar

En este capítulo, examinaremos las decisiones que necesitarás tomar para liberar el código de un proyecto que ya existe. Hablaremos de los potenciales beneficios para ti y los demás. También discutiremos los pasos concretos que necesitarás seguir para higienizar o refactorizar tu aplicación. Y finalmente, navegaremos por las objeciones específicas que podrías escuchar y cómo responder a ellas.

## Cómo han lidiado con esto otras personas

La excelente guía de Karl Fogel, "Producción de software de código abierto" tiene [toda una sección](http://producingoss.com/en/opening-closed-projects.html) dedicada exclusivamente a la liberación de proyectos cerrados. El trabajo de Karl no está enfocado a redacciones periodísticas, pero es útil en general para cualquier proyecto de código abierto.

# Consideraciones prácticas antes de comenzar

## ¿Necesitas liberar todo el proyecto? 

Muchos proyectos que comienzan con código cerrado incluyen partes que son tan específicas para el flujo de trabajo de tu empresa que no serían útiles para nadie más, o también puede que incluyan componentes propietarios que no quieres exponer en internet. Sin embargo, esto no debe ser una razón para renunciar a liberar tu código. Por ejemplo, puedes eliminar las partes que sean muy locales o estén protegidas por derechos de autor e incorporarlas como un módulo aparte que solo tus desarrolladores puedan ver. 

## ¿Está higienizado tu proyecto? 

![limpiar limpiar limpiar](https://media.opennews.org/fieldguides/open-sourcing/sanitary.png)

Aunque en general [separar tu configuración de tu código](https://12factor.net/config) es buena práctica, los programas de código cerrado hacen que sea más fácil para los desarrolladores romper esta regla. ¿Tu aplicación tiene claves o configuraciones en el repositorio que deberían ser exportadas al entorno o administradas de otra forma?

Aquí unos cuantos recursos: 

* Usa un [proyecto como *Git Secrets*](https://github.com/awslabs/git-secrets) de AWS para asegurarte de no estar publicando cambios secretos por accidente en internet. Y dado que tu historial de Git pudiera contener instancias antiguas de esos secretos del repositorio, valora también borrarlo antes de hacer público el proyecto. 

* Limpia la información que pueda contener datos personales, incluyendo datos de muestra que estés enviando con el código. Usa [Poirot](https://github.com/emanuelfeld/poirot), una herramienta que realiza búsquedas en el historial de revisiones de un repositorio para encontrar patrones textuales (ej. contraseñas, tókenes, datos de configuración, direcciones IP, números telefónicos y nombres).

Si estás liberando datos, querrás tener especial cuidado con esto también, particularmente con los datos de los usuarios. Incluso cuando los datos *parecen* haber sido anonimizados, con frecuencia pueden desanonimizarse (o sea, pueden analizarse a la inversa para vincularlos de nuevo al usuario original): 

> * En 2000, Latanya Sweeney demostró que el 87% de la población de EE.UU. puede ser identificada usando solamente su código postal, sexo y fecha de nacimiento ([Fuente](http://dataprivacylab.org/projects/identifiability/paper1.pdf)). 

> * Incluso si la base de datos no incluye información de ubicación, edad o sexo, puede desanonimizarse usando factores aparentemente tan generales como favoritos y términos de búsqueda.

>  * Por ejemplo, en 2006, un conjunto de datos de las búsquedas de AOL llevó a la desanonimización de una usuaria valiéndose simplemente de los términos que había estado buscando ([Fuente](http://www.nytimes.com/2006/08/09/technology/09aol.html)).

>  * En 2008, Narayanan y Shmatikov usaron técnicas de desanonimización para re-identificar a 500,000 suscriptores de Netflix, con un conjunto de datos que únicamente incluía fechas y valoraciones de películas ([Fuente](https://www.cs.cornell.edu/~shmat/shmat_oak08netflix.pdf)).

## ¿El proyecto ya es funcional o todavía está a medio desarrollar?

![](https://media.opennews.org/fieldguides/open-sourcing/makeitfit.gif)

Puede que el proyecto que quieres liberar ya tenga cierto camino recorrido pero no sea funcional todavía. ¿Tienes una hoja de ruta para las próximas tareas que deben ejecutarse en el proyecto? Publicar una hoja de ruta de desarrollo puede ayudar a los potenciales colaboradores a entender qué estás planeando construir, y decidir en qué otras áreas de la base de código pueden concentrarse. De esta forma podrás centrar tu atención únicamente en las funciones necesarias para llevar el proyecto a un estado funcional. 

[TAREA: hipervincular a la sección de hojas de ruta]

## ¿Qué tipo de colaboración te interesa?

El tipo de colaboración que se necesita de la comunidad varía de un proyecto a otro. Quizás tu proyecto es un proyecto maduro y lo único que estás buscando son reportes de errores. Pero también podría ser algo tan nuevo que lo que estás buscando es ayuda para refinar la interfaz de desarrollo. ¿Esperas recibir aportes en partes específicas? Deberías identificar en qué parte(s) del proyecto deseas que la gente ayude. ¿Estás buscando retroalimentación sobre los problemas centrales que el proyecto busca solucionar? Puedes aclararlo incluyendo una sección en el archivo README o creando una serie de tickets sobre esta preocupación. (Consulta el [Capítulo 5](Capitulo05-Documentacion.md) sobre la documentación y el [Capítulo 6](Capitulo06-Comunidad.md) sobre cómo trabajar en comunidad.)

## Manéjalo como si fuera un proyecto nuevo

Consulta el [Capítulo 2](Capitulo02-Empezar-proyecto-nuevo.md) para ver las instrucciones sobre cómo nombrar el proyecto, elegir una licencia y evaluar a la competencia.

## Ejemplos

[TAREAS: ¡añade tus ejemplos!]

## Últimos toques

Hablemos ahora de cómo disponer tu base de código y tu infraestructura de código para tener más probabilidades de éxito.

## Puntos a verificar

- [ ] Toma en cuenta a tu público y a tu competencia
- [ ] Prepara la argumentación de por qué tu organización se puede beneficiar de la liberación de este proyecto
- [ ] Identifica las partes del proyecto que *no deben* liberarse
- [ ] Higieniza tu código para asegurarte de no estar compartiendo secretos ni claves públicamente
- [ ] Comparte tu hoja de ruta de desarrollo, o al menos el estado en que se encuentra el proyecto, para informar a los potenciales usuarios y colaboradores 
