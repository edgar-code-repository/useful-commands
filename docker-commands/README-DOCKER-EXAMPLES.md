DOCKER EXAMPLES
--------------------------------------------------------------

**Running MySQL 5.7**


Running the container in detached mode (-d option). 

The root password is defined as an environment variable (-e option):

```

docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=password -d mysql:5.7

```

Defining a volume, so your databases and data is not lost when the container is terminated:

```

docker run -p 3306:3306 -v /path/volume:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=password -d mysql:5.7

```

--------------------------------------------------------------