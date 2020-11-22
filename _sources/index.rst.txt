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

Muchas veces, cuando estamos creando alguna cosa (puede ser el TFM, nuevos
algoritmos...) tendemos a ir creando copias cada vez que añadimos cosas
nuevas. Por ejemplo, cuando terminé mi TFM, el directorio era algo parecido a:

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

Lo mismo ocurre cuando trabajamos con software. Una vez, pedí unos algoritmos
y me mandaron una carpeta que contenia los siguientes tres ficheros:

..  code-block::

    ALG-dir/
    ├── algoritmo.R
    ├── algoritmo2.R
    └── algoritmo_revisado.R

Por tanto, mi primera pregunta fue: *¿Qué fichero tengo que usar?*

No suficiente con eso, una vez supe qué fichero uitlizar, abrí el fichero y
ví que la función estaba definida de la siguiente forma:

..  code-block:: 3

    algoritmo <- func(a, b, ni, nj, r, d) {
        ...
    }

Así que mi siguiente pregunta fue: *¿Qué significa cada parámetro?*.

Por tanto, en este módulo veremos cómo podemos evitar todo esto mediante el
uso de paquetes de R y su gestión desde la nube. De esta forma, facilitaremos
el uso de nuestros algoritmos a la comunidad científica y, a la vez,
tendremos más organizado y localizado todo nuestro trabajo.

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


