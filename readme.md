<h1 align="center">Hi 👋, I'm Edgar Ronaldo Henao Villarreal</h1>
<h3 align="center">A full-stack developer from Colombia. Passionate to games and some coffee</h3>

- 🌱 I’m currently learning **React and Spark**

- 👨‍💻 All of my projects are available at [https://github.com/ronis97](https://github.com/ronis97)

- 💬 Ask me about **Java, Python, Sql, HTML, CSS**

- 📫 How to reach me **ronivillarreal@hotmail.com**

- 📄 Know about my experiences [Simple project development POO](Simple project development POO)

- ⚡ Fun fact **I hate bugs**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/www.linkedin.com/in/edgar-ronaldo-henao-villarreal" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="www.linkedin.com/in/edgar-ronaldo-henao-villarreal" height="30" width="40" /></a>
<a href="https://fb.com/www.linkedin.com/in/edgar-ronaldo-henao-villarreal" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="www.linkedin.com/in/edgar-ronaldo-henao-villarreal" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://codeigniter.com" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/codeigniter.svg" alt="codeigniter" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://heroku.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/heroku/heroku-icon.svg" alt="heroku" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.oracle.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/oracle/oracle-original.svg" alt="oracle" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://unity.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/unity3d/unity3d-icon.svg" alt="unity" width="40" height="40"/> </a> </p>

## Comandos maven

```
maven package
```

```
mvn archetype:generate -DgroupId=edu.escuelaing.arep -DartifactId=app -DarchetypeArtifactId=mavenarchetype-quickstart -DinteractiveMode=false
```

```
mvn exec:java -Dexec.mainClass="edu.escuelaing.arep.HttpServer"
```

```
mvn clean install
```

```
heroku local web
```

```
heroku create
```

```
git push heroku main
```
heroku open

```
heroku git:remote -a <nombre>
```
```
echo "Docker File" > DockerFile
```

## Comandos Docker

#### Construir imagen
```
docker build --tag dockersparkprimer .
```
#### Mapear puertos
```
docker run -d -p 34002:6000 --name firstdockercontainer3 dockersparkprimer
```
#### Union instancias contenedores
```
docker-compose up -d
```
#### Referencia local docker imagen
```
docker tag dockersparkprimer dnielben/firstsprkwebapprepo
```
#### Push al repo en docker (antes hacer login)
```
docker push dnielben/firstsprkwebapprepo:latest
```
#### Cambiar nombre repositorio (opcional)
```
docker tag primer-docker-spark:latest dnielben/primersparkweb:latest
```
## AWS
```
sudo yum update -y
```
```
sudo yum install docker
```

```
sudo service docker start
```
```
sudo usermod -a -G docker ec2-user
```
```
docker run -d -p 42000:6000 --name firstdockerimageaws dnielben/firstsprkwebapprepo
```
#### Dockerfile:
```
FROM openjdk:8

WORKDIR /usrapp/bin

ENV PORT 6000

COPY /target/classes /usrapp/bin/classes
COPY /target/dependency /usrapp/bin/dependency

CMD ["java","-cp","./classes:./dependency/*","co.edu.escuelaing.sparkdockerdemolive.SparkWebServer"]
```

#### docker-compose.yml:
```
version: '2'


services:
  web:
    build:
      context: .
      dockerfile: Dockerfile
    container_name: web
    ports:
      - "8087:6000"

  db:
    image: mongo:3.6.1
    container_name: db
    volumes:
      - mongodb:/data/db
      - mongodb_config:/data/configdb
    ports:
      - 27017:27017
    command: mongod

networks:
  red1:
    driver: bridge

volumes:
  mongodb:
  mongodb_config:
  ```
  
  #### POM:
  
   ```
  <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
    <modelVersion>4.0.0</modelVersion>
    <groupId>edu.escuelaing.arep</groupId>
    <artifactId>Taller4AREP</artifactId>
    <packaging>jar</packaging>
    <version>1.0-SNAPSHOT</version>

    <name>Taller4AREP</name>
    <url>http://maven.apache.org</url>
    <properties>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
        <maven.compiler.source>8</maven.compiler.source>
        <maven.compiler.target>8</maven.compiler.target>
    </properties>
    <dependencies>
        <dependency>
            <groupId>com.sparkjava</groupId>
            <artifactId>spark-core</artifactId>
            <version>2.9.2</version>
        </dependency>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>3.8.1</version>
            <scope>test</scope>
        </dependency>
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-simple</artifactId>
            <version>1.7.32</version>
            <scope>compile</scope>
        </dependency>
        <dependency>
            <groupId>org.mongodb</groupId>
            <artifactId>mongodb-driver</artifactId>
            <version>3.0.4</version>
        </dependency>
    </dependencies>
    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-dependency-plugin</artifactId>
                <version>3.0.1</version>
                <executions>
                    <execution>
                        <id>copy-dependencies</id>
                        <phase>package</phase>
                        <goals><goal>copy-dependencies</goal></goals>
                    </execution>
                </executions>
            </plugin>
        </plugins>
    </build>
</project>
 ```
 
 #### Generacion llave segura:
 ```
 keytool -genkeypair -alias ecikeypair -keyalg RSA -keysize 2048-storetype PKCS12 -keystore ecikeystore.p12 -validity 3650
 ```
