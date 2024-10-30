# api-store

## Description

This project consists of creating a REST endpoint that allows
data belonging to a specific spaceship to be recovered.
This api was writing in Java 17 with maven and H2 database. Database
creating and inserting data automatically on the start of application.

## Run in local environment

Need to add in environment variables:

-Dspring.profiles.active=local

# Start the application:

- **Maven install:** Do a Maven install `mvn install`
- **Run test:** Execute the following maven
  command `mvn test`
- **Web App:** To start the embedded server from the command line use `mvn spring-boot:run`, or run
  StoreApplication class.
- **Swagger Documentation:** available at  `localhost:9030/swagger-ui.html`
- **Code coverage report:** available
  at  `http://localhost:63342/api-spaceship/target/site/jacoco/index.html`


## Curl of endpoint

curl


Architecture:

- Application: contains domain model, service and port
- Adapter: contains repository(out) and controller (in)
- Commons: contains configuration, utils, constants and exceptions

- Used @ControllerAdvice to manage exceptions to avoided using try-catch blocks.
- Used flyway to automatically run database.
- Used Facade, Builder patterns
- Used Validator custom annotation for fields
- Used Jacoco for code coverage report

## Conclusion.

I have made the project small and simple based on the presented task.
Of course, in a real project there would be a different structure and there would be more logic
and different implementations.

