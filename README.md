# Ejemplo 1 con Docker

## Descripcion

Práctica para explicar conceptos básicos de docker.

Tecnologías empleadas:
- Flask
- Docker
    - Dockerfile
    - Docker Compose
- Redis

Estructura del proyecto
```three
.dockerignore
app.py
docker-compose.yml
Dockerfile
README.md
requirements.txt
```

## Comandos

| Acción                                         | Comando                                       |
|------------------------------------------------|---------------------------------------------- |
| Ver la versión de Docker                       | `docker --version`                            |
| Ver información detallada de Docker            | `docker info`                                 |
| Descargar una imagen desde Docker Hub          | `docker pull nombre_de_la_imagen`             |
| Ver todas las imágenes en el sistema           | `docker images`                               |
| Ver todos los contenedores en ejecución        | `docker ps`                                   |
| Ver todos los contenedores (incluso detenidos) | `docker ps -a`                                |
| Crear un contenedor a partir de una imagen     | `docker run nombre_de_la_imagen`              |
| Detener un contenedor                          | `docker stop id_del_contenedor`               |
| Iniciar un contenedor detenido                 | `docker start id_del_contenedor`              |
| Entrar en un contenedor en ejecución           | `docker exec -it id_del_contenedor /bin/bash` |
| Ver logs de un contenedor                      | `docker logs id_del_contenedor`               |
| Eliminar un contenedor                         | `docker rm id_del_contenedor`                 |
| Eliminar una imagen                            | `docker rmi nombre_de_la_imagen`              |
| Ver el uso de recursos de los contenedores     | `docker stats`                                |
| Construir una imagen a partir de un Dockerfile | `docker build -t nombre_de_la_imagen .`       |
| Ver redes disponibles en Docker                | `docker network ls`                           |
