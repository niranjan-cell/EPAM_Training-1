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
docker image inspect <image_name/image_id> : To check the details about the image
docker system df : To check the disk usage

docker image rm <image_name/image_id> : To remove the image from local
docker image rm -f <image_name/image_id> : To remove the image from local forcefully
docker image prune -a : To remove all dangling image from local

docker image history <image_name/image_id>: To check the history of the image
