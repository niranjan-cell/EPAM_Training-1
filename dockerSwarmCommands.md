```
docker swarm init : To initialize the swarm cluster
docker node ls : To list the nodes available in the cluster
docker swarm join-token worker : To get the join token for worker
docker swarm join-token manager : To get the join token for manager
docker swarm leave : To leave the swarm cluster 
docker node rm <hostname_of_worker_node/workerid> : To remove node from swarm cluster
docker node inspect <hostname_of_worker_node/workerid> : To inspect the node
docker node demote <hostname_of_worker_node/workerid> : To demote as worker
docker node promote <hostname_of_worker_node/workerid> : To demote as manager

docker service create -d -p <host_port>:<container_port> --replicas <no_of replicas> <image_name>: To create a service in swarm cluster
docker service ls : To list the service
docker service rm <service_id> : To remove the service
docker service ps <service_id> : To list the task started by service
docker service scale <service_id>=<no_of_replicas> : TO scale up or scale down the service
docker service logs <service_id> : To check the logs of the service
docker service create --mode=global -d alpine ping google.com : To start container in global mode
docker node update --label-add="key=value" <hostname_of_worker_node/workerid> : TO add the label to node
docker service create --constraint node.labels.key==value --replicas=2 -d <image_name> : TO run the service in those node where we have the specific label
docker service create --constraint node.role==manager --replicas=2 -d <image_name> : To run the service in manager
https://docs.docker.com/engine/reference/commandline/service_create/

```