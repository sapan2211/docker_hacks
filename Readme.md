#########################################
Pre-Reqs
1) Docker is installed and running on your system

#########################################
Basic Docker commands
1) List all running containers
docker ps
2) List all containers including non running containers
docker ps -a
3) List all the images locally available
docker images
4) Delete a docker image
docker rmi <image-id/name>
5)stop a container
docker stop <container-id/name>
6) remove a stopped container 
docker rm <container-id/name> -f
7) run a new container
docker run <image:tag> <shell(/bin/sh)>
	--it connect to interactive terminal
	--name <name> name the container
	--rm remove continer automatically after it exits
	-p <external:internal>
	-v map a volume
	-d detach
8) create a new bash process inside container and connect to terminal
docker exec -it <running/stopped-container-name> <shell(/bin/bash)>
9) logs
docker logs <name>
#########################################
Useful containerization commands
1) Login to account
docker login
2) Build container image using Dockerfile in local folder
docker build -t <name:version-tag> .
3) Get image to local machine
docker pull <name:version-tag>
4) retag a local image
docker tag <old-name:version> <newname:version>
5) push image to accout repo
docker push <name:version-tag>
6) create image from container (useful when customizing image manually)
docker commit <container> <new-name:version>
#########################################
