FROM amazoncorretto:8-alpine

EXPOSE 8080

WORKDIR /usr/src/app

# Copy all of source code
COPY . .

# Build project
RUN ./mvnw package

# Run app
CMD [ "java", "-jar", "./target/docker-example-1.1.3.jar" ]
