
# TP sur la gestion des exceptions en Java

## Objectifs

Comprendre les concepts de base de la gestion des exceptions en Java
Savoir identifier les situations susceptibles de générer des exceptions
Savoir gérer les exceptions de manière appropriée

### Exercice 1 : Identification des exceptions

```Java
// Génération d'une `ArithmeticException`
int a = 10;
int b = 0;

int c = a / b;

// Génération d'une `ArrayIndexOutOfBoundsException`
int[] tableau = new int[10];

System.out.println(tableau[11]);

// Génération d'une `NullPointerException`
String chaine = null;

System.out.println(chaine.length());

// Génération d'une `NumberFormatException`
String nombre = "123";

int entier = Integer.parseInt(nombre);

// Génération d'une `FileNotFoundException`
File fichier = new File("fichier.txt");

FileReader lecteur = new FileReader(fichier);
```

**Explications**

```
L'instruction int c = a / b; génère une ArithmeticException car la division par zéro est illégale.
L'instruction System.out.println(tableau[11]); génère une ArrayIndexOutOfBoundsException car l'index 11 est hors des limites du tableau.
L'instruction System.out.println(chaine.length()); génère une NullPointerException car la variable chaine est nulle.
L'instruction int entier = Integer.parseInt(nombre); génère une NumberFormatException car la chaîne nombre ne représente pas un nombre entier valide.
L'instruction FileReader lecteur = new FileReader(fichier); génère une FileNotFoundException car le fichier fichier.txt n'existe pas.
```

**Justifications**

La division par zéro est illégale en Java. Si une division par zéro est tentée, une ArithmeticException est générée.
L'index d'un tableau ne doit pas être supérieur à la longueur du tableau. Si un index hors limites est utilisé, une ArrayIndexOutOfBoundsException est générée.
Une variable null ne peut pas être utilisée pour accéder à une propriété.

### Exercice 2 : Gestion des exceptions

```Java
// Gestion d'une `ArithmeticException`
int a = 10;
int b = 0;

try {
    int c = a / b;
} catch (ArithmeticException e) {
    System.out.println("Division par zéro.");
}

// Gestion d'une `ArrayIndexOutOfBoundsException`
int[] tableau = new int[10];

try {
    System.out.println(tableau[11]);
} catch (ArrayIndexOutOfBoundsException e) {
    System.out.println("Index hors limites.");
}

// Gestion d'une `NullPointerException`
String chaine = null;

try {
    System.out.println(chaine.length());
} catch (NullPointerException e) {
    System.out.println("La chaîne est nulle.");
}

// Gestion d'une `NumberFormatException`
String nombre = "123";

try {
    int entier = Integer.parseInt(nombre);
} catch (NumberFormatException e) {
    System.out.println("Le nombre n'est pas valide.");
}

// Gestion d'une `FileNotFoundException`
File fichier = new File("fichier.txt");

try {
    FileReader lecteur = new FileReader(fichier);
} catch (FileNotFoundException e) {
    System.out.println("Le fichier n'existe pas.");
}
```

**Explications**

L'instruction try/catch permet de gérer les exceptions.
Le bloc try contient le code qui peut générer une exception.
Le bloc catch contient le code qui sera exécuté si une exception est générée.
La variable e dans le bloc catch contient l'objet exception qui a été généré.
Conclusion

La gestion des exceptions est une partie importante de la programmation en Java. Elle permet de garantir que le programme continue de s'exécuter même si une exception est générée
