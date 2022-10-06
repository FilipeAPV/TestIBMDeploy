#FROM eclipse-temurin:17-jdk-focal
FROM eclipse-temurin:17-jdk-jammy
RUN ls -la 
WORKDIR /app
RUN ls -la
#COPY ./local-path/. /app

COPY .mvn/ .mvn
COPY mvnw pom.xml ./

RUN ls -la

#RUN chmod +x ./mvnw dependency:go-offline
#RUN chmod +x ./mvnw dependency:resolve 
RUN .mvn clean package

RUN ls -la
#RUN chmod +x mvnw dependency:go-offline
COPY src ./src
 
CMD ["./mvnw", "spring-boot:run"]

# syntax=docker/dockerfile:1


