# Anteproyecto

Created: March 26, 2024 4:01 PM

# Título del proyecto

Chato

# Nombre de los autores

- Javier Miguel Martín Gallardo, se enfocará en la parte de Angular e Ionic
- Adrián Perogil Fernández, hará la parte de Android

# Descripción

Nuestro proyecto se basará en una aplicación enfocada en las incidencias de una empresa, en la cuál estará implicado un administrador y un usuario, siendo este último quien podrá subir las incidencias para que el administrador las pueda solucionar. Acciones que puede usar cada rol:

- **ADMINISTRADORES**
    - Gestión de  usuarios.
    - Comunicación directa con los usuarios mediante un chat.
    - Gestión de incidencias.

- **USUARIOS**
    - Gestión de su propio perfil.
    - Visualización de sus incidencias.
    - Creación de incidencias.
    - Comunicación directa con el administrador al crear una incidencia.

# Objetivos del proyecto

Nuestro objetivo para este proyecto, es poder ayudar a las empresas mediante una aplicación de incidencias, para así poder comunicarse con los usuarios que tienen problemas a la hora de trabajar, queremos añadir un chat entre ambos roles de la aplicación para hacer más amena la forma de arreglar dichos incidentes.

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
    - Usaremos esta estrategia para los documentos de incidentsInfo y chatInfo ya que necesitaremos mezclar datos de ambos documentos, así conseguiremos con una consulta, extraer toda la información.

![image](https://github.com/imchopi/TFG_Chato/assets/92975232/8148a595-1e41-42da-8fe7-f69c63cbf570)
