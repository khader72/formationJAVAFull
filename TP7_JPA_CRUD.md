# Cours : Gestion des Données avec Spring Boot et Spring Data JPA

## Introduction à la Gestion des Données avec Spring Boot

### Qu'est-ce que Spring Data JPA ?

Spring Data JPA est un projet de Spring qui simplifie l'accès aux données dans les applications Java en intégrant JPA (Java Persistence API) et en offrant des fonctionnalités avancées pour la gestion des bases de données.

### Intégration d'une Base de Données avec Spring Boot

Spring Boot offre une intégration facile avec diverses bases de données relationnelles et non relationnelles, telles que MySQL, H2, PostgreSQL, MongoDB, etc.

## Concepts de Base de Spring Data JPA

### Annotations JPA

- `@Entity`: Marque une classe comme entité JPA.
- `@Id`: Définit la clé primaire de l'entité.
- `@GeneratedValue`: Spécifie la génération automatique de la clé primaire.
- `@OneToMany`, `@ManyToOne`, `@ManyToMany`, `@OneToOne`: Définit les relations entre les entités.

### Repositories

Les repositories Spring Data JPA offrent des méthodes pour effectuer des opérations CRUD (Create, Read, Update, Delete) sur les entités.

- Interface `JpaRepository<T, ID>` : Interface de base pour les repositories JPA.
- Méthodes telles que `save()`, `findById()`, `findAll()`, `deleteById()`.

## Exemple Complet : CRUD avec Spring Boot, Thymeleaf et JPA

### Étape 1 : Configuration de la Base de Données

**`application.properties`**

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/mydatabase
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.hibernate.ddl-auto=update
```

### Étape 2 : Création de l'Entité User

User.java

```java

import javax.persistence.*;

@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    private String username;
    private String email;
    // Getters and Setters
}
```

### Étape 3 : Création du Repository

UserRepository.java

```java

import org.springframework.data.jpa.repository.JpaRepository;

public interface UserRepository extends JpaRepository<User, Long> {
}
```

### Étape 4 : Création du Contrôleur

UserController.java

```java

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.*;

@Controller
@RequestMapping("/users")
public class UserController {

    private final UserRepository userRepository;

    @Autowired
    public UserController(UserRepository userRepository) {
        this.userRepository = userRepository;
    }

    @GetMapping("/")
    public String listUsers(Model model) {
        model.addAttribute("users", userRepository.findAll());
        return "user/list";
    }

    @GetMapping("/create")
    public String createUserForm(Model model) {
        model.addAttribute("user", new User());
        return "user/form";
    }

    @PostMapping("/create")
    public String createUser(@ModelAttribute("user") User user) {
        userRepository.save(user);
        return "redirect:/users/";
    }

    @GetMapping("/edit/{id}")
    public String editUserForm(@PathVariable("id") Long id, Model model) {
        User user = userRepository.findById(id).orElseThrow(() -> new IllegalArgumentException("Invalid user Id:" + id));
        model.addAttribute("user", user);
        return "user/form";
    }

    @PostMapping("/edit/{id}")
    public String editUser(@PathVariable("id") Long id, @ModelAttribute("user") User user) {
        userRepository.save(user);
        return "redirect:/users/";
    }

    @GetMapping("/delete/{id}")
    public String deleteUser(@PathVariable("id") Long id) {
        userRepository.deleteById(id);
        return "redirect:/users/";
    }
}
```

### Étape 5 : Création des Vues Thymeleaf

src/main/resources/templates/user/list.html

```
html

<!DOCTYPE html>
<html lang="en" xmlns:th="http://www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <title>Users</title>
</head>
<body>
    <h1>Users</h1>
    <table>
        <tr th:each="user : ${users}">
            <td th:text="${user.id}"></td>
            <td th:text="${user.username}"></td>
            <td th:text="${user.email}"></td>
            <td><a th:href="@{/users/edit/{id}(id=${user.id})}">Edit</a></td>
            <td><a th:href="@{/users/delete/{id}(id=${user.id})}">Delete</a></td>
        </tr>
    </table>
    <a th:href="@{/users/create}">Create New User</a>
</body>
</html>
```

src/main/resources/templates/user/form.html

```
html
<!DOCTYPE html>
<html lang="en" xmlns:th="http://www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <title>User Form</title>
</head>
<body>
    <h1>User Form</h1>
    <form th:object="${user}" th:action="@{(id != null) ? @{/users/edit/{id}(id=${id})} : @{/users/create}}">
        <input type="hidden" th:field="*{id}"/>
        <label>Username: <input type="text" th:field="*{username}"/></label><br/>
        <label>Email: <input type="text" th:field="*{email}"/></label><br/>
        <input type="submit" value="Save"/>
    </form>
    <a th:href="@{/users/}">Cancel</a>
</body>
</html>
```

### Étape 6 : Tests et Exécution

Créez une base de données MySQL nommée mydatabase.
Exécutez l'application Spring Boot.

Accédez à http://localhost:8080/users/ dans votre navigateur pour accéder à l'application CRUD.
