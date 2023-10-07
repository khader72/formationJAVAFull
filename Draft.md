
Plan de formation Java Web sur 3 jours

Jour 1
Introduction à Java
Définition du langage Java
Java est un langage de programmation objet-orienté, compilé, à typage fort et à portée statique.
Il est développé par Oracle Corporation et est utilisé pour développer une variété d'applications, notamment des applications web, des applications mobiles et des applications de bureau.
Installation de l'environnement de développement Java
Pour développer des applications Java, vous avez besoin d'un environnement de développement Java (IDE).
Il existe de nombreux IDE Java disponibles, tels que Eclipse, IntelliJ IDEA et NetBeans.
Écriture d'un premier programme Java
Voici un exemple de programme Java simple :
Java
public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello, world!");
    }
}
Utilisez le code avec précaution. En savoir plus
Ce programme affiche le message "Hello, world!" dans la console.

Jour 1
Introduction à Java
Qu'est-ce que Java ?
Installation de l'environnement de développement Java
Les bases de la programmation Java
Variables
Types de données
Opérations
Conditions
Boucles
Fonctions
Diapositives du Jour 1

Diapositive 1

Titre : Introduction à Java
Sous-titre : Qu'est-ce que Java ?
Diapositive 2

Java est un langage de programmation orienté objet
Créé par Sun Microsystems en 1995
Open source et gratuit
Utilisé pour développer des applications Web, mobiles, de bureau et d'entreprise
Diapositive 3

Installation de l'environnement de développement Java
Diapositive 4

Les bases de la programmation Java
Variables
Types de données
Opérations
Conditions
Boucles
Fonctions
Explications

Diapositive 2

Java est un langage de programmation orienté objet

Les objets sont des entités qui ont des propriétés et des méthodes
Les propriétés sont des données associées à un objet
Les méthodes sont des actions qu'un objet peut effectuer
Créé par Sun Microsystems en 1995

Sun Microsystems a été racheté par Oracle en 2010
Open source et gratuit

Java est un logiciel open source, ce qui signifie qu'il est disponible gratuitement et que son code source est accessible à tous
Utilisé pour développer des applications Web, mobiles, de bureau et d'entreprise

Java est un langage de programmation polyvalent qui peut être utilisé pour développer une grande variété d'applications
Diapositive 3

Les variables

Les variables sont utilisées pour stocker des données
Les variables doivent être déclarées avant utilisation
Les variables peuvent être de différents types de données
Types de données

Les types de données définissent le type de données qu'une variable peut contenir
Les types de données primitifs sont les types de données de base de Java
Les types de données non primitifs sont des types de données complexes qui sont construits à partir de types de données primitifs
Opérations

Les opérations sont utilisées pour effectuer des calculs sur des données
Les opérations arithmétiques sont les opérations les plus courantes
Conditions

Les conditions sont utilisées pour tester des conditions et prendre des décisions
Les instructions if et else sont utilisées pour tester des conditions simples
Les instructions switch sont utilisées pour tester des conditions complexes
Boucles

Les boucles sont utilisées pour répéter des instructions
Les instructions for et while sont utilisées pour répéter des instructions un nombre fixe de fois
Les instructions do-while sont utilisées pour répéter des instructions jusqu'à ce qu'une condition soit remplie
Fonctions

Les fonctions sont des blocs de code qui peuvent être réutilisés
Les fonctions sont déclarées avec la mot-clé function
Exemple

Java
public class HelloWorld {

    public static void main(String[] args) {
        // Déclaration d'une variable
        int age = 25;

        // Affichage de la valeur de la variable
        System.out.println(age);

        // Calcul de l'âge de l'utilisateur dans 10 ans
        int ageDansDixAns = age + 10;

        // Affichage du résultat du calcul
        System.out.println("L'âge de l'utilisateur dans 10 ans sera de " + ageDansDixAns);

        // Condition
        if (age >= 18) {
            System.out.println("L'utilisateur est majeur");
        } else {
            System.out.println("L'utilisateur est mineur");
        }

        // Boucle
        for (int i = 0; i < 10; i++) {
            System.out.println(i);
        }

        // Fonction
        sayHello

Les bases de la programmation orientée objet
Classes et objets
En programmation orientée objet, les données et les comportements sont organisés dans des classes.
Une classe est un modèle qui définit les attributs et les méthodes d'un objet.
Un objet est une instance d'une classe.
Héritage
L'héritage permet à une classe d'hériter des attributs et des méthodes d'une autre classe.
Cela permet de réutiliser le code et de simplifier la maintenance du code.
Encapsulation
L'encapsulation permet de cacher les détails de l'implémentation d'une classe.
Cela permet de rendre le code plus maintenable et plus évolutif.
Interfaces
Une interface est un contrat qui définit les méthodes que doivent implémenter les classes qui la mettent en œuvre.
Cela permet de créer des relations entre des classes qui n'ont pas de relation d'héritage.
Exceptions
Les exceptions sont utilisées pour gérer les erreurs qui peuvent survenir dans un programme.
Elles permettent de rendre le code plus robuste et plus facile à déboguer.
Opérateurs en Java
Opérateurs arithmétiques
Les opérateurs arithmétiques sont utilisés pour effectuer des opérations mathématiques sur des valeurs.
Voici quelques exemples d'opérateurs arithmétiques :
+ - Addition
- - Soustraction
* - Multiplication
/ - Division
% - Modulo
Opérateurs logiques
Les opérateurs logiques sont utilisés pour combiner des expressions booléennes.
Voici quelques exemples d'opérateurs logiques :
&& - Et
|| - Ou
! - Non
Opérateurs de comparaison
Les opérateurs de comparaison sont utilisés pour comparer des valeurs.
Voici quelques exemples d'opérateurs de comparaison :
== - Egalité
!= - Inégalité
< - Inférieur
> - Supérieur
<= - Inférieur ou égal
>= - Supérieur ou égal
Opérateurs de flux
Les opérateurs de flux sont utilisés pour traiter des collections de données.
Voici quelques exemples d'opérateurs de flux :
forEach() - Parcours d'une collection
filter() - Filtrage d'une collection
map() - Transformation d'une collection
reduce() - Réduction d'une collection
Opérateurs de chaîne de caractères
Les opérateurs de chaîne de caractères sont utilisés pour manipuler des chaînes de caractères.
Voici quelques exemples d'opérateurs de chaîne de caractères :
+ - Concaténation
.length() - Obtention de la longueur d'une chaîne de caractères
.charAt() - Obtention d'un caractère d'une chaîne de caractères
.indexOf() - Recherche d'un caractère ou d'une chaîne de caractères dans une chaîne de caractères
.substring() - Extraction d'une partie d'une chaîne de caractères

Jour 2
Collections en Java
Collections immuables
Les collections immuables sont des collections qui ne peuvent pas être modifiées après avoir été créées.
Elles sont utiles pour garantir l'intégrité des données.
Collections réactives
Les collections réactives sont des collections qui sont mises à jour de manière synchrone avec les modifications des données.
Elles sont utiles pour créer des applications web et mobiles réactives.
Entrée/sortie (E/S) en Java
Lecture et écriture de fichiers texte
Java fournit des classes et des méthodes pour lire et écrire des fichiers texte.
Lecture et écriture de fichiers binaires
Java fournit également des classes et des méthodes pour lire et écrire des fichiers binaires.
Collections immuables

Les collections immuables sont des collections qui ne peuvent pas être modifiées après avoir été créées.

Elles sont utiles pour garantir l'intégrité des données, car elles empêchent les modifications accidentelles ou malveillantes.

Voici quelques exemples de collections immuables en Java :

String
BigInteger
BigDecimal
List avec Collections.unmodifiableList()
Set avec Collections.unmodifiableSet()
Map avec Collections.unmodifiableMap()
Collections réactives

Les collections réactives sont des collections qui sont mises à jour de manière synchrone avec les modifications des données.

Elles sont utiles pour créer des applications web et mobiles réactives, qui doivent réagir rapidement aux changements de données.

Voici quelques exemples de collections réactives en Java :

List avec Stream()
Set avec Stream()
Map avec Stream()
Lecture et écriture de fichiers texte

Java fournit des classes et des méthodes pour lire et écrire des fichiers texte.

La classe File représente un fichier sur le système de fichiers.

La classe Scanner est utilisée pour lire les données d'un fichier texte.

La classe PrintWriter est utilisée pour écrire les données dans un fichier texte.

Exemple de lecture d'un fichier texte

Java
File file = new File("my-file.txt");

Scanner scanner = new Scanner(file);

while (scanner.hasNextLine()) {
    System.out.println(scanner.nextLine());
}
Utilisez le code avec précaution. En savoir plus
Exemple d'écriture d'un fichier texte

Java
File file = new File("my-file.txt");

PrintWriter writer = new PrintWriter(file);

writer.println("Hello, world!");

writer.close();
Utilisez le code avec précaution. En savoir plus
Lecture et écriture de fichiers binaires

Java fournit également des classes et des méthodes pour lire et écrire des fichiers binaires.

La classe FileInputStream est utilisée pour lire les données d'un fichier binaire.

La classe FileOutputStream est utilisée pour écrire les données dans un fichier binaire.

Exemple de lecture d'un fichier binaire

Java
File file = new File("my-file.bin");

FileInputStream inputStream = new FileInputStream(file);

byte[] bytes = new byte[(int) file.length()];

inputStream.read(bytes);

inputStream.close();

// Do something with the bytes
Utilisez le code avec précaution. En savoir plus
Exemple d'écriture d'un fichier binaire

Java
File file = new File("my-file.bin");

FileOutputStream outputStream = new FileOutputStream(file);

byte[] bytes = "Hello, world!".getBytes();

outputStream.write(bytes);

outputStream.close();
Utilisez le code avec précaution. En savoir plus
Sources
github.com/MYvLiang/FormTools

Tests unitaires en Java
Définition des tests unitaires
Les tests unitaires sont des programmes qui testent les fonctionnalités d'une unité de code.
Ils permettent de garantir que le code fonctionne correctement.
Écrire des tests unitaires
Il existe de nombreuses façons d'écrire des tests unitaires en Java.
Une méthode courante consiste à utiliser la bibliothèque JUnit.
Exécuter des tests unitaires
Les tests unitaires peuvent être exécutés manuellement ou automatiquement.
Il existe de nombreux outils disponibles pour exécuter des tests unitaires en Java.
Définition des tests unitaires

Les tests unitaires sont des programmes qui testent les fonctionnalités d'une unité de code.

Une unité de code est un bloc de code qui est responsable d'une fonctionnalité unique.

Les tests unitaires sont importants car ils permettent de garantir que le code fonctionne correctement.

Écrire des tests unitaires

Il existe de nombreuses façons d'écrire des tests unitaires en Java.

Une méthode courante consiste à utiliser la bibliothèque JUnit.

JUnit est une bibliothèque de tests unitaires open source pour Java.

Pour écrire des tests unitaires avec JUnit, vous devez créer une classe de test qui hérite de la classe JUnit4.

Voici un exemple de classe de test JUnit :

Java
public class MyTest extends JUnit4 {

    @Test
    public void testMyMethod() {
        // Écrire le code de test ici
    }
}
Utilisez le code avec précaution. En savoir plus
L'annotation @Test indique à JUnit que la méthode testMyMethod() est un test.

Exécuter des tests unitaires

Les tests unitaires peuvent être exécutés manuellement ou automatiquement.

Pour exécuter des tests unitaires manuellement, vous pouvez utiliser la commande mvn test.

Pour exécuter des tests unitaires automatiquement, vous pouvez utiliser un outil de test unitaire tel que Maven Surefire ou Gradle Test.

Exemple de test unitaire

Voici un exemple de test unitaire pour une méthode qui calcule le volume d'un cylindre :

Java
public class CylinderTest extends JUnit4 {

    @Test
    public void testCalculateVolume() {
        // Créer un objet Cylinder
        Cylinder cylinder = new Cylinder(10, 5);

        // Calculer le volume
        double volume = cylinder.calculateVolume();

        // Vérifier le résultat
        assertEquals(785.3981633974483, volume);
    }
}
Utilisez le code avec précaution. En savoir plus
Ce test vérifie que la méthode calculateVolume() renvoie la valeur correcte pour un cylindre de rayon 10 et de hauteur 5.

Slides du Jour 2

Diapositive 1

Titre : Tests unitaires en Java
Sous-titre : Définition, écriture et exécution
Diapositive 2

Définition des tests unitaires
Importance des tests unitaires
Diapositive 3

Méthodes courantes pour écrire des tests unitaires
Bibliothèque JUnit
Diapositive 4

Écrire un test unitaire avec JUnit
Annotation @Test
Diapositive 5

Exécuter des tests unitaires
Manuellement
Automatiquement
Diapositive 6

Exemple de test unitaire
Vérification du résultat d'une méthode
Diapositive 7

Exercice
Écrire un test unitaire pour une méthode qui calcule la somme de deux nombres
Diapositive 8

Conclusion
Importance des tests unitaires
Méthodes pour écrire des tests unitaires
Exécution des tests unitaires
Diapositive 9

Remarques
Les tests unitaires sont une partie essentielle du développement logiciel
Ils permettent de garantir la qualité du code
Il existe de nombreuses ressources disponibles pour apprendre à écrire des tests unitaires

Jour 3
Développement d'une application Web simple
Création de contrôleurs
Les contrôleurs sont responsables du traitement des requêtes HTTP et de la génération des réponses.
Utilisation de Thymeleaf pour les vues
Thymeleaf est un moteur de template HTML qui permet de créer des vues dynamiques.
Gestion des données avec Spring Boot
Spring Boot fournit des fonctionnalités pour gérer les données, telles que Spring Data JPA.
Intégration d'une base de données (par exemple, MySQL, H2)
Spring Boot fournit des fonctionnalités pour intégrer des bases de données, telles que Spring Data JPA.
Création de contrôleurs

Les contrôleurs sont responsables du traitement des requêtes HTTP et de la génération des réponses.

Ils sont définis dans des classes qui héritent de la classe @Controller.

Les contrôleurs utilisent des méthodes annotées avec @RequestMapping pour mapper les requêtes HTTP aux actions.

Utilisation de Thymeleaf pour les vues

Thymeleaf est un moteur de template HTML qui permet de créer des vues dynamiques.

Les vues Thymeleaf sont définies dans des fichiers HTML qui utilisent des expressions Thymeleaf pour accéder aux données du modèle.

Gestion des données avec Spring Boot

Spring Boot fournit des fonctionnalités pour gérer les données, telles que Spring Data JPA.

Spring Data JPA est une API pour accéder aux données dans les bases de données relationnelles.

Intégration d'une base de données (par exemple, MySQL, H2)

Spring Boot fournit des fonctionnalités pour intégrer des bases de données, telles que Spring Data JPA.

Pour intégrer une base de données MySQL, vous pouvez utiliser la dépendance mysql-connector-java.

Pour intégrer une base de données H2, vous pouvez utiliser la dépendance h2.

Slides du Jour 3

Diapositive 1

Titre : Développement d'une application Web simple
Sous-titre : Contrôleurs, vues, données
Diapositive 2

Contrôleurs
Responsables du traitement des requêtes HTTP et de la génération des réponses
Vues
Utilisées pour afficher les données à l'utilisateur
Données
Stockées dans une base de données
Diapositive 3

Contrôleurs en Java
Définition
Mapping des requêtes HTTP aux actions
Diapositive 4

Thymeleaf
Moteur de template HTML
Expressions Thymeleaf
Diapositive 5

Spring Data JPA
API pour accéder aux données dans les bases de données relationnelles
Diapositive 6

Intégration d'une base de données
MySQL
H2
Diapositive 7

Exemple d'application Web simple
Contrôleur
Vue
Base de données
Diapositive 8

Conclusion
Développement d'une application Web simple
Contrôleurs
Vues
Données
Diapositive 9

Exercice
Créer une application Web simple qui affiche une liste de produits
Diapositive 10

Remarques
Les applications Web peuvent être complexes
Il existe de nombreuses autres technologies et frameworks qui peuvent être utilisés pour développer des applications We










Diapositive 11

Titre : Développement d'une application Web simple
Sous-titre : Exemple d'application Web simple
Diapositive 12

Contrôleur
Classe ProductController
Méthode index()
Java
@Controller
public class ProductController {

    @GetMapping("/")
    public String index(Model model) {
        // Récupère la liste des produits
        List<Product> products = productService.findAll();

        // Ajoute la liste des produits au modèle
        model.addAttribute("products", products);

        return "index";
    }
}
Utilisez le code avec précaution. En savoir plus
Diapositive 13

Vue
Fichier index.html
Utilise des expressions Thymeleaf pour afficher la liste des produits
HTML
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml"
      xmlns:th="http://www.thymeleaf.org">
<head>
    <title>Liste des produits</title>
</head>
<body>
    <h1>Liste des produits</h1>
    <ul>
        <li th:each="product : ${products}">
            <a th:href="@{/product/{id}(id=${product.id})}">
                {{ product.name }}
            </a>
        </li>
    </ul>
</body>
</html>
Utilisez le code avec précaution. En savoir plus
Diapositive 14

Base de données
Table products
Colonnes id, name, price
SQL
CREATE TABLE products (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    price DECIMAL(10, 2)
);

Gestion des données avec Spring Boot
Spring Boot fournit des fonctionnalités pour gérer les données, telles que Spring Data JPA.

Spring Data JPA est une API pour accéder aux données dans les bases de données relationnelles.


Spring Data JPA
Spring Data JPA fournit une abstraction sur les bases de données relationnelles.

Cela permet aux développeurs de se concentrer sur l'écriture de code métier sans avoir à se soucier des détails de la base de données.

Spring Data JPA fournit des fonctionnalités pour les opérations CRUD (Create, Read, Update, Delete) sur les données.

Intégration d'une base de données
Pour intégrer une base de données avec Spring Boot, vous devez ajouter la dépendance appropriée à votre projet Maven ou Gradle.

Pour intégrer une base de données MySQL, vous pouvez utiliser la dépendance mysql-connector-java.

Pour intégrer une base de données H2, vous pouvez utiliser la dépendance h2.

Exemple
Voici un exemple d'utilisation de Spring Data JPA pour accéder à une base de données MySQL :

Java
@Entity
public class Product {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Integer id;

    private String name;

    private Double price;

    public Product() {
    }

    public Product(String name, Double price) {
        this.name = name;
        this.price = price;
    }

    public Integer getId() {
        return id;
    }

    public void setId(Integer id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public Double getPrice() {
        return price;
    }

    public void setPrice(Double price) {
        this.price = price;
    }
}

@Repository
public interface ProductRepository extends JpaRepository<Product, Integer> {
}

@RestController
public class ProductController {

    @Autowired
    private ProductRepository productRepository;

    @GetMapping("/products")
    public List<Product> getAllProducts() {
        return productRepository.findAll();
    }

    @PostMapping("/products")
    public Product createProduct(@RequestBody Product product) {
        return productRepository.save(product);
    }
}
Utilisez le code avec précaution. En savoir plus
Ce code définit une entité Product pour représenter un produit.

Il définit également une interface ProductRepository qui étend l'interface JpaRepository.

L'interface JpaRepository fournit des méthodes pour accéder aux données de la base de données.

Le contrôleur ProductController utilise l'interface ProductRepository pour accéder aux données de la base de données.

La méthode getAllProducts() renvoie la liste de tous les produits.

La méthode createProduct() crée un nouveau produit et l'enregistre dans la base de données.

Pour tester ce code, vous pouvez exécuter la commande suivante :

curl -X POST -H "Content-Type: application/json" -d '{"name": "T-shirt", "price": 10.00}' http://localhost:8080/products

Cette commande créera un nouveau produit avec le nom "T-shirt" et le prix 10,00 €.

Pour afficher la liste de tous les produits, vous pouvez exécuter la commande suivante :

curl http://localhost:8080/products
Cette commande renverra la réponse suivante :

[
    {
        "id": 1,
        "name": "T-shirt",
        "price": 10.00
    }
]
Liens utiles
Spring Data JPA: https://spring.io/projects/spring-data-jpa
MySQL: https://www.mysql.com/
H2: https://www.h2database.com/
Sources
github.com/mohammedatef555/jpa-hibernate-fundmentals
github.com/GabrielTonhatti/curso-angular
dzone.com/articles/integration-spring-mvc-and
github.com/yugabyte/orm-examplessoumis à licence (Apache - 2.0)
github.com/shangan23/ecommerce-apisoumis à licence (Apache - 2.0)

Diapositive 15

Exercice
Créer une application Web simple qui affiche une liste de produits
Diapositive 16

Remarques
Les applications Web peuvent être complexes
Il existe de nombreuses autres technologies et frameworks qui peuvent être utilisés pour développer des applications Web
Conclusion

Ce plan de formation a couvert les bases du développement d'applications Web en Java.

Les sujets suivants ont été abordés :

Installation de l'environnement de développement Java
Introduction à Java
Les bases de la programmation orientée objet
Tests unitaires en Java
Collections en Java
Entrée/sortie (E/S) en Java
Développement d'une application Web simple
Ce plan de formation est un point de départ pour apprendre à développer des applications Web en Java.

Pour en savoir plus, il existe de nombreuses ressources disponibles, telles que des livres, des articles et des cours en ligne.
