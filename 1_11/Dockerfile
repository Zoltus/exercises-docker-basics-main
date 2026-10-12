FROM amazoncorretto:8-jdk

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy files
COPY . .

# Give perm just incase
RUN chmod +x mvnw

# Run file
RUN ./mvnw package

# Expose port
EXPOSE 8080

# Execute file
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
