# Anteproyecto

Created: March 26, 2024 4:01 PM

# Título del proyecto

Chato

# Nombre de los autores

- Javier Miguel Martín Gallardo, se enfocará en la parte de Angular e Ionic. --> [Enlace del repositorio de Javier](https://github.com/jotaeme890/TFC-Chato-Angular/tree/definitive-tfc)
- Adrián Perogil Fernández, hará la parte de Android. --> 
[Enlace del repositorio de Adrián](https://github.com/imchopi/TFG_Chato_Android)

# Descripción

Nuestro proyecto se basará en una aplicación enfocada en las incidencias de una empresa, en la cuál estará implicado un administrador y un usuario, siendo este último quien podrá subir las incidencias para que el administrador las pueda solucionar. Acciones que puede usar cada rol:

- **ADMINISTRADORES**
    - Gestión de usuarios.
    - Gestión de categorias.
    - Gestión de incidencias.

- **USUARIOS**
    - Gestión de su propio perfil.
    - Visualización de sus incidencias.
    - Creación de incidencias.
    - Filtrado por categoría de las incidencias.

# Objetivos del proyecto

Nuestro objetivo para este proyecto, es poder ayudar a las empresas mediante una aplicación de incidencias, para que el usuario pueda enviar la incidencia al administrador y este resolverla. También mediante las categorías, tanto el usuario como el administrador, tendrá más claro el tipo de problema para resolver la incidencia con mayor facilidad.

# Tecnologías utilizadas

- **Móvil**
    - **Backend:** Firebase.
    - **Frontend:** Android & Kotlin.

- **Web**
    - **Backend:** Firebase.
    - **Frontend:** Angular & Ionic (Typescript).
    

# Estructura de datos

La estrategia que seguiremos:

- Estrategia 1: Colecciones separadas
    - Con esta estrategía pretendemos englobar toda la información en un documento →  colección userInfo
    - Así conseguimos tener los datos almacenados tanto para ver los usuarios con mayor claridad y realizar algún cambio en el futuro en caso de querer modificar un usuario.
- Estrategia 3: Documentos Denormalizados
    - Usaremos esta estrategia para los documentos de incidentsInfo y categoryInfo ya que necesitaremos mezclar datos de ambos documentos, así conseguiremos con una consulta, extraer toda la información.

![image](https://github.com/imchopi/TFG_Chato/assets/92975232/c8267ed9-6506-4982-bb0d-53ebaacd0a4d)


# Tareas

Adrián - Android

Tareas realizadas y cambios
- Página de bienvenida (18 de Abril)
- Registro → Por correo (18 de Abril)
- Login → Por correo (18 de Abril)
- Página de incidencias (19 de Abril)
- Listado de incidencias (22 de Abril)
- Detalles de incidencias (23 de Abril)
- Añadir incidencias (24/25/26 de Abril)
- Cámara (29 de Abril)
- Galería (30 de Abril)
- Diseño (1/2/3/6/7 de Mayo)

Tareas pendientes por hacer  
- Mostrar detalles del usuario en el menú
- Modo offline con Room
- Comprobación de inputs en el registro
  
Tareas realizadas de las pendientes
- Mostrar detalles del usuario en el menú (30 de Mayo)
- Modo offline con Room (25 de Mayo)
- Comprobación de inputs en el registro (4 de Junio)
- Traducción (9 de Junio)

</br>
Javier - Angular
</br>

- **Día 08/04/2024 →** Ya que no nos han proporcionado el feedback del anteproyecto, he realizado el diseño de la página de **Login** y la de **Registro** en Figma. Este diseño es el básico (sin texto, ni colores, etc).

- **Día 09/04/2024 →** Hoy he creado el repositorio, añadido todos los servicios principales (Autenticación, Traducción). Y he creado la página de **Access** que contendrá el componente de LogIn y el de Register. He hecho un pequeño formulario de Login usando Angular Material, aún falta estilo y que pueda hacer Login y registro.

- **Día 10/04/2024 →** Hoy le he añadido estilo a la página de acceso, a los componentes de registro y de login, he añadido un validador para saber si las contraseñas coinciden. He añadido a los formularios los errores. He arreglado algunas propiedades mal escritas en las interfaces y he agregado el registro y el logueo conectándose al Backend en Firebase.

- **Día 11/04/2024 →** Añadida la guarda para tener que estar logueado en la aplicación para poder navegar en las páginas que no sean las de acceso, he cambiado el estilo del formulario de registro, ya que he arreglado los errores que seguían saliendo al registrarse, he arreglado las interfaces (añadiendo los atributos **role** y **surname**, y he eliminado los atributos **firstSurname** y **secondSurname**) y he agregado una guarda para que solo los usuarios con el rol de **Admin** puedan acceder, ya que la página es de administración.

- **Día 12/04/2024 →** He añadido PrimeNG al proyecto, ya que quiero tener toast personalizados en algunas partes de la aplicación, he creado el logo de la app, y he cambiado la pantalla de acceso para que este salga en los dispositivos con pantallas más pequeñas (ya que en tamaño grande sale una imagen a la derecha de los formularios), he añadido un toast que sale al registrarte ya que solo puedes acceder a mi parte de la aplicación si eres admin (por defecto en el registro es usuario normal, un admin te tiene que cambiar el role). Me falta poner toast en los fallos del login (y ver cómo recoger el error de que un gmail ya está en uso) para acabar con la página de acceso.

- **Día 16/04/2024 →** He empezado el diseño de la página **Home,** la cual contendrá todas las incidencias que van dejando los usuarios, desde allí podremos navegar a cada una de las incidencias, al igual que aplicarle filtros a la vista general y acceder al menú de la aplicación. También he diseñado la vista de la página con el menú abierto. También he añadido toast con errores al hacer un registro(el de correo en uso), en el login, me da error y sale el error aun que esté bien y después ya carga y lleva a **Home** (HABLAR CON JUAN, SOLUCIONADO).

- **Día 17/04/2024 →** He arreglado el problema con los toast a la hora de iniciar sesión y registrarse (arreglando también su tamaño). También he añadido el header de la aplicación, con un menú lateral y el logo de la app.

- **Día 18/04/2024 →** He añadido el SplashScreen para que al recargar la página no vaya a **Access** y después navegue a **Home**, he usado un lottie para que se vea una animación mientras tanto. También he empezado a crear el diseño final de la aplicación. Al crear el SplashScreen me ha empezado a dar errores ya que al hacer el deslogueo del usuario, al volver a **Access** había una capa invisible por encima de la página y se quedaba inutilizable, lo he arreglando borrando el component de header y pasando todo el header y el menú a **app.component.html**, aun que creyendo que era el SplashScreen lo he acabado borrando, más adelante lo pondré.

- **Día 19/04/2024 →** Hoy he implementado ya la captura de datos desde Firebase, para obtener los datos de los usuarios logueados en la aplicación, he acabado la estética del menú lateral y he implementado todas las páginas que incluye dicho menú.

- **Día 22/04/2024 →** Hoy he agregado una tabla para poder ver la información de todos los usuarios conectados, también he añadido un tab para ver la información o los datos en forma de gráficas. También he añadido la vista de la información detallada de los usuarios. Y también el update de los usuarios.

- **Día 23/04/2024 →** Hoy he cambiado la forma en la que tenía el update de los usuarios, ya que no cambiaba correctamente los datos, y al modificar el usuario conectado no se actualizaba el observable de user$. También he estado modificando el menú para añadir la foto del usuario y abajo de dicho menú con la opción de navegar a la página de **About**. He incluido el contenido de dicha página, incluyendo la información de los repos de Adri y mía.

- **Día 25/04/2024 →** Hoy he avanzado con los diseños de la aplicación en Figma.

- **Día 26/04/2024 →** Hoy he creado la vista del componente del incidente, ya solo me quedaría la vista en detalle del incidente y agregar la parte de los filtros (NO FUNCIONAL PARA CHECKPOINT), para posteriormente hacer los filtros funcionales, y la página de ajustes, con el cambio de iodoma y el perfil del usuario conectado.

- **Día 27/04/2024 →** Hoy he seguido con el diseño en figma. Y he arreglado el diseño de la tarjeta del incidente para que se viera mejor.

- **Día 29/04/2024 →** Hoy he intentado arreglar el diseño de la página de **Home** pero sigue fallando, he cambiado la interfaz de las incidencias para recoger un TimeStamp y he arreglado la plantilla para que muestre la fecha y la hora de la incidencia correctamente.

- **Día 30/04/2024 →** Hoy he arreglado el diseño de la página **Home**, y ahora es completamente responsive y las tarjetas de las incidencias se ven correctamente, también he cambiado el tipo de dato que introduzco en Firebase al subir una foto, ya que antes tenía los diferentes tipos de tamaño, pero cómo introduce al final la misma url en todos, no merece la pena dejar que sea un objeto, por lo que ahora solo introduce el string de la url hacía el storage.

- **Día 02/04/2024 →** Hoy he mejorado el diseño de la vista de las incidencias, para que se viese mejor en dispositivos más pequeños, también he seguido con el diseño en figma, ya solo me quedaría poner que el usuario pueda modificar el role de otro usuario (se me pasó ponerlo en el formulario que ya hay) y la vista del detalle de las incidencias para el checkout. Después me quedaría la vista de los gráficos en **Análisis de datos** y toda la página de **Ajustes**.

- **Día 03/05/2024 →** Hoy he añadido el campo de role a la hora de editar un usuario, ya que anteriormente no lo tenía hecho y al modificar el usuario no se podía cambiar este. También he seguido con el diseño en Figma.

- **Día 04/05/204 →** Hoy he empezado con la vista de detalle de las incidencias, he modificado el servicio de incidencias, y he añadido que cada vez que cliquemos en una incidencia, si su valor de **checked** está en falso, pase a verdadero, así podremos usar más adelante este campo para filtrar y a parte para poner una directiva a las incidencias que no estén abiertas. Ahora mismo está puesto temporalmente el cambio del tipo string a Date, ya que Adri está subiendo la fecha en tipo string. Y he añadido una pre-directiva para el checkpoint, para que las incidencias no vistas salgan de otro color.

- **Día 05/05/2024 →** Hoy ya he acabado todo lo que quería para el checkpoint, ya que he añadido la vista del detalle de la incidencia, y he añadido las palabras necesarios con sus traducciones. Ya me quedaría: Arreglar la carga del autologin, hacer la vista de las gráficas y poder editar, añadir o eliminar categorías, los filtros con las categorías, y la página de ajustes.

- **Día 16/05/2024 →** Hoy he continuado con el TFC, he creado el servicio de categorías, he añadido el observable de las categorías para poder capturar la colección entera, he continuado con el figa, arreglando cosas y añadiendo cosas nuevas. También he planteado la página de ajustes, quiero implementar una navegación en **breadcrumb**, pero no sé si se quedará la página muy vacía.

- **Día 17/05/2024 →** Hoy he replanteado la página de **about**, cambiando su diseño. He seguido con el figma añadiendo esta página nueva.

- **Día 20/05/2024 →** Hoy he seguido con el figma de la aplicación, quedando solo la página de **Ajustes**.

- **Día 21/05/2024 →** Hoy he añadido la tabla de las categorías al apartado de **Análisis de datos**, he modificado algunas palabras, para que salgan traducidas. He seguido con figma añadiendo la página modal para modificar los usuarios. He añadido la opción de borrar una categoría, también añadiendo el botón para poder editarla.

- **Día 22/05/2024 →** Hoy he arreglado el servicio de las categorías, he añadido un dialog de angular material que sale a la hora de querer borrar una categoría, pero dicha categoría no puede ser borrada si alguna incidencia la usa (YA QUE NO PODEMOS BORRAR INCIDENCIAS), he añadido este nuevo dialog al diseño en figma. También he añadido la actualización de las categorías y la creación de las mismas.

- **Día 23/05/2024 →** Hoy he seguido con el diseño de figma, ya que he añadido la creación de las categorías y su respectiva modificación. He añadido las gráficas de PrimeNG para visualizar en modo de gráfica circular de que categorías son las incidencias y que rol tienen los usuarios existentes. También he añadido un botón para poder descargar los datos desde Firebase y se pasan a .CSV. He seguido con el figma añadiendo las gráficas en la página de **Análisis de datos**. También he añadido la primera versión del filtro de **Home** ya coge bien los datos del formulario usando selectables y lo que me queda es filtrar las incidencias.

- **Día 24/05/2024 →** Hoy he acabado el filtro funcionando correctamente, ya solo me quedaría darle el estilo para hacerlo cómo en figma. Me quedaría toda la página de ajustes y coger los archivos .csv que genero, pasarlos a 1 y tratarlos para hacer el power BI.

- **Día 25/05/2024 →** Hoy he acabado el diseño del filtro para tamaño de tablet/escritorio, me falta el diseño móvil.

- **Día 27/05/2024 →** Hoy he creado el script de Python para transformar los datos de los archivos .csv en un único archivo que se pueda usar en Power BI. También he añadido los archivos para los iconos de la aplicación. Y capacitor, haciendo una vibración según algunas acciones. También he hecho los filtros en el tamaño móvil.

- **Día 28/05/2024 →** Hoy he añadido un dialog a la hora de resolver alguna categoría, al igual que un toast para saber si algo ha fallado o no. También he modificado el figma para añadir estos cambios.

- **Día 29/05/2024 →** Hoy he intentado añadir un cambio de tema en la aplicación pero no ha acabado funcionando.

- **Día 30/05/2024 →** He arreglado el autologin funcionando ya correctamente, he arreglado el filtro para que al cambiar de tamaño siga con los campos y he arreglado el tamaño de las incidencias para que se vea correctamente, también he añadido el archivo _redirects y modificado el archivo de angular.json, para que mi proyecto funcione bien en netlify y que al recargar no te salga el mensaje de que la página no existe.

- **Día 03/06/2024 →** Toda la parte funcional de la app ya estaría hecha, me falta pulir alguna cosa, he acabado todo el diseño en figma, he revisado todos los comentarios y he creado la documentación. También he añadido un botón para ir para atrás en la vista de detalles, la cuál también ha sido añadida a figma. Solo me quedaría el vídeo y subir todas las cosas necesarias a github.

- **Día 10/06/2024 →** Hoy he hecho el vídeo y he acabado todo.
