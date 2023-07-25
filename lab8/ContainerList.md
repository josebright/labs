# Containers Lab - Docker

## Listing Container
To list the Docker containers present in your environment, I use the following command:
```
docker ps -a
```

| CONTAINER ID | IMAGE| COMMAND| CREATED | STATUS | PORTS || NAMES |
| -------- | -------- | -------- | -------- | -------- | -------- | -------- |
|2f7939a25039 | postgres:latest  |  "docker-ent..."  |  3 days ago | Up 3 hours | 5432/tcp |  db_server |

## Pulling Latest Ubuntu Image
To pull the latest Ubuntu image from the Docker registry, use the following command:
```
 docker pull ubuntu:latest
```

## Run Container
To run a container using the Ubuntu image you just pulled, use the following command:
```
docker run -it ubuntu
# Or
docker run -it --name my_ubuntu_container ubuntu:latest
```

## Removing Image
To remove the Ubuntu image that was pulled earlier, I used the following command:
```
docker rmi ubuntu:latest
```

If you get error while trying to delete, try to stop the container first by using the command:
```
docker stop <container_id>
```