# Fuseki2 Docker Installation

This project is based the offical FUSEKI documentation on https://jena.apache.org/documentation/fuseki2/fuseki-docker.html

For DevOps who gonna build your own Fuseki2 docker image, this repo provides another documentation on this task.


# Fixed build variables

```
ARG OPENJDK_VERSION=15
ARG ALPINE_VERSION=3.12
ARG JENA_VERSION=4.2.0
```

# Fixed broken alpinelinux APK

The following command has been added to Docker for solving broken APK repo issue
```
RUN echo -e "http://nl.alpinelinux.org/alpine/v3.5/main\nhttp://nl.alpinelinux.org/alpine/v3.5/community" > /etc/apk/repositories

```
# Build image 

```
$ docker-compose build 
```


