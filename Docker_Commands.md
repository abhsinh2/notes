Take help from docker

```docker --help```

```docker run --help```

```docker version```

```docker info```

Search a contianer in docker hub

```docker search <IMAGE_NAME>```

```docker pull <IMAGE_NAME>```

```docker images```

```docker pull <IMAGE_NAME>:<VERSION>```

Run a docker. The '-p 8080:80' tells Docker to map your localhost port 8080 to Docker container's port 80.

```docker run -p 8080:80 <IMAGE_NAME>```

Run in detached mode

```docker run -p 8080:80 -d <IMAGE_NAME>```

Run with name

```docker run --name <MY_IMAGE_NAME> -p 8888:80 -d <IMAGE_NAME>```

```docker ps```

```docker ps -a```

```docker stop <MY_IMAGE_NAME>```

```docker start <MY_IMAGE_NAME>```

```docker restart <MY_IMAGE_NAME>```

```docker kill <MY_IMAGE_NAME>```

Execute bash

```docker run --name <MY_IMAGE_NAME> -it <IMAGE_NAME>:latest bash```

Docker ssh into container '<MY_IMAGE_NAME>'

```docker exec -it <MY_IMAGE_NAME> bash```

```
docker run -it -d --name <MY_IMAGE_NAME> <IMAGE_NAME>:latest bash
docker attach <MY_IMAGE_NAME>
```

Check history of image

```docker history <IMAGE_NAME>```

find out low-level information about your system

```
docker inspect <CONTAINER_ID>
docker inspect <CONTAINER_ID> | grep "IPAddress"
```

Copy files from local machine to container

```docker cp index.html <MY_IMAGE_NAME>:/root```

Create own image from running container

```
docker stop <MY_IMAGE_NAME>
docker ps -a
docker commit <CONTAINER_ID> <NEW_IMAGE_NAME>
docker images
docker run -it -d -p 8888:80 <NEW_IMAGE_NAME>
```

Removing container

```docker rm <CONTAINER_ID_1> <CONTAINER_ID_2>```

Removing images

```docker rmi <IMAGE_1> <IMAGE_2>```





