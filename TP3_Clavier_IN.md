## System.console() : Lecture Simple des Chaînes de Caractères

Java fournit la méthode `System.console().readLine()` pour lire des chaînes de caractères à partir de la console. C'est une méthode simple et directe pour capturer des entrées clavier, en particulier pour les applications en ligne de commande.

```java
String nom = System.console().readLine("Entrez votre nom : ");

## 1. Lecture d'une chaîne de caractères

```java
String chaîne = System.console().readLine();
```


## 2. Lecture d'un entier

```java
int entier = Integer.parseInt(System.console().readLine());
```

## 3. Lecture d'un réel
```java
double réel = Double.parseDouble(System.console().readLine());
```


## 4. Lecture d'une chaîne de caractères avec une limite de caractères
```java
String chaîne = System.console().readLine("Entrez votre nom : ");
```



##  Exemples supplémentaires

System.console
Lecture d'une chaîne de caractères avec un message d'invite :

```java
String chaîne = System.console().readLine("Entrez votre nom : ");
```

Lecture d'une chaîne de caractères avec validation :
```java
String chaîne;
do {
  chaîne = System.console().readLine("Entrez votre nom : ");
} while (chaîne.length() < 3);
```

Lecture d'une chaîne de caractères à partir d'un fichier :

```java
Scanner scanner = new Scanner(new File("fichier.txt"));
String chaîne = scanner.nextLine();
```java

Lecture d'un entier à partir d'un flux réseau :

```java
Scanner scanner = new Scanner(new InputStream());
int entier = scanner.nextInt();
```

## Exercice

Écrire un programme qui demande à l'utilisateur son nom et son âge. Le programme doit ensuite afficher un message d'accueil avec le nom et l'âge de l'utilisateur.

```java
import java.util.Scanner;

public class Exercice {

  public static void main(String[] args) {
    // Créer un scanner pour lire l'entrée clavier
    Scanner scanner = new Scanner(System.in);

    // Demander le nom de l'utilisateur
    System.out.println("Entrez votre nom : ");
    String nom = scanner.nextLine();

    // Demander l'âge de l'utilisateur
    System.out.println("Entrez votre âge : ");
    int âge = scanner.nextInt();

    // Afficher un message d'accueil
    System.out.println("Bonjour " + nom + ", vous avez " + âge + " ans.");
  }
}
```

## System.console  VS Scanner

  **Avantages et inconvénients de System.console**
  
**Avantages**

Simple à utiliser
S'intègre bien à l'environnement d'exécution Java

**Inconvénients**

Nécessite que l'environnement d'exécution Java dispose d'une console
Ne fonctionne pas sur tous les systèmes d'exploitation

**Avantages et inconvénients de Scanner**

**Avantages**

Polyvalent
Fonctionne sur tous les systèmes d'exploitation

**Inconvénients**

Plus complexe à utiliser que System.console
Nécessite de convertir les données en types Java

**Conclusion**

System.console est un moyen simple et rapide d'obtenir une entrée clavier. Scanner est un moyen plus polyvalent, mais il nécessite plus de travail pour convertir les données en types Java.

| Critère          | `Scanner`                                                         | `System.console()`                                 |
| -----------------| ------------------------------------------------------------------ | -------------------------------------------------- |
| **Avantages**    | Polyvalent, peut lire différents types de données (chaînes, entiers, etc.). | Simple à utiliser pour lire des chaînes de caractères. |
| **Inconvénients**| Plus complexe à utiliser pour les débutants. Nécessite de convertir les données en types Java appropriés. | Nécessite que l'environnement d'exécution Java dispose d'une console. Ne fonctionne pas sur tous les systèmes d'exploitation. |
| **Exemple**      | Lecture d'une chaîne de caractères :<br>`Scanner scanner = new Scanner(System.in);`<br>`String chaîne = scanner.nextLine();` | Lecture d'une chaîne de caractères :<br>`String chaîne = System.console().readLine();` |

**Commentaire :**

- **Scanner** est un outil polyvalent pour la lecture des entrées utilisateur. Il peut gérer différents types de données et offre une grande flexibilité. Cependant, il peut être plus complexe à utiliser, surtout pour les débutants, car il nécessite de convertir les données lues en types Java appropriés.

- **System.console()**, d'autre part, est simple à utiliser pour lire des chaînes de caractères. Il peut être préféré pour des cas simples où seule la lecture de chaînes est nécessaire. Cependant, il est important de noter qu'il a ses limitations, notamment le fait qu'il ne fonctionne pas sur tous les systèmes d'exploitation et qu'il ne peut pas lire d'autres types de données que des chaînes.

Ces différences font en sorte que le choix entre `Scanner` et `System.console()` dépend des besoins spécifiques de votre programme et du niveau de complexité que vous souhaitez atteindre.

