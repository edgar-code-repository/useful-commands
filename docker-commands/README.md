DOCKER COMMANDS
-----------------------------------------------------------------------

Useful docker commands to pull, build and run containers.

-----------------------------------------------------------------------

**Pull image from Docker Hub:**

```

docker pull <tag_name:version>

```

**Build an image with a Dockerfile (from the same directory where the file is located):**

```

docker build -t <tag_name> .

```

**Run and stop a container:**

```

docker run -d <tag_name> 

docker stop <container_id>

```


**List running containers:**

```

docker ps

```

**Show logs:**

```

docker logs <container_id>

```

**List images and containers:**

```

docker images

docker images -a

docker container ls

docker container ls -a

```

**Delete container:**

```

docker rm <id or name>

```

**Delete image:**

```

docker rmi <id or name>

```

-----------------------------------------------------------------------