# Sping boot example

## run

    mvn clean package && java -jar target\spring-boot-hello-world-1.0.jar

or 

    mvn spring-boot:run

### Test the service

Now that the service is up, visit [http://localhost:8080/hello-world](http://localhost:8080/hello-world), where you see:

	{"id":1,"content":"Hello, World!"}

Provide a `name` query string parameter with [http://localhost:8080/hello-world?name=foo](http://localhost:8080/hello-world?name=foo). Notice how the value of the `content` attribute changes from "Hello, World!" to "Hello foo!":

	{"id":2,"content":"Hello, foo!"}

## see

- [https://spring.io/guides/gs/actuator-service/](https://spring.io/guides/gs/actuator-service/)
- [https://github.com/spring-guides/gs-actuator-service](https://github.com/spring-guides/gs-actuator-service)