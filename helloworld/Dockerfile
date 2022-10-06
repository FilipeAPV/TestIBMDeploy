#FROM eclipse-temurin:17-jdk-focal
FROM eclipse-temurin:17-jdk-jammy
 
WORKDIR /app
 
COPY .mvn/ .mvn
COPY mvnw pom.xml ./
#RUN chmod +x ./mvnw dependency:go-offline
#RUN chmod +x ./mvnw dependency:resolve 
#RUN mvn clean package

RUN dir /s

COPY src ./src
 
CMD ["./mvnw", "spring-boot:run"]

# syntax=docker/dockerfile:1


