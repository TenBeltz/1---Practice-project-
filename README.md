# Gestión de Empresas

# Descripción de la Tarea

TenBeltz va a desarrollar un sistema de gestión de empleados para empresas.
Este sistema debe ser capaz de gestionar los siguientes datos:

- Los administradores del sistema (@Michael y @Keyther ), tendrán que registrar las nuevas empresas de forma manual (desde el `panel de administración de Django`)
- De cada empresa, queremos conocer su nombre, ciudad, pais, logo y descripción
- Cada empresa tendrá uno o más gestores (los gestores serán usuarios de `Django contrib auth` ), los administradores del sistema crearán estos usuarios y los asignarán a su respectiva empresa.
- Por lo tanto, debe haber un login, que redirija al usuario al panel de gestión de su empresa, sin embargo, **no debe haber un formulario para crear una cuenta nueva**  ya que esas las crean los administradores.
- En el panel de gestión, los usuarios podrán ver, crear, eliminar y editar:
    - Empleados
    - Departamentos
        - Debe ser posible editar la lista de empleados que forman parte de un departamento
        - Queremos ser capaces de editar el nombre de un departamento
        - Debemos ser capaces de seleccionar el jefe del departamento
- Para cada empleado queremos conocer su nombre, apellido 1, apellido 2, edad, puesto de trabajo, fecha en la que se unió  a la empresa
- Por cada departamento, queremos ver los empleados que lo componen, el nombre del departamento, y quien es el jefe del departamento
- Los gestores podrán seleccionar 1 jefe por cada departamento, y este debe aparecer destacado en la lista de empleados del departamento
- Una vez iniciada sesión, el logo, nombre y descripción de la empresa debe estar presente en todo momento, en todas las páginas del sitio web
- **El proyecto debe estar desplegado** online, en `render.com`

# Entregables

<aside>
ℹ️ Para que el proyecto se considere completo, tendréis que entregar lo siguiente

</aside>

- Un timeline con la planificación que vais a seguir para realizar el proyecto (puede ser cualquier otro formato de organización, no tiene por qué ser una timeline)
- Modelo **Entidad - Relacion**  de la base de datos
- Esquema gráfico de las tablas de `Django` , @Michael tendrá que generarlo utilizando *alguna librería* de python para django.
- Repositorio de **github** con el código fuente del proyecto
- Un **[README.md](http://README.md)** con la documentación del proyecto:
    - Descripción del proyecto.
    - Tecnologías utilizadas.
    - Instrucciones de instalación y configuración del proyecto.
    - Instrucciones de uso del sistema.
    - Créditos y contribuciones.
    - Capturas de pantalla de la web
- Se deberán documentar todos los recursos / documentación utilizados durante el desarrollo de este proyecto. Para ello, cada vez que encontreis algo que no sepais hacer, vais a generar una píldora colaborativa, una píldora colaborativa es un documento con la siguiente información:
    - Autor
    - Fecha
    - Descripción del problema
    - Descripción de la solución
    - URLs/archivos de la documentación y recursos utilizados para resolver el problema

# Normas

- Todas las excepciones deben estar correctamente gestionadas, es decir, no se debe permitir que un usuario introduzca un número en un nombre, etc.
- Al ocasionarse una excepción, el usuario deberá recibir un mensaje de error
- En el frontend, hay que evitar en la medida de lo posible, la redundancia del código, consecuentamente, el header deberá estar en un `.html` a parte, y será reutilizado en el resto de los archivos `.html` mediante las funciones que nos aporta django en el frontend
- La estructura del proyecto de django debe ser la siguiente:
    - Proyecto/
        - manage.py
        - gestionempresas/
            - settings.py
            - urls.py
            - …
        - apps/
            - users/
                - views.py
                - models.py
                - urls.py
                - …
                - templates/
                    - login.html
            - crud/
                - views.py
                - models.py
                - urls.py
                - …
                - templates/
                    - ejemplo.html
                    - …
        
    
    # Compensación 💸
    
    Este proyecto tendrá una pequeña recompensa simbólica para vosotros, el estudiante que muestre un mayor desempeño e interés, **recibirá 10$, y el otro recibirá 5$.** 
    
    Por ello, es importante que os comuniqueis mediante chats a los cuales nosotros tengamos acceso, para poder monitorizar vuestro progreso y evaluaros correctamente.
