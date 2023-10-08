
# Développement d'une Application Web avec Spring Boot

## Introduction au Développement Web avec Spring MVC

### Qu'est-ce que Spring MVC ?

Spring MVC est un framework Java pour le développement d'applications Web basées sur le modèle MVC (Modèle-Vue-Contrôleur). Il facilite la création d'applications Web robustes et modulaires.

#### Architecture MVC
- **Modèle :** Représente les données et la logique métier.
- **Vue :** Affiche l'interface utilisateur.
- **Contrôleur :** Traite les requêtes utilisateur et gère les interactions entre le modèle et la vue.

### Utilisation de Thymeleaf pour les Vues

#### Qu'est-ce que Thymeleaf ?

Thymeleaf est un moteur de templates Java qui permet d'intégrer facilement des données dans les vues HTML.

#### Exemple de Code Thymeleaf

```html
<!DOCTYPE html>
<html lang="en" xmlns:th="http://www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <title>Exemple Thymeleaf</title>
</head>
<body>
    <h1 th:text="${message}">Message par défaut</h1>
</body>
</html>
```

### Création de Contrôleurs avec Spring MVC

**Création d'un Contrôleur**

```java

import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.GetMapping;

@Controller
public class MainController {

    @GetMapping("/")
    public String home(Model model) {
        model.addAttribute("message", "Bonjour, c'est une application Web simple !");
        return "index";
    }
}
```

**Configuration de Tomcat**

**Intégration avec Tomcat**

Téléchargez et installez Apache Tomcat sur votre machine.
Ajoutez votre application Web (fichier WAR) dans le dossier webapps de Tomcat.
Démarrez le serveur Tomcat en exécutant startup.sh (Linux) ou startup.bat (Windows).

## Introduction à Spring Boot

### Qu'est-ce que Spring Boot ?

Spring Boot est un projet de Spring qui simplifie le développement d'applications Java en fournissant des configurations par défaut pour démarrer rapidement et facilement un projet.

### Comparaison entre Spring Boot et Tomcat

Spring Boot vs Tomcat

```
Tomcat : Tomcat est un serveur d'application Java qui nécessite une configuration manuelle et peut être utilisé avec Spring MVC.
Spring Boot : Spring Boot intègre un serveur d'application (par défaut, Tomcat) et fournit des configurations par défaut, éliminant ainsi le besoin de configuration manuelle.
```

### Déploiement avec Spring Boot

Comment Déployer avec Spring Boot
Créez un fichier JAR exécutable en utilisant Maven ou Gradle : mvn clean install ou gradle build.
Exécutez l'application en utilisant la commande : 
```cmd
java -jar votrefichier.jar.
```

### Utilisation de Maven avec Spring Boot
Maven et Spring Boot
Maven est un outil de gestion de projets qui facilite la gestion des dépendances et la construction de projets Java.

**Top 10 des Commandes Maven pour Spring Boot**

```
mvn clean install : Compile et construit le projet.
mvn spring-boot:run : Exécute l'application Spring Boot.
mvn clean package : Empaquete l'application dans un fichier JAR.
mvn spring-boot:repackage : Repackage l'application JAR.
mvn dependency:tree : Affiche l'arborescence des dépendances.
mvn spring-boot:stop : Arrête l'application Spring Boot.
mvn spring-boot:start : Démarre l'application Spring Boot en arrière-plan.
mvn spring-boot:build-info : Affiche les informations de build.
mvn clean install -DskipTests : Compile et construit le projet en ignorant les tests.
mvn clean install -Pproduction : Compile et construit le projet avec le profil "production".
```

### Configuration de Port et Page d'Accueil Statique
Changer le Port dans Spring Boot properties
```
# application.properties
server.port=8081
```

###  Ajouter une Page d'Accueil Statique (index.html)

Créez un dossier static ou public dans le répertoire des ressources.
Ajoutez un fichier index.html à ce dossier avec le contenu HTML souhaité.


### Afficher l'Arborescence de Spring Boot

Afficher l'Arborescence du Projet
Utilisez la commande Maven : mvn dependency:tree pour afficher l'arborescence des dépendances.
Utilisez la commande tree (Linux/Unix) ou dir (Windows) pour afficher l'arborescence du projet.

