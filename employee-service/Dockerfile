# Use the official Tomcat 9 image as the base
FROM tomcat:9-jdk11-openjdk-slim

# Set the working directory in the container
WORKDIR /usr/app

# Copy the JAR file into the container at /usr/app
COPY target/employee-service-0.0.1-SNAPSHOT.jar /usr/app/employee-service.jar

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Run the jar file 
ENTRYPOINT ["java", "-jar", "employee-service.jar"]