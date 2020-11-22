Gestionando mi paquete desde la nube
====================================


.. admonition:: Objetivos

   - Añadir un sistema de control de versiones a un proyecto.
   - Sincronizar un paquete de R con la nube.
   - Gestionar el paquete desde la nube.


Ejercicio
---------

En primer lugar, lo que haremos será inicializar un sistema de control de
versiones en nuestro paquete. Para ello, abrimos el paquete desde RStudio y
desde la terminal ejecutamos:

.. code-block:: shell

    git init
    git add *
    git commit -m 'Initial commit'

Esto habrá inicializado el sistema de control de versiones git en nuestro
paquete y habrá realizado el primer *commit*.

Ahora, nos vamos a nuestra cuenta de Github y creamos un nuevo repositorio
público llamado *siq025-practica*.

Una vez creado, para sincronizar nuestro paquete con el repositorio de Github
tenemos que ejecutar los siguientes comandos desde la terminal:

.. code-block:: shell

   git remote add origin https://github.com/<username>/siq025-practica.git
   git push --set-upstream origin master

Si volvemos al navegador y refrescamos la página del repositorio, ya
deberíamos poder ver los archivos del paquete desde Github.

Una vez sincronizado el paquete, vamos a añadir dos nuevas funciones al paquete,
una que haga la multiplicación de dos números y otra que haga la división.

Para ello, lo primero que haremos será crear una nueva rama de git llamada
`mul-div`. Esto lo podemos hacer ejecuntando desde la terminal:

.. code-block:: shell

   git branch mul-div
   git switch mul-div

Creada la nueva rama, tal y como vimos en la sesión anterior, creamos dos nuevos
ficheros llamados ``multiplicacion.R`` y ``division.R``. El primero de ellos
contendrá la siguiente función

.. code-block:: R
   :linenos:

   multiplicacion <- function(a, b) {
       return(a * b)
   }

y el segundo

.. code-block:: R
   :linenos:

   division <- function(a, b) {
       if (b == 0) {
           stop("el divisor no puede ser 0")
       }
       return(a / b)
   }

Realizados los cambios, subimos a Github estos dos ficheros ejecutando desde
la terminal:

.. code-block:: shell
   :linenos:

   git add R/multiplicacion.R
   git add R/division.R
   git commit -m 'Se ha añadido la multiplicacion y la division'
   git push --set-upstream origin mul-div

Para finalizar, tenemos que mezclar los cambios que hemos realizado en la
rama *mul-div* a la rama *master*. Pra ello, tenemos que ir a la
pestaña *Pull Requests* de nuestro repositorio de Github y crear uno nuevo.
La rama *compare* será la rama *mul-dev* y la rama *base* será la rama
*master*. Después de revisar que todo esté correcto, aceptaremos el
*pull request* y lo mezclaremos.

Ahora volvemos a RStudio y desde la consola vamos a cambiarnos a la rama
master y nos la actualizaremos con los cambios que ha introducido el *pull
request* que hemos mezclado. Para ello, ejecutaremos desde la terminal:

.. code-block:: shell

   git switch master
   git pull
   git branch -d mul-dev  # Borra la rama mul-dev

Y si queremos volver a instalar nuestro paquete con las nuevas funciones,
simplemente tenemos que volver a compilar y ejecutar el paquete. De esta
forma, ya podemos calcular la multiplicación y la división de dos números!

.. code-block:: R

   > SIQ025:::multiplicacion(3, 7)
   [1] 21
   > SIQ025:::division(2.6, 2)
   [1] 1.3
   > SIQ025:::division(77, 0)
   Error in SIQ025:::division(77, 0) : el divisor no puede ser 0

