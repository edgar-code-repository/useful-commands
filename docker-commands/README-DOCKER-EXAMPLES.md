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

Connecting to MySQL from DBeaver:

![DBeaverWithMySQL](../screenshots/Docker_MySQL_From_DBeaver.png)

--------------------------------------------------------------

**Running Jenkins**


Running the container in detached mode (-d option):

```

docker run -p 8080:8080 -p 50000:50000 -d jenkins/jenkins:lts-jdk11

```

Defining a volume, so your configurations are not lost when the container is terminated:

```

docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -d jenkins/jenkins:lts-jdk11

```

Jenkins running in port 8080:

![Jenkins](../screenshots/Docker_Jenkins.png)

--------------------------------------------------------------

**Running Sonarqube**


Running in detached mode (-d option):

```

docker run -d -p 9000:9000 sonarqube

```

Defining a volume:

```

docker run -d -v /local/path:/opt/sonarqube sonarqube

```

Sonarqube running in port 9000:

![Sonarqube](../screenshots/SonarQube.png)

--------------------------------------------------------------

**Running Nexus**


Running in detached mode (-d option):

```

docker run -d -p 8081:8081 sonatype/nexus3

```

Defining a volume:

```

docker run -d -p 8081:8081 -v /local/path/nexus-volume:/nexus-data sonatype/nexus3

```

Sonarqube running in port 8081:

![Nexus](../screenshots/Nexus_Repository_Manager.png)

--------------------------------------------------------------

**Running PostgreSQL 14.2**


Running in detached mode (-d option):

```

docker run -e POSTGRES_USER=root -e POSTGRES_PASSWORD=pwd -p 5432:5432 -d postgres:14.2

```

Defining a volume:

```

docker run -e POSTGRES_USER=root -e POSTGRES_PASSWORD=pwd  -p 5432:5432 -v /local/path/postgresql:/var/lib/postgresql -d postgres:14.2

```

Connecting to PostgreSQL from DBeaver:

![DBeaverWithPostgreSQL](../screenshots/PostgreSQLFromDBeaver.png)

--------------------------------------------------------------