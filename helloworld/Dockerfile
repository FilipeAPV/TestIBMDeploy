FROM eclipse-temurin:17-jdk-focal
RUN ls -la 
WORKDIR /app
RUN ls -la 
COPY .mvn/ .mvn
COPY mvnw pom.xml ./
RUN ls -la
RUN chmod +r pom.xml
#RUN chmod +x ./mvnw dependency:go-offline
RUN chmod +x ./mvn dependency:go-offline
 
COPY src ./src
 
CMD ["./mvnw", "spring-boot:run"]


