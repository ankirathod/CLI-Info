## Docker

``docker images`` or ``docker image ls`` list docker images

``docker build -t <tag> .`` build docker image based on the docker file in current location and add tag

``docker build -t <tag> -f <Dockerfile path>`` build docker image based on the docker file located at specific path and add tag

``docker containers`` or ``docker container ls`` list all running containers 

``docker container ls -a`` list all containers

``docker rm [image-name/container-name]`` remove image or container

``docker rm -v $(docker ps --filter status=exited -q)``  remove containers based on the status