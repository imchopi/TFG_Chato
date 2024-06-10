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

Nuestro objetivo para este proyecto, es poder ayudar a las empresas mediante una aplicación de incidencias, para que el usuario pueda enviar la incidencia al administrador y este resolverla. También mediante las categorías, tanto el usuario como el adminsitrador, tendrá mas claro el tipo de problema para resolver la incidencia con mayor facilidad.

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




