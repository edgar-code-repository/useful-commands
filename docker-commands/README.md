DOCKER COMMANDS
-----------------------------------------------------------------------

Useful docker and docker compose commands to work with containers.

-----------------------------------------------------------------------

**Docker commands**


1. Pull image from Docker Hub:

```
    docker pull <tag_name:version>
```

2. Build an image with a Dockerfile (from the same directory where the file is located):

```
    docker build -t <tag_name> .
```

3. Run and stop a container:

```
    docker run -d <tag_name> 

    docker stop <container_id>
```


4. List running containers:

```
    docker ps
```

5. Show logs:

```
    docker logs <container_id>
```

6. List images and containers:

```
    docker images

    docker images -a

    docker container ls

    docker container ls -a
```

7. Delete container:

```
    docker rm <id or name>
```

8. Delete image:

```
    docker rmi <id or name>
```

-----------------------------------------------------------------------

**Docker compose commands**


1. Build docker compose project:

```
    docker-compose build
```

2. Run containers (en detached mode):

```
    docker-compose up -d
```

3. Stop containers:

```
    docker-compose down
```

-----------------------------------------------------------------------