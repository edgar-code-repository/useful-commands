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

-----------------------------------------------------------------------