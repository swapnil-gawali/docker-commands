# Docker-Commands

<img src="docker.png" height="150" alt="">

### Images

<br />

* Pull image from registry
```docker image pull <IMAGE_NAME>```

* Inspecting image
```docker image inspect <IMAGE_ID>```

* List all images
```docker image ls```

* Build image from dockerfile with tag 
```docker build -t <DOCKER_ID>/<IMAGE_NAME>:<VERSION> .```

* Tagging existing image
```docker image tag <EXISTING_IMAGE_NAME> <NEW_TAG_NAME>```