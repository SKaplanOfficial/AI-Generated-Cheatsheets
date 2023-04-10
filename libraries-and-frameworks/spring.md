# Spring Cheatsheet

## Unique Features

- Java-based web framework
- Inversion of Control (IoC) container
- Model-View-Controller (MVC) architecture
- Spring Boot auto-configuration
- Spring Data JPA
- Spring Security

## Controllers

```java
// Define a controller
@Controller
public class ControllerName {
    @GetMapping("/url")
    public String functionName(Model model) {
        // Controller body
        return "template";
    }
}
```

## Views

```html
<!-- Thymeleaf syntax -->
<div th:each="item : ${items}">
    <span th:text="${item.attribute}"></span>
</div>
```

## Forms

```html
<!-- HTML syntax for form -->
<form method="POST" action="/url">
    <input type="text" name="field_name">
    <button type="submit">Submit</button>
</form>

<!-- Handle form submission in controller -->
@PostMapping("/url")
public String functionName(@ModelAttribute ModelName model) {
    // Form handling code
    return "success";
}
```

## Database

```java
// Connect to a database
spring.datasource.url=jdbc:mysql://localhost:3306/db_name
spring.datasource.username=username
spring.datasource.password=password

// Define a model
@Entity
public class ModelName {
    @Id
    @GeneratedValue(strategy = GenerationType.AUTO)
    private Long id;
    private String field_name;
}

// Create a migration
spring.jpa.hibernate.ddl-auto=create
```

## Authentication

```java
// User registration
@PostMapping("/register")
public String registerUser(@ModelAttribute("user") User user) {
    userService.save(user);
    return "redirect:/login";
}

// User login
@GetMapping("/login")
public String login(Model model) {
    model.addAttribute("user", new User());
    return "login";
}

@PostMapping("/login")
public String loginUser(@ModelAttribute("user") User user) {
    if (userService.authenticate(user)) {
        return "redirect:/home";
    } else {
        return "redirect:/login";
    }
}

// User logout
@GetMapping("/logout")
public String logout(HttpSession session) {
    session.invalidate();
    return "redirect:/login";
}
```

## Resources

- [Spring Documentation](https://spring.io/docs)
- [Spring Boot Tutorial](https://spring.io/guides/gs/spring-boot/)
- [Spring Data JPA Tutorial](https://spring.io/guides/gs/accessing-data-jpa/)
- [Spring Security Tutorial](https://spring.io/guides/gs/securing-web/)