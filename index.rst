SIQ025 - Software de modelización de sistemas industriales
==========================================================

Bienvenid@s!

Este es el módulo 2 de la asignatura *SIQ025 - Software de modelización
de sistemas industriales* del máster en Matemática computacional de la UJI.

En esta parte de la asignatura veremos cómo podemos gestionar todo el
software que vayamos desarrollando durante nuestra carrera profesional. En
concreto, aprenderemos a crear paquetes de software en el lenguaje de
programación R y a gestionarlos desde la nube usando Github. También veremos
cómo se pueden automatizar tareas que se tienen que ejecutar cada vez que se
modifique el código (por ejemplo, la actualización de la página web del
paquete).

El objetivo final de este módulo es que, al término de este, seais capaces de
implementar un paquete de software (en este caso del lenguaje de programación
de R) y gestionarlo desde la nube.

Motivación
----------

Muchas veces, cuando estamos desarrollando algún proyecto (puede ser desde la
redacción del TFM a la implementación de nuevos algoritmos), cada vez que
añadimos cosas nuevas tendemos a crear una copia de lo anterior.

Por ejemplo, cuando terminé mi TFM, el directorio que lo contenía era algo
parecido a:

..  code-block::

    TFM-dir/
    ├── TFM-1.pdf
    ├── TFM-2.pdf
    ├── TFM-22.pdf
    ├── TFM-3.pdf
    ├── ...
    ├── TFM-def.pdf
    ├── TFM-def2-con_figuras.pdf
    ├── TFM-def4-revisado.pdf
    └── TFM-def4-revisado-final.pdf

Lo mismo ocurre cuando trabajamos con software. Una vez, pedí a otra persona
unos algoritmos que necesitaba y me mandó una carpeta que contenia los
siguientes tres ficheros:

..  code-block::

    ALG-dir/
    ├── algoritmo.R
    ├── algoritmo2.R
    └── algoritmo_revisado.R

Nada más verlos mi primera pregunta fue: *¿Qué fichero tengo que usar?*

No suficiente con eso, una vez supe qué fichero era el bueno, lo abrí el y
me encontré con una función definida de la siguiente forma:

..  code-block::

    algoritmo <- func(a, b, ni, nj, r, d) {
        ...
    }

Así que mi siguiente pregunta fue: *¿Qué significa cada parámetro de la
función?*.

Al final, simplemente con seguir un metodología de trabajo efectiva todos
estos problemas de gestión de proyectos se pueden evitar. Por tanto, en este
módulo veremos una metodología de trabajo basada en el uso de paquetes de R y
su gestión desde la nube. De esta forma, tendremos más localizado y
organizado todo nuestro trabajo y, a la vez,  facilitaremos a la comunidad
científica el uso de nuestros algoritmos.

Un ejemplo de lo que conseguiremos al final de este curso lo podemos
encontrar en `esta web <https://aleixalcacer.github.io/biaa/>`_.

Timeline
--------

Este módulo se dividirá en dos partes muy marcadas. Por un lado, en la
primera parte, que será muy teórica, analizaremos

- El lenguaje de programación R y el IDE RStudio.
- El sistema  de control de versiones Git.
- El entorno web de gestión de software Github.

Por otro lado, en la segunda parte, que será mucho más práctica, veremos
cómo podemos

- Crear un paquete de R.
- Gestionar nuestro paquete desde la nube.
- Documentar nuestro software.
- Crear una página web con toda la información de nuestro paquete.


Evaluación
----------

Respecto a la metodología de evaluación, la nota de este módulo se calculará de
la siguiente forma:

- Parte teórica (10%):
    - Entrega 2 (5%): *Ejercicios sobre R.*
    - Entrega 3 (5%): *Ejercicios sobre Git.*

- Parte práctica (40%):
    - Entrega 5 (10%): *Creación de un paquete de R.*
    - Entrega 6 (10%): *Sincronización del paquete con Github*.
    - Entrega 7 (10%): *Documentación de las funciones.*
    - Entrega 8 (10%): *Creación de una página web del paquete.*

- Trabajo final (40%)
- Participación en clase (10%)


Contacto
--------

Profesor: Aleix Alcacer Sales

Mail: aalcacer@uji.es

Tutorias
++++++++

Todas las tutorias se realizarán de manera virtual. Para establecer
una cita, simplemente con mandar un mail a la dirección anterior será
suficiente.


.. toctree::
   :maxdepth: 2
   :hidden:


