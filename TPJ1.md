
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
## TP 3 : Boucles et affichage de nombres


```Java
import java.util.Scanner;

public class TP3 {

    public static void main(String[] args) {

        /*
        Ce programme affiche les nombres de 0 à 9 en utilisant une boucle `for`.

        La boucle `for` s'exécutera 10 fois, une fois pour chaque nombre de 0 à 9.

        La valeur de la variable `i` sera incrémentée de 1 à chaque itération de la boucle.

        La valeur de la variable `i` est affichée à l'écran à chaque itération de la boucle.
        */

        // Déclaration de la variable `i`
        int i;

        // Boucle `for`
        for (i = 0; i <= 9; i++) {
            System.out.println(i);
        }

    }
}
```


**Sortie console**
```
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
```

**Explications**

La variable i est déclarée de type int et affectée à la valeur 0.
La boucle for s'exécutera 10 fois, une fois pour chaque nombre de 0 à 9.
La valeur de la variable i est incrémentée de 1 à chaque itération de la boucle.
La valeur de la variable i est affichée à l'écran à chaque itération de la boucle.

## TP 4 : Saisie d'un nombre et affichage de son carré



```Java
import java.util.Scanner;

public class TP4 {

    public static void main(String[] args) {

        /*
        Ce programme demande à l'utilisateur de saisir un nombre et affiche son carré.

        Un objet `Scanner` est créé pour lire l'entrée utilisateur.

        La méthode `nextInt()` est utilisée pour lire un entier de l'entrée utilisateur.

        La valeur saisie par l'utilisateur est affectée à la variable `nombre`.

        La valeur saisie par l'utilisateur est multipliée par elle-même pour calculer son carré.

        Le carré du nombre saisi est affiché à l'écran.

        L'objet `Scanner` est fermé pour libérer les ressources utilisées.
        */

        // Déclaration des variables
        int nombre;

        // Création d'un objet Scanner
        Scanner scanner = new Scanner(System.in);

        // Saisie de l'entrée utilisateur
        System.out.println("Entrez un nombre : ");
        nombre = scanner.nextInt();

        // Calcul du carré
        int carre = nombre * nombre;

        // Affichage du résultat
        System.out.println("Le carré du nombre est de " + carre);

        // Fermeture de l'objet Scanner
        scanner.close();

    }
}
```

**Sortie console**

```
Entrez un nombre : 5
Le carré du nombre est de 25
```

**Explications**

Un objet Scanner est créé pour lire l'entrée utilisateur.
La méthode nextInt() est utilisée pour lire un entier de l'entrée utilisateur.
La valeur saisie par l'utilisateur est affectée à la variable nombre.
La valeur saisie par l'utilisateur est multipliée par elle-même pour calculer son carré.
Le carré du nombre saisi est affiché à l'écran.
L'objet Scanner est fermé pour libérer les ressources utilisées.

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

## TP 5 : Saisie d'un nom et affichage d'un message de bienvenue



```Java
import java.util.Scanner;

public class TP5 {

    public static void main(String[] args) {

        /*
        Ce programme demande à l'utilisateur de saisir son nom et affiche un message de bienvenue.

        Un objet `Scanner` est créé pour lire l'entrée utilisateur.

        La méthode `nextLine()` est utilisée pour lire une chaîne de caractères de l'entrée utilisateur.

        La valeur saisie par l'utilisateur est affectée à la variable `nom`.

        Un message de bienvenue est affiché à l'écran avec le nom saisi par l'utilisateur.

        L'objet `Scanner` est fermé pour libérer les ressources utilisées.
        */

        // Déclaration des variables
        String nom;

        // Création d'un objet Scanner
        Scanner scanner = new Scanner(System.in);

        // Saisie de l'entrée utilisateur
        System.out.println("Entrez votre nom : ");
        nom = scanner.nextLine();

        // Affichage du message de bienvenue
        System.out.println("Bienvenue, " + nom + " !");

        // Fermeture de l'objet Scanner
        scanner.close();

    }
}
```

**Sortie console**

```
Entrez votre nom : John Doe
Bienvenue, John Doe !
```

**Explications**
```
Un objet Scanner est créé pour lire l'entrée utilisateur.
La méthode nextLine() est utilisée pour lire une chaîne de caractères de l'entrée utilisateur.
La valeur saisie par l'utilisateur est affectée à la variable nom.
Un message de bienvenue est affiché à l'écran avec le nom saisi par l'utilisateur.
L'objet Scanner est fermé pour libérer les ressources utilisées.
```

## TP 6 : Saisie d'une note et affichage d'une mention

```Java
import java.util.Scanner;

public class TP6 {

    public static void main(String[] args) {

        /*
        Ce programme demande à l'utilisateur de saisir une note et affiche la mention correspondante.

        Un objet `Scanner` est créé pour lire l'entrée utilisateur.

        La méthode `nextFloat()` est utilisée pour lire un nombre réel de l'entrée utilisateur.

        La valeur saisie par l'utilisateur est affectée à la variable `note`.

        La mention est calculée en fonction de la valeur de la variable `note`.

        La mention est affichée à l'écran.

        L'objet `Scanner` est fermé pour libérer les ressources utilisées.
        */

        // Déclaration des variables
        float note;
        String mention;

        // Création d'un objet Scanner
        Scanner scanner = new Scanner(System.in);

        // Saisie de l'entrée utilisateur
        System.out.println("Entrez une note : ");
        note = scanner.nextFloat();

        // Calcul de la mention
        if (note >= 12) {
            mention = "Très bien";
        } else if (note >= 10) {
            mention = "Bien";
        } else if (note >= 8) {
            mention = "Assez bien";
        } else if (note >= 6) {
            mention = "Passable";
        } else {
            mention = "Insuffisant";
        }

        // Affichage de la mention
        System.out.println("La mention est de " + mention);

        // Fermeture de l'objet Scanner
        scanner.close();

    }
}
```

**Sortie console**

```
Entrez une note : 10
La mention est de Bien
```

** Explications **

```
Un objet Scanner est créé pour lire l'entrée utilisateur.
La méthode nextFloat() est utilisée pour lire un nombre réel de l'entrée utilisateur.
La valeur saisie par l'utilisateur est affectée à la variable note.
La mention est calculée en fonction de la valeur de la variable note.
La mention est affichée à l'écran.
L'objet Scanner est fermé pour libérer les ressources utilisées.
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

## Un TP de synthèse avec 4 méthodes + la méthode main pour résumer les concepts sur les méthodes en Java avec Scanner pour les entrées claviers :

TP de synthèse

Objectifs

Récapituler les concepts sur les méthodes en Java
Utiliser Scanner pour les entrées claviers
Méthodes

saisirNom() : demande à l'utilisateur de saisir son nom et renvoie la chaîne de caractères saisie.
saisirAge() : demande à l'utilisateur de saisir son âge et renvoie l'entier saisi.
calculerSalaire() : calcule le salaire annuel d'un employé en fonction de son âge.
afficherResultats() : affiche les résultats du calcul du salaire.
Méthode main

```
Java
public class TPSynthese {

    public static void main(String[] args) {

        // Déclaration des variables
        String nom;
        int age;
        float salaire;

        // Saisie du nom et de l'âge
        nom = saisirNom();
        age = saisirAge();

        // Calcul du salaire
        salaire = calculerSalaire(age);

        // Affichage des résultats
        afficherResultats(nom, age, salaire);

    }

    // Méthode pour saisir le nom
    public static String saisirNom() {

        // Déclaration de la variable
        String nom;

        // Création d'un objet Scanner
        Scanner scanner = new Scanner(System.in);

        // Saisie de l'entrée utilisateur
        System.out.println("Entrez votre nom : ");
        nom = scanner.nextLine();

        // Fermeture de l'objet Scanner
        scanner.close();

        // Retour de la valeur saisie
        return nom;

    }

    // Méthode pour saisir l'âge
    public static int saisirAge() {

        // Déclaration de la variable
        int age;

        // Création d'un objet Scanner
        Scanner scanner = new Scanner(System.in);

        // Saisie de l'entrée utilisateur
        System.out.println("Entrez votre âge : ");
        age = scanner.nextInt();

        // Fermeture de l'objet Scanner
        scanner.close();

        // Retour de la valeur saisie
        return age;

    }

    // Méthode pour calculer le salaire
    public static float calculerSalaire(int age) {

        // Déclaration de la variable
        float salaire;

        // Calcul du salaire
        salaire = 100000 * (age + 25);

        // Retour de la valeur calculée
        return salaire;

    }

    // Méthode pour afficher les résultats
    public static void afficherResultats(String nom, int age, float salaire) {

        // Affichage du nom
        System.out.println("Nom : " + nom);

        // Affichage de l'âge
        System.out.println("Âge : " + age);

        // Affichage du salaire
        System.out.println("Salaire : " + salaire);

    }

}
```


**Sortie console**

```
Entrez votre nom : John Doe
Entrez votre âge : 30
Nom : John Doe
Âge : 30
Salaire : 3750000
```

**Explications**
La méthode saisirNom() utilise Scanner pour lire une chaîne de caractères de l'entrée utilisateur.
La méthode saisirAge() utilise Scanner pour lire un entier de l'entrée utilisateur.
La méthode calculerSalaire() calcule le salaire annuel d'un employé en fonction de son âge.
La méthode afficherResultats() affiche les résultats du calcul du salaire.
Ce TP permet de mettre en pratique les concepts suivants :

Déclaration de méthodes
Appel de méthodes
Paramètres de méthodes
Retour de méthodes
Utilisation de Scanner pour les entrées claviers
Ce TP peut être adapté en fonction des besoins. Par exemple, on peut ajouter des méthodes supplémentaires pour calculer d'autres informations, telles que le montant des impôts ou la durée des vacances.



La méthode saisirNom() utilise Scanner pour lire une chaîne de caractères de l'entrée utilisateur.
La méthode saisirAge() utilise Scanner pour lire un entier de l'entrée utilisateur.
La méthode calculerSalaire() calcule le salaire annuel d'un employé en fonction de son âge.
La méthode afficherResultats() affiche les résultats du calcul du salaire.
Ce TP permet de mettre en pratique les concepts suivants :

Déclaration de méthodes
Appel de méthodes
Paramètres de méthodes
Retour de méthodes
Utilisation de Scanner pour les entrées claviers
Ce TP peut être adapté en fonction des besoins. Par exemple, on peut ajouter des méthodes supplémentaires pour calculer d'autres informations, telles que le montant des impôts ou la durée des vacances.
