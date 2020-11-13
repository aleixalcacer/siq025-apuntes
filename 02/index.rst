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

.. code-block:: R

    usethis::use_git()

y le decimos que sí a todo.

Esto habrá inicializado el sistema de control de versiones git en nuestro
paquete y habrá realizado el primer *commit*.

Ahora, nos vamos a nuestra cuenta de Github y creamos un nuevo repositorio
público llamado *SIQ025*.

Una vez creado, para sincronizar nuestro paquete con el repositorio de Github
tenemos que ejecutar los siguientes comandos desde la terminal:

.. code-block:: R

   git remote add origin https://github.com/aleixalcacer/siq025-practica.git
   git push --set-upstream origin master

Si volvemos al navegador y refrescamos la página del repositorio, ya
deberíamos poder ver los archivos del paquete desde Github.

