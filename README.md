# Docker-Commands

<img src="docker.png" height="150" alt="">

### Images

<br />

* Pull image from registry
```
docker image pull <IMAGE_NAME>
```

* Inspecting image
```
docker image inspect <IMAGE_ID>
```

* List all images
```
docker image ls
```

* Build image from dockerfile with tag 
```
docker build -t <DOCKER_ID>/<IMAGE_NAME>:<VERSION> .
```

* Tagging existing image
```
docker image tag <EXISTING_IMAGE_NAME> <NEW_TAG_NAME>
```


### Containers

<br />

* list all containers
```
docker container ls || docker container ls -a || docker container ps || docker container ps -a
```

* Inspecting container
```
docker container inspect <CONTAINER_NAME>
```

* Running container
```
docker container run <IMAGE_NAME>
```

* Assigning name & run container
```
docker container run --name <CUSTOM_NAME> <IMAGE_NAME>
```

* Assigning name, port & run container
```
docker container run --name <CUSTOM_NAME> --publish <OUTSIDE_PORT>:<CONTAINER_PORT> <IMAGE_NAME>
```

* Assigning name, port & run container in background (-d || --detach)
```
docker container run --name <CUSTOM_NAME> --publish <OUTSIDE_PORT>:<CONTAINER_PORT> --detach <IMAGE_NAME>
```

* Stop container gracefully within 10 seconds
```
docker container stop <CONTAINER_ID>
```

* Stop container immediately
```
docker container kill <CONTAINER_ID>
```

* Starting container
```
docker container start <CONTAINER_ID>
```

* Display the running processes of a container
```
docker container top <CONTAINER_ID>
```

* Fetch the logs of a container
```
docker container logs <CONTAINER_ID>
```

* Display a live stream of container(s) resource usage statistics like RAM, CPU, IO
```
docker container stats <CONTAINER_ID>
```

* Running command inside running container (-it used for interactive tty)
```
docker container exec -it <CONTAINER_ID> /bin/bash || docker container exec -it <CONTAINER_ID> sh
```

* Pause container
```
docker container pause <CONTAINER_ID>
```

* Un-Pause container
```
docker container unpause <CONTAINER_ID>
```

* Stop and remove container forcefully
```
docker container rm -f <CONTAINER_ID>
```

* Remove all stopped containers
```
docker container prune
```

* Remove all stopped containers forcefully
```
docker container prune -f
```

* List all ports assigned to container
```
docker container port <CONTAINER_ID>
```

* Exposing container port to outside
```
docker container --expose <PORT_NUMBER> <IMAGE_NAME>
```
