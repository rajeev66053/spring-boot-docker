## Download Docker Desktop for Windows [Downloads](https://docs.docker.com/desktop/windows/install/)


## System requirements
###### Windows 11 64-bit: Home or Pro version 21H2 or higher, or Enterprise or Education version 21H2 or higher.
###### Windows 10 64-bit: Home or Pro 2004 (build 19041) or higher, or Enterprise or Education 1909 (build 18363) or higher.
###### Enable the WSL 2 feature on Windows. For detailed instructions, refer to the Microsoft documentation.


## Create a docker file in spring boot application

## Generate a jar file from spring boot application. Give the jar file name in pom.xml file.

## Run a cmd from application path and run command to build docker image
###### docker build -t spring-boot-docker.jar .


## Check docker image using following command
###### docker image ls


## Run the docker image to run application using following command. Here we can run the application in 9090 port but local application run in 8080 port.
###### docker run -p 9090:8080 spring-boot-docker.jar


## docker tag docker-image-name rajeev66053/docker-image
###### docker tag spring-boot-docker.jar rajeev66053/spring-boot-docker.jar

## Push to docker hub
###### docker push rajeev66053/spring-boot-docker.jar

## To pull docker image
###### docker pull rajeev66053/spring-boot-docker.jar


## Run the pulled docker image
###### docker run -p 9090:8080 rajeev66053/spring-boot-docker.jar