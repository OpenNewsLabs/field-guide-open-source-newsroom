# Capítulo 4: El código y cómo lanzar la primera versión

En este capítulo hablaremos de cómo preparar tu proyecto de código abierto y desarrollarlo de forma tal que:

* Sea fácil para ti y los demás llevar un control de cuánto han avanzado y ayudarse los unos a los otros

* Excluyas los datos privados en lo que publiques

* Reduzcas y evites los errores

* Minimices el trabajo innecesario

* Incrementes las probabilidades de que la gente use el software

## Entonces, ¿qué estamos haciendo aquí?

**No estamos escribiendo código únicamente**. Estamos colaborando en un espacio de trabajo compartido —aunque sea un espacio virtual en lugar de una redacción o un laboratorio físico— haciendo cosas juntos. El trabajo no es solamente escribir funciones y clases, sino también experimentar y planear y proponer ideas tipo "esto es lo que deberíamos hacer".   Por lo tanto, deberíamos tratar de asegurarnos de que cualquiera que entre a nuestro espacio de trabajo pueda ver qué es lo que hemos dicho y hecho, y pueda reutilizar el trabajo que ya se ha realizado. 

**Digámoslo una vez más: no estamos escribiendo código solamente.** Estamos haciendo historia, una historia utilizable, que puedes usar tú, o los colaboradores que aparezcan el año que viene. Es por eso que estaremos hablando de cómo usar un sistema de [control de fuente](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) (conocido también como [control de versiones](https://en.wikipedia.org/wiki/Version_control)) que mantenga un registro de quién ha hecho qué y por qué. Por eso es que sugerimos que uses un controlador de cambios público para tus TAREAS. Y es la razón por la cual es importante tener cuidado con lo que publicas (código o contenido visible en el controlador de errores), porque una vez que publicas algo en internet es imposible borrarlo completamente.

Sin embargo, primero una nota al margen: es importante no olvidar que todo lo que se incluye en este capítulo es algo ideal. Dados tu tiempo y recursos, puede que no sea fácil hacerlo todo (bien).  Es difícil decir qué es lo mínimo que debe tener un proyecto de código abierto para triunfar, pero recuerda que no todos incluirán todos los elementos.

## Control de versiones

Hay muchos sistemas de control de versiones que puedes usar para alojar tu repositorio, pero nuestra recomendación es que uses Git y GitHub, que es el sistema más popular en las comunidades de código abierto y periodismo. He aquí unos cuantos recursos para cada nivel, sea cual sea tu grado de familiarización con Git hasta este punto.

### Git

Particularmente si vas a ser quien dé mantenimiento a nivel de código, [aprende a usar Git más allá de las funciones básicas](https://www.harihareswara.net/sumana/2014/10/31/0). 

Aquí tenemos una [lección básica sobre Git](https://openhatch.org/missions/git) por ejemplo. Clona un repositorio de un proyecto que no te interese y trata de usar los comandos más avanzados haciéndole pequeños cambios al código. Así, si arruinas todo, no habrás echado a perder el trabajo. 

Aprende a ramificar y a combinar cambios y a trabajar con remote y cherry-pick y bisect. Lee [esta explicación superútil sobre el modelo de Git](http://web.mit.edu/nelhage/Public/git-slides-2009.pdf), que explica exactamente qué hace qué. Te ayudará.  

Más recursos:

* [Por qué trabajar con ramas y cómo hacerlo](http://producingoss.com/en/vc.html#branches)

* [Un modelo acertado de ramificación en Git](http://nvie.com/posts/a-successful-git-branching-model/)

## Ayudar a otros a contribuir

Ayuda a la gente a saber cómo pueden contribuir a tu proyecto.  Uno de los tantos beneficios del código abierto es lograr que otras personas le echen un vistazo a tu código y ayuden a mejorarlo.  Es importante facilitar este proceso tanto como sea posible creando una documentación específica sobre cómo hacerlo.  He aquí unas cuántas formas de proceder:

* **Céntrate en buena documentación y buenas directrices para colaboradores.** Consulta el [Capítulo 5](Capitulo05-Documentacion.md) para más información.

* **Algunas cosas como gestión de dependencias**, Docker, etc., son buenas tecnologías para ayudar a que la gente colabore más rápido.

* [TAREA: más ejemplos aquí]

## Seguimiento de problemas

Usa un control público de cambios para problemas/errores.  Es probable que tu código vaya a presentar algunos problemas o que necesite perfeccionamiento, y es importante que la gente pueda comunicarte esas cuestiones.  También es muy beneficioso que estas cuestiones sean públicas, para que quienes enfrenten los mismos problemas puedan encontrarlas y posiblemente resolverlas ellos mismos.

* Si estás usando GitHub, puedes utilizar los Problemas (Issues).

* Probablemente sea buena idea incluir en el archivo README o en la documentación principal información sobre dónde la gente puede reportar problemas.

* Valora evitar usar la sección Issues (Problemas) de GitHub para asistencia técnica, para que no te abrumen las preguntas de ayuda.

Ayuda a la gente a ver cómo hacer preguntas/informar sobre un error.  Para ayudar a que los Problemas resulten más eficientes para ti y tus usuarios, puedes añadir indicaciones sobre cómo [buscar problemas vigentes](http://wp-cli.org/docs/bug-reports/) y preguntas.  

GitHub te permite crear [plantillas de problemas](https://help.github.com/articles/creating-an-issue-template-for-your-repository/), que son realmente útiles para la eficiencia del trabajo:

* Ejemplo de plantilla de problemas:

```
### ¿Qué estabas tratando de hacer? Por favor incluye la versión del programa que estabas usando.

### ¿Qué esperabas que pasara?

### ¿Qué pasó en lugar de eso? Si viste un mensaje de error, por favor, pégalo aquí también.
```

## Versiones

Cada vez que publiques una nueva versión de tu programa debería haber un número de versión asociado. Suele ser un número de 3 dígitos, como 1.2.3 y la estructura más común es el  [Versionamiento semántico](http://semver.org/), que trata de comunicar cierto nivel de compatibilidad con números y ubicaciones específicas.

## Paquetes/distribución

Si deseas que otros medios de prensa usen tu proyecto, entonces en cada actualización deberás darles una versión que puedan instalar (en forma de app descargable o como un "paquete").

Adáptate a las necesidades de tus usuarios — si es una aplicación, ponla en la App Store de Apple o en Google Play.  La mayoría de los lenguajes de software tienen un administrador central de paquetes, que facilita la obtención y la administración de los módulos de código.

<table>
  <tr>
    <td>Lenguaje o herramienta</td>
    <td>Administrador de paquetes</td>
  </tr>
  <tr>
    <td>Javascript</td>
    <td>NPM</td>
  </tr>
  <tr>
    <td>CSS o HTML</td>
    <td>NPM (y en menor medida Bower)</td>
  </tr>
  <tr>
    <td>Python</td>
    <td>PyPI</td>
  </tr>
  <tr>
    <td>Ruby</td>
    <td>RubyGems</td>
  </tr>
  <tr>
    <td>PHP</td>
    <td>Composer</td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
  </tr>
</table>


Más detalles sobre cómo lidiar con [casos raros y pequeñas cuestiones de procedimiento](http://producingoss.com/en/packaging.html).

## Dependencias

Trabaja con los frameworks y dependencias que sean populares en tu comunidad de usuarios y cuya estabilidad esté demostrada.  Usar dependencias inestables o sin mantenimiento puede desestabilizar tu proyecto.

Por ejemplo: Si tus usuarios están usando Python 2.7 y todavía no han cambiado a Python 3, probablemente lo mejor sea que tu aplicación corra en Python 2.7.  Si la mayoría de tus usuarios está en Windows, asegúrate de que tu cosa corra en Windows.

Usa el administrador de paquetes más apropiado para las dependencias. (Consulta "Paquetes" más adelante).  Esto ayudará a que la instalación y el proceso de desarrollo sean más fáciles y predecibles.

A veces puede ser mejor tratar de evitar las dependencias porque no son estables, o quizás simplemente quieres evitar que la instalación sea engorrosa.  (Por ejemplo, instalar dependencias para interfaces que emplean un navegador puede ser difícil, o demandar demasiada variedad, y puede que no valga la pena.)

## ¿Está higienizado tu proyecto? 

Regresa al [Capítulo 3](Capitulo03-Proyectos-anteriores.md) donde hablamos sobre consideraciones verdaderamente importantes a la hora de mantener a salvo y en privado la información y los datos. 

## Pruebas automatizadas e integración continua

Las pruebas automatizadas en y para tu base de código reducen las regresiones, lo cual te permite a ti y a tus colaboradores trabajar y añadir código más rápido. Pero no pierdas el sueño queriendo conseguir un 100% de cobertura, porque definitivamente la utilidad de esto es estrecha y menos importante cada vez. [Travis CI](https://travis-ci.org/) es muy fácil de configurar para casos normales.  

Aquí algunos recursos para depuración de errores:

* [Depuración sistemática de errores
](http://akaptur.com/blog/2013/07/24/systematic-debugging/)

* [Notas rápidas en Software Libre y de Código Abierto para nuevos colaboradores sobre el método científico y la historia utilizable](https://www.harihareswara.net/sumana/2016/10/12/0) 

También hay herramientas para generación automatizada de documentos que te pueden dar ventaja a la hora de crear documentación. Por ejemplo:

* [Doxygen (Java/C++/PHP/Python)](http://www.doxygen.org/)

* [Pydoc (Python)](https://docs.python.org/2/library/pydoc.html)

* [Swagger (RESTful APIs)](http://swagger.io/)

Incluso puedes automatizar pruebas para muchas de las sugerencias expuestas en esta guía de campo. Open Project Linter es una herramienta acompañante que comprueba si los directorios de tu proyecto cumplen con buenas prácticas de documentación y programación. (¡Y también es un proyecto de código abierto en el cual puedes colaborar!)

* [Open Project Linter](https://github.com/OpenNewsLabs/open-project-linter)


[TAREA: información sobre cómo identificar bugs, errores y errores de usuarios]

## Más recursos

He aquí un buen resumen del camino para llegar a la primera publicación del proyecto:

* Publicar un proyecto de código abierto: [http://wiki.civiccommons.org/Releasing_Open_Source/](http://wiki.civiccommons.org/Releasing_Open_Source/) 

## Puntos a verificar

- [ ] Usa control de versiones
- [ ] Usa un control público de bugs para las TAREAS
- [ ] Evalúa qué es lo que necesitas en realidad para un proyecto mínimo
- [ ] Crea un archivo README claro e informativo
- [ ] Crea un archivo CONTRIBUTING (COLABORAR) independiente
- [ ] Evalúa usar herramientas de administración de dependencias, Docker, etc. para ayudar a que la gente empiece a colaborar más rápido
- [ ] Anuncia dónde es que los usuarios y los colaboradores pueden informar sobre problemas
- [ ] Usa las plantillas de problemas en Github
- [ ] Asegúrate de asignarle a tu producto números de versiones
- [ ] Ofrece una versión instalable (aplicación o paquete)
- [ ] Pon a disposición pública el paquete desde el administrador de paquetes asociado
- [ ] Determina qué frameworks y dependencias son estables y populares en la comunidad de tus usuarios y valora usarlos
- [ ] Evita incluir datos sensibles en el repositorio
- [ ] Firma criptográficamente los paquetes y/o las incorporaciones de código individuales con GPG
- [ ] Crea pruebas automatizadas para que puedas cambiar el código con confianza
- [ ] Usa integración continua
- [ ] Evalúa la pertinencia de usar herramientas de generación de documentos
