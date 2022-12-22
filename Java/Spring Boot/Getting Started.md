# Spring Boot

## Getting started

If we are a new to spring boot, the best way to start learning is built a simple application first. In this tutorial I will show how to getting started the **hello world** app.

1. Start a new spring boot project

   We use [start.spring.io](https://start.spring.io/) to initializr our project.

   (add picture and explain the project metadata atribute)

2. Add some code

   Open the file on `src/main/java/com/example/demo` (should explain how this directory is formed). Add some code as the following

   ```
   package com.risma.userservice;

   import org.springframework.boot.SpringApplication;
   import org.springframework.boot.autoconfigure.SpringBootApplication;
   import org.springframework.web.bind.annotation.GetMapping;
   import org.springframework.web.bind.annotation.RequestParam;
   import org.springframework.web.bind.annotation.RestController;

   @SpringBootApplication
   @RestController
   public class UserServiceApplication {

       public static void main(String[] args) {
           SpringApplication.run(UserServiceApplication.class, args);
       }

       @GetMapping("/hello")
       public String hello(@RequestParam(value = "name", defaultValue = "Word") String name) {
           return String.format("Hello %s!", name);
       }
   }
   ```

   \*UserServiceApplication.java is created when the process of initializr and some code in.

   code that should add are:

   - @RestController in the top of `public class UserServiceApplication` (what is the restcontroller mean?)
   - add hello() function

   ````
   @GetMapping("/hello")
       public String hello(@RequestParam(value = "name", defaultValue = "Word") String name) {
           return String.format("Hello %s!", name);
       }
       ```
   ````

   (what are @GetMapping, @requestParam, String.format mean?)

3. Run our app
   Open the terminal--I'm using MacOs, so just provided the command on that. We can build and run the application by issuing the following command:

```
./mvnw spring-boot:run
```

we can add the `--quiet` option (what the function of quiet here?)

```
./mvnw spring-boot:run
```

The output on the terminal will look like this:

![running spring boot](./images/Running%20spring%20boot.png)

The last couple of lines here tell us that Spring has started. Spring Boot’s embedded Apache Tomcat server is acting as a webserver and is listening for requests on localhost port 8080.

Open your browser and in the address bar at the top enter http://localhost:8080/hello. You should get a nice friendly response like this:

![hello world](./images/hello%20world%20app.png)

Add the param name on the url, `http://localhost:8080/hello?name=risma`. It should show `Hello Risma!`
