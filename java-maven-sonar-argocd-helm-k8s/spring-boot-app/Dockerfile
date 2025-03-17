# Use the correct Java 17 base image
FROM eclipse-temurin:17-jre-alpine

# Define the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the built JAR file into the container
COPY ${artifact} app.jar

# Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "app.jar"]
