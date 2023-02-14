# Docker + Python

---
## Creamos contenedor sencillo de Python:
    docker run -it --rm -v C:\Users\roima\PycharmProjects\DockerPython:/usr/src/myapp -w /usr/src/myapp python:3 python main.py

``docker`` es el comando base

``run`` crea el contenedor

``-it`` son dos opciones que sirven para interactuar con la terminal del contenedor

``--rm`` borra el contenedor al terminar la acción

``-v`` define el mapeo del volumen a continuación

- ``"$PWD"`` constante para el directorio donde estamos (En Windows no funciona)
- ``/usr/src/myapp`` el directorio dentro del contenedor

``-w`` es el directorio de trabajo (_workdir_)

``python:3`` la imagen

``python main.py`` comando a ejecutar en el contenedor 