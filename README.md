## Docker Commands

Docker Commands:

1. `docker run`: Create and run a new container based on an image.

```bash
Example: docker run <image>
```

2. `docker ps`: List running containers.

```bash
Example: docker ps
```

3. `docker images`: List available images.

```bash
Example: docker images
```

4. `docker pull`: Download an image from a registry.

```bash
Example: docker pull <image>
```

5. `docker build`: Build an image from a Dockerfile.

```bash
Example: docker build -t <image_name> <path_to_dockerfile>
```

6. `docker start`: Start a stopped container.

```bash
Example: docker start <container>
```

7. `docker stop`: Stop a running container.

```bash
Example: docker stop <container>
```

8. `docker restart`: Restart a running container.

```bash
Example: docker restart <container>
```

9. `docker rm`: Remove a stopped container.

```bash
Example: docker rm <container>
```

10. `docker rmi`: Remove an image.

```bash
Example: docker rmi <image>
```

11. `docker exec`: Run a command inside a running container.

```bash
Example: docker exec <container> <command>
```

12. `docker cp`: Copy files/folders between a container and the local filesystem.

```bash
Example: docker cp <container>:<path_to_file> <local_path>
```

13. `docker logs`: Fetch the logs of a container.

```bash
Example: docker logs <container>
```

14. `docker inspect`: View detailed information about a container or image.

```bash
Example: docker inspect <container/image>
```

15. `docker network ls`: List Docker networks.

```bash
Example: docker network ls
```

16. `docker network create`: Create a Docker network.

```bash
Example: docker network create <network_name>
```

17. `docker network connect`: Connect a container to a network.

```bash
Example: docker network connect <network> <container>
```

18. `docker network disconnect`: Disconnect a container from a network.

```bash
Example: docker network disconnect <network> <container>
```

## Docker compose Commands

1. docker-compose up: Create and start containers defined in the docker-compose.yml file.

```bash
Example: docker-compose up
```

2. docker-compose down: Stop and remove containers, networks, and volumes defined in the docker-compose.yml file.

```bash
Example: docker-compose down
```

3. docker-compose build: Build or rebuild services defined in the docker-compose.yml file.

```bash
Example: docker-compose build
```

4. docker-compose start: Start services defined in the docker-compose.yml file.

```bash
Example: docker-compose start
```

5. docker-compose stop: Stop services defined in the docker-compose.yml file.

```bash
Example: docker-compose stop
```

6. docker-compose restart: Restart services defined in the docker-compose.yml file.

```bash
Example: docker-compose restart
```

7. docker-compose ps: List containers of services defined in the docker-compose.yml file.

```bash
Example: docker-compose ps
```

8. docker-compose logs: Fetch the logs of services defined in the docker-compose.yml file.

```bash
Example: docker-compose logs
```

9. docker-compose exec: Run a command inside a running service container.

````bash
Example: docker-compose exec <service> <command> 10. docker-compose pull: Download updated images for services defined in the ```
docker-compose.yml file.

```bash
Example: docker-compose pull
````

11. docker-compose rm: Remove stopped containers for services defined in the docker-compose.yml file.

```bash
Example: docker-compose rm
```

12. docker-compose config: Validate and view the composed configuration.

```bash
Example: docker-compose config
```

13. docker-compose scale: Scale services up or down.

```bash
Example: docker-compose scale <service>=<num_instances>
```

14. docker-compose run: Run a one-time command against a service container.

```bash
Example: docker-compose run <service> <command>
```

15. docker-compose pause: Pause services.

```bash
Example: docker-compose pause <service>
```

16. docker-compose unpause: Unpause services.

```bash
Example: docker-compose unpause <service>
```

17. docker-compose up -d: Create and start containers in detached mode.

```bash
Example: docker-compose up -d
```

18. docker-compose down -v: Stop and remove containers, networks, volumes, and images defined in the docker-compose.yml file.

```bash
Example: docker-compose down -v
```

## Introduction of Docker Compose

Docker Compose is really useful when we don’t have the development environment setup on our local machine to run all parts of the application to test or we want to run all parts of the application with one command.

For example, if you want to run Next.js and nodeJS express server on different ports and need a single command to set up and run the whole thing. You can accomplish that with Docker Compose.

## Docker Compose

```
Docker-compose is a tool that is used for multi-container applications in a single host.
As we can see in the following figure, we can run multi containers as services
in a single host with the help of docker-compose.yaml.
```

Once we install `docker-compose`, basically, we need to follow these three steps

1. Define Dockerfile for the service/container
2. Define docker-compose.yaml file with all the services, ports, and other details
3. Run this command docker-compose up

```bash
# create and start containers
docker-compose up
# start services with detached mode
docker-compose -d up
# start specific service
docker-compose up <service-name>
# list images
docker-compose images
# list containers
docker-compose ps
# start service
docker-compose start
# stop services
docker-compose stop
# display running containers
docker-compose top
# kill services
docker-compose kill
# remove stopped containers
docker-compose rm
# stop all contaners and remove images, volumes
docker-compose down

# build with no cache
docker-compose build --no-cache
# start the services
docker-compose up
# list the services
docker-compose ps
# list the containers
docker ps
# stop services
docker-compose stop
```
