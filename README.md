# E-CommerceDay2
# Getting Started with Spring Boot

Spring Boot is a framework designed to simplify the development of Java applications, particularly web applications. It builds upon the Spring Framework and provides auto-configuration, embedded servers, and streamlined dependency management, making it easier to create robust applications with minimal setup.

## Understanding Spring Boot MVC
Spring Boot MVC follows the Model-View-Controller (MVC) design pattern to separate concerns and enhance code maintainability. This pattern consists of:

- **Model (M)**: Represents business logic and data handling.
- **View (V)**: Manages UI components, often using templates like Thymeleaf.
- **Controller (C)**: Processes user requests and interacts with the Model and View.

This architecture ensures a clean and scalable structure for web applications.

## How Spring Boot Handles MVC Requests
1. The client (browser or API client) sends an HTTP request.
2. The request is handled by `DispatcherServlet`, the front controller.
3. It maps the request to the appropriate controller method (`@GetMapping`, `@PostMapping`, etc.).
4. The controller communicates with the service layer and retrieves data from the database.
5. The data is passed to the view layer for rendering or returned as JSON.
6. The response is sent back to the client.

## Setting Up Spring Boot Development Environment

To start developing with Spring Boot, follow these steps:

1. **Install Java**: Ensure JDK 17 or later is installed.
2. **Set Up an IDE**: Spring Boot development is best supported in IDEs like:
   - Spring Tool Suite (STS)
   - IntelliJ IDEA
   - Eclipse with Spring plugins
3. **Create a Spring Boot Project**:
   - Use [Spring Initializr](https://start.spring.io/) to generate a project.
   - Choose dependencies like Spring Web, Thymeleaf, and JPA.
4. **Run the Application**:
   - Use the command: `mvn spring-boot:run` (for Maven) or `./gradlew bootRun` (for Gradle).
   
## Example Controller
Below is a simple example of a Spring Boot Controller handling HTTP GET requests:

```java
@RestController
@RequestMapping("/api")
public class HelloController {
    @GetMapping("/hello")
    public String sayHello() {
        return "Hello, Spring Boot!";
    }
}
```   

## Screenshots
![Screenshot 2025-03-22 111007](https://github.com/user-attachments/assets/1c907806-3e8a-4b54-9e41-6e3c2a5c7c8d)
![Screenshot 2025-03-22 111024](https://github.com/user-attachments/assets/be91b303-f4a3-48ef-963b-edd852f700fa)


