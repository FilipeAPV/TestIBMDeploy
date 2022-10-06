#FROM eclipse-temurin:17-jdk-focal
#RUN ls -la 
#WORKDIR /app
#RUN ls -la 
#COPY .mvn/ .mvn
#COPY mvnw pom.xml ./
#RUN ls -la

#RUN chmod +x ./mvnw dependency:go-offline

 
#COPY src ./src

FROM eclipse-temurin:17-jdk-focal
FROM maven:3.8.3-openjdk-17
RUN mvn clean package
CMD ["./mvn", "spring-boot:run"]


