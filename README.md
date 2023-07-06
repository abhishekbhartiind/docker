Docker Compose is really useful when we don’t have the development environment setup on our local machine to run all parts of the application to test or we want to run all parts of the application with one command.

For example, if you want to run Next.js and nodeJS express server on different ports and need a single command to set up and run the whole thing. You can accomplish that with Docker Compose.

### What is Docker Compose

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
```
