# tecnochiguires
Pagina web del equipo TecnoChiguires para programacion 2.
Criterios
Para esta evaluación, nuestros criterios eran:
Realizar la navegación por lo menos en  3 páginas web programadas en cualquier lenguaje de programación que el equipo considere conveniente.
Una de esas páginas debe solicitar datos y validarlos con javascript.
Incluir bootstrap en los diseños de dichas páginas.
Diseño de la página
La página consiste de 7 archivos estáticos HTML. El usuario puede navegar fácilmente entre las páginas utilizando los menús de navegación y el flujo de registro.

La página de inicio contiene enlaces al resto de las páginas principales: el portafolio, la sección “sobre nosotros”, y la página de registro.

El portafolio contiene el contenido principal de la página. La sección “Sobre nosotros” contiene la información del equipo, asi como un enlace a nuestro repositorio de github donde se puede ver el código fuente de la página.

La temática de la página es un portafolio, el cual contiene información de proyectos realizados por el equipo previamente, y contiene un botón de registro para crear una solicitud para formar parte del equipo.

Al hacer click sobre el botón de registro, la página ejecuta código javascript que realiza las siguientes acciones:
Revisa si el usuario ya tiene iniciada una sesión
De ser positivo, se redirige a la página “Usuario”, donde el usuario puede ver toda la información de su cuenta.
Una vez que la solicitud de entrar al equipo se aprueba manualmente por el administrador, la página cambia para indicar que fue aprobado. De otro modo, la página dice que la solicitud está pendiente.
La página permite al usuario cerrar su sesión y crear un nuevo registro.
De ser negativo, se redirige a la página “Formulario”, donde el usuario puede registrarse por primera vez. Al fondo de la página “Formulario”, hay un enlace que lleva a la sección “Iniciar Sesión”, donde el usuario puede volver a entrar en una sesión anterior.
Una vez registrado, el usuario es redirigido a la página “gracias”, donde se le indica que su solicitud está siendo revisada, y que puede acceder a su página de usuario donde podrá ver la información que acaba de ingresar.

Este código es funcional, y se programó utilizando javascript para el funcionamiento del botón de registro y validación del formulario, y utiliza la base de datos de firebase para almacenar los datos del usuario y autenticación.

La lógica javascript está incluída directamente en el archivo HTML, por lo que no hace falta tener un archivo separado js. A futuro, una vez que el equipo considere expandir la página, el código javascript puede moverse a un archivo separado y enlazarse.

Enlace a la página web
La página web es accesible desde el enlace https://tecnochiguires.vercel.app/

Para visualizar el código fuente de la página, puede navegar a la sección “Sobre Nosotros” y hacer click en el enlace “Ver código fuente en GitHub”

Alternativamente, en caso de que la página presente fallas o no esté disponible, también puede descargar el código desde esta carpeta de google drive.

Para iniciar la página localmente, deberá hacerlo con un servidor local. La manera más fácil de hacerlo es con python. Puede navegar hasta la carpeta con la terminal y ejecutar el comando “python -m http.server”.
