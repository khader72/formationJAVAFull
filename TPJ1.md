
## TP 1 : Déclaration et affectation de variables



```java

public class TP1 {

    public static void main(String[] args) {

        /*
        Ce programme déclare et affecte des variables de différents types de données.

        La variable `age` est déclarée de type `int` et affectée à la valeur 25.

        La variable `nom` est déclarée de type `String` et affectée à la valeur "John Doe".

        La variable `salaire` est déclarée de type `double` et affectée à la valeur 100000.0.

        Les valeurs des variables sont affichées à l'écran.
        */

        // Déclaration des variables
        int age = 25;
        String nom = "John Doe";
        double salaire = 100000.0;

        // Affichage des variables
        System.out.println("L'âge de l'utilisateur est de " + age);
        System.out.println("Le nom de l'utilisateur est " + nom);
        System.out.println("Le salaire de l'utilisateur est de " + salaire);

    }
}
```

**Sortie console**

```
L'âge de l'utilisateur est de 25
Le nom de l'utilisateur est John Doe
Le salaire de l'utilisateur est de 100000.0
```

**Explications**

```
La variable age est déclarée de type int et affectée à la valeur 25.
La variable nom est déclarée de type String et affectée à la valeur "John Doe".
La variable salaire est déclarée de type double et affectée à la valeur 100000.0.
Les valeurs des variables sont affichées à l'écran.
```

## TP 2 : Calculs et affichage de résultats


```Java


public class TP2 {

    public static void main(String[] args) {

        /*
        Ce programme calcule et affiche les valeurs suivantes :

        * L'âge de l'utilisateur dans 10 ans
        * Le salaire annuel de l'utilisateur
        * Le message "L'utilisateur est majeur" si l'utilisateur est âgé de 18 ans ou plus
        * Le message "L'utilisateur est mineur" si l'utilisateur est âgé de moins de 18 ans

        La variable `age` est déclarée de type `int` et affectée à la valeur 25.

        La variable `salaire` est déclarée de type `double` et affectée à la valeur 100000.0.

        Les calculs et les messages sont affichés à l'écran.
        */

        // Déclaration des variables
        int age = 25;
        double salaire = 100000.0;

        // Calculs
        int ageDansDixAns = age + 10;
        double salaireAnnuel = salaire * 12;

        // Affichage des résultats
        System.out.println("L'âge de l'utilisateur dans 10 ans sera de " + ageDansDixAns);
        System.out.println("Le salaire annuel de l'utilisateur est de " + salaireAnnuel);

        // Condition
        if (age >= 18) {
            System.out.println("L'utilisateur est majeur");
        } else {
            System.out.println("L'utilisateur est mineur");
        }

    }
}
```


**Sortie console**

```
L'âge de l'utilisateur dans 10 ans sera de 35
Le salaire annuel de l'utilisateur est de 1200000.0
L'utilisateur est majeur
```

**Explications**

```
La variable age est déclarée de type int et affectée à la valeur 25.
La variable salaire est déclarée de type double et affectée à la valeur 100000.0.
Les calculs sont effectués
```

## Synthèse 1  Code hors POO

```java
public class HelloWorld {

    public static void main(String[] args) {
        // Déclaration des variables
        int age = 25; // Variable d'âge
        String nom = "John Doe"; // Variable de nom
        double salaire = 100000.0; // Variable de salaire

        // Affichage des variables
        System.out.println("L'âge de l'utilisateur est de " + age);
        System.out.println("Le nom de l'utilisateur est " + nom);
        System.out.println("Le salaire de l'utilisateur est de " + salaire);

        // Calculs
        int ageDansDixAns = age + 10; // Calcul de l'âge de l'utilisateur dans 10 ans
        double salaireAnnuel = salaire * 12; // Calcul du salaire annuel de l'utilisateur

        // Affichage des résultats des calculs
        System.out.println("L'âge de l'utilisateur dans 10 ans sera de " + ageDansDixAns);
        System.out.println("Le salaire annuel de l'utilisateur est de " + salaireAnnuel);

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
        sayHello();
    }

    public static void sayHello() {
        System.out.println("Bonjour !");
    }
}

```


Voici un code complet en Java qui intègre tous les concepts du jour 1 :

Java
// Déclaration des variables
int age = 25; // Variable d'âge
String nom = "John Doe"; // Variable de nom
double salaire = 100000.0; // Variable de salaire

// Affichage des variables
System.out.println("L'âge de l'utilisateur est de " + age);
System.out.println("Le nom de l'utilisateur est " + nom);
System.out.println("Le salaire de l'utilisateur est de " + salaire);

// Calculs
int ageDansDixAns = age + 10; // Calcul de l'âge de l'utilisateur dans 10 ans
double salaireAnnuel = salaire * 12; // Calcul du salaire annuel de l'utilisateur

// Affichage des résultats des calculs
System.out.println("L'âge de l'utilisateur dans 10 ans sera de " + ageDansDixAns);
System.out.println("Le salaire annuel de l'utilisateur est de " + salaireAnnuel);

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
public static void sayHello() {
    System.out.println("Bonjour !");
}

// Appel de la fonction
sayHello();
Utilisez le code avec précaution. En savoir plus
Ce code comprend les éléments suivants :

Variables

Déclaration de variables d'âge, de nom et de salaire
Affichage des valeurs des variables
Types de données

Utilisation de types de données primitifs (int, String et double)
Opérations

Calcul de l'âge de l'utilisateur dans 10 ans
Calcul du salaire annuel de l'utilisateur
Conditions

Vérification de l'âge de l'utilisateur pour déterminer s'il est majeur ou mineur
Boucles

Affichage des nombres de 0 à 9
Fonctions

Définition d'une fonction sayHello() qui affiche un message
Appel de la fonction sayHello()
Commentaires

Chaque ligne de code est commentée pour expliquer sa fonction. Ces commentaires sont utiles pour comprendre le code et le réutiliser.


## Exemple de sortie

```
L'âge de l'utilisateur est de 25
Le nom de l'utilisateur est John Doe
Le salaire de l'utilisateur est de 100000.0
L'âge de l'utilisateur dans 10 ans sera de 35
Le salaire annuel de l'utilisateur est de 1200000.0
L'utilisateur est majeur
0
1
2
3
4
5
6
7
8
9
Bonjour !
```

Ce code est un bon point de départ pour apprendre les bases de la programmation Java. Il est important de pratiquer la programmation pour maîtriser ces concepts.
