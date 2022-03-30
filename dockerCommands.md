```
docker image pull <image_name> : To pull image
docker image ls : To list the images in the local
docker container ls : To list all the running container
docker container run -it <image_name>:<version> : To create a container
docker container run -it -d <image_name>:<version> : To create a container with detached mode
docker container run --name <container_name> -it -d <image_name>:<version> : To create a container with detached mode
docker container stop <container_id/container_name> : To stop the container
docker container start <container_id/container_name> : To start the container
docker container restart <container_id/container_name> : To restart the container
docker container pause <container_id/container_name> : To pause the container
docker container unpause <container_id/container_name> : To unpause the container
docker container kill <container_id/container_name> : To kill the container
docker container top <container_id/container_name> : To see all the processes running inside the container
docker container rename <container_id/container_name> <new_name> : To rename the container
docker container inspect <container_id/container_name> : To see all the details about the continer
docker container exec <container_id/container_name> <command> : To run command inside container
docker container exec -it <container_id/container_name> bash : To go inside the container
docker container run -it -d -p <host_port>:<container_port> <image_name>:<version> : For port mapping
docker container cp <source> <container_id>:<destination> : To copy file or directory from host to container
docker container logs <container_id/container_name> -f : To see the container log
docker container commit <container_id/container_name> <image_name> : To take a snapshot of running container

docker system df : To check the disk usage

docker image rm <image_name/image_id> : To remove the image from local
docker image rm -f <image_name/image_id> : To remove the image from local forcefully
docker container ls -q : TO get all running container id
docker container ls -aq : TO get all container id
docker container rm -f $(docker container ls -aq) : To remove all container from host
docker container stats : To check the memory and cpu utilization of the containers

docker image ls : To check all the local image
docker image tag <image_name_u_want_to_tag> <dockerhub_id>/image_name:[tag] : TO tag the image
docker image push <image_name>:[tag] : To push the image
docker image inspect <image_name/image_id> : To check the details about the image
docker image pull <image_name>:[tag] : TO pull the image 

docker image prune -a : To remove all unused image from local
docker image save <image_name>:[tag] > file_name.tar : To create tar file from the image
docker image load < file_name.tar : To create image from tar file

docker image history <image_name/image_id>: To check the history of the image
```