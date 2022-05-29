# Basic Spring Boot App

Exercice 15 - https://spring.io/guides/gs/spring-boot/

## Commands

- `./mvnw spring-boot:run` to run
- `./mvnw clean package` to build and then `java -jar target/spring-boot-app-0.0.1-SNAPSHOT.jar --server.port=8080`
- Access `http://localhost:8080/`
- or access Actuator `http://localhost:8080/actuator` & `http://localhost:8080/actuator/health`

Spring Boot also has Groovy support, letting you build Spring MVC web applications with as little as a single file:
1. Create ***app.groovy***
```
@RestController
class ThisWillActuallyRun {

    @GetMapping("/")
    String home() {
        return "Hello, World!"
    }

}
```
2. `spring run app.groovy`
3. `curl localhost:8080`
