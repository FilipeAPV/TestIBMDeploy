FROM eclipse-temurin:17-jdk-focal
RUN ls -la 
WORKDIR /app
RUN ls -la 
COPY .mvn/ .mvn
COPY mvnw pom.xml ./
RUN ls -la
RUN dos2unix mvnw
RUN chmod +x ./mvnw dependency:go-offline

 
COPY src ./src
 
CMD ["./mvnw", "spring-boot:run"]


