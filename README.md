# MongOAuth
CRUD API with Java, Spring Boot, MongoDB, and OAuth 2.0.

## Spring Boot:
version 2.2.2

## Dependencies:
* **Spring Web** (spring-boot-starter-web): web application functionality
* **Spring Data MongoDB** (spring-boot-starter-data-mongodb): MongoDB functionality
* **Embedded MongoDB Database** (de.flapdoodle.embed.mongo): embed an in-memory MongoDB database, great for testing and tutorials like this
* **Rest Repositories** (spring-boot-starter-data-rest): needed for the @RepositoryRestResource annotation, which allows us to quickly generate a REST api from our domain classes
* **Okta** (okta-spring-boot-starter): starter that simplifies integrating OAuth 2.0 and OIDC authentication and authorization
* **Lombok** (lombok): a getter, constructor, and setter helper generator via annotations

## Run the application:
./gradlew bootRun

## Test the application
curl http://localhost:8080/fridge
curl -v --header "Content-Type: application/json" -d  "{\"name\":\"milk\",\"owner\":\"Andrew\",\"expiration\":\"01-01-2020\"}" http://localhost:8080/fridge

