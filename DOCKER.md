# Docker

## Docker Image.
- A Docker Image is a read-only template containing a set of instructions for creating a Docker container.
- Docker images are built from a series of read-only layers. Each instruction in a Dockerfile adds a new layer to the image.
- **Docker Images are Immutable.** Once built, an image cannot be changed. If you need to alter the application code or update a dependency, you must build a new image. 
This immutability guarantees consistency.
- Images can be pushed to a central registry like **Docker Hub**, allowing teams around the world to use the exact same development, testing, and production environments.

## Docker Container.
- A Docker Container is a **runnable instance** of a **Docker Image**.
- A Docker container can be created, started, stopped, moved, or deleted using the Docker API or the Docker CLI.
- Docker takes the read-only image and adds a thin, **temporary read-write layer** on top. Any changes made within the running container like creating new files, modifying logs,
  or installing temporary packages occur in this top read-write layer.

## Useful Docker Command.
| Command   | Description |
|-----------|------------|
|`docker info`| TODO  |
|`docker ps`  | TODO |
|`docker --version`| TODO |
|`docker images` | TODO |
|`docker pull <IMAGE-NAME>` | |
|`docker login` | |
|`docker build -t <IMAGE-TAG> <BUILD-CONTEXT>` | |
|`docker push <IMAGE-NAME>` | |
|`docker inspect <IMAGE-NAME>` | |
|`docker history <IMAGE-NAME>` | |
|`docker exec -it <CONTAINER-ID> bash` | |
|`docker run <IMAGE-NAME>` | |
|`docker create <IMAGE-NAME>` | |
|`docker stop <CONTAINER-NAME>` | |
|`docker restart <CONTAINER-NAME>` | |
|`docker rm <CONTAINER-NAME>` | |
|`docker logs <CONTAINER-NAME>`||
|`docker stats <CONTAINER-NAME>`||
