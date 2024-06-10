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
    - Día 08/04/2024 -> Ya que no nos han proporcionado el feedback del anteproyecto, he realizado el diseño de la página de Login y la de Registro en Figma. Este diseño es el básico (sin texto, ni colores, etc).
</br>
- Día 09/04/2024 -> Hoy he creado el repositorio, añadido todos los servicios principales Autenticación, Traducción). Y he creado la página de Access que contendrá el componente de LogIn y el de Register. He       hecho un pequeño formulario de Login usando Angular Material, aún falta estilo y que pueda hacer Login y registro.
</br>
- Día 10/04/2024 -> Hoy le he añadido estilo a la página de acceso, a los componentes de registro y de login, he añadido un validador para saber si las contraseñas coinciden. He añadido a los formularios los        errores. He arreglado algunas propiedades mal escritas en las interfaces y he agregado el registro y el logueo conectándose al Backend en Firebase.
</br>
- Día 11/04/2024 -> Añadida la guarda para tener que estar logueado en la aplicación para poder navegar en las páginas que no sean las de acceso, he cambiado el estilo del formulario de registro, ya que he          arreglado los errores que seguían saliendo al registrarse, he arreglado las interfaces (añadiendo los atributos role y surname, y he eliminado los atributos firstSurname y secondSurname) y he agregado una         guarda para que solo los usuarios con el rol de Admin puedan acceder, ya que la página es de administración.
</br>
- Día 12/04/2024 -> He añadido PrimeNG al proyecto, ya que quiero tener toast personalizados en algunas partes de la aplicación, he creado el logo de la app, y he cambiado la pantalla de acceso para que este        salga en los dispositivos con pantallas más pequeñas (ya que en tamaño grande sale una imagen a la derecha de los formularios), he añadido un toast que sale al registrarte ya que solo puedes acceder a mi parte    de la aplicación si eres admin (por defecto en el registro es usuario normal, un admin te tiene que cambiar el role). Me falta poner toast en los fallos del login (y ver cómo recoger el error de que un gmail ya   está en uso) para acabar con la página de acceso.
</br>
- Día 16/04/2024 -> He empezado el diseño de la página Home, la cual contendrá todas las incidencias que van dejando los usuarios, desde allí podremos navegar a cada una de las incidencias, al igual que aplicarle   filtros a la vista general y acceder al menú de la aplicación. También he diseñado la vista de la página con el menú abierto. También he añadido toast con errores al hacer un registro(el de correo en uso), en     el login, me da error y sale el error aun que esté bien y después ya carga y lleva a Home (HABLAR CON JUAN, SOLUCIONADO).
</br>
- Día 17/04/2024 -> He arreglado el problema con los toast a la hora de iniciar sesión y registrarse (arreglando también su tamaño). También he añadido el header de la aplicación, con un menú lateral y el logo de   la app.
</br>
- Día 18/04/2024  He añadido el SplashScreen para que al recargar la página no vaya a Access y después navegue a Home, he usado un lottie para que se vea una animación mientras tanto. También he empezado a crear   el diseño final de la aplicación. Al crear el SplashScreen me ha empezado a dar errores ya que al hacer el deslogueo del usuario, al volver a Access había una capa invisible por encima de la página y se quedaba   inutilizable, lo he arreglando borrando el component de header y pasando todo el header y el menú a app.component.html, aun que creyendo que era el SplashScreen lo he acabado borrando, más adelante lo pondré.
</br>
 - Día 19/04/2024 -> Hoy he implementado ya la captura de datos desde Firebase, para obtener los datos de los usuarios logueados en la aplicación, he acabado la estética del menú lateral y he implementado todas    las páginas que incluye dicho menú.
 </br>
 - Día 22/04/2024  Hoy he agregado una tabla para poder ver la información de todos los usuarios conectados, también he añadido un tab para ver la información o los datos en forma de gráficas. También he añadido la vista de la información detallada de los usuarios. Y también el update de los usuarios.
  </br>
 - Día 23/04/2024 -> Hoy he cambiado la forma en la que tenía el update de los usuarios, ya que no cambiaba correctamente los datos, y al modificar el usuario conectado no se actualizaba el observable de user$. También he estado modificando el menú para añadir la foto del usuario y abajo de dicho menú con la opción de navegar a la página de About. He incluido el contenido de dicha página, incluyendo la información de los repos de Adri y mía.
   </br>
- Día 25/04/2024 -> Hoy he avanzado con los diseños de la aplicación en Figma.
</br>





