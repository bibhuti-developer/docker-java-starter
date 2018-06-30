# docker-java-starter

## Dockerfile for Maven-Based GitHub Projects  
Refer   : Dockerfile  
### Images: ###  
1. alpine/git  
2. maven:3.5-jdk-8-alpine  
3. openjdk:8-jre-alpine  

Command :  
```javascript
docker build 
  --build-arg url=<git url>\
  --build-arg project=<project>\
  --build-arg artifactid=<artiface id>\
  --build-arg version=<project version>\
  -t <project-tag-name> - < Dockerfile
```
```javascript
docker run -ti -p8080:8080 <project-tag-name>
```
