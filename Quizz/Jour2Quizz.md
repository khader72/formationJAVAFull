## Jour 2: Programmation Orientée Objet (POO) en Java

**Qu'est-ce que la programmation orientée objet (POO) ?**

A. Un langage de programmation
B. Un style de programmation basé sur les objets et les classes
C. Un système d'exploitation orienté vers les objets
D. Un type de café orienté vers les objets
E. Une méthode de programmation basée sur les algorithmes

**Qu'est-ce qu'un objet en programmation orientée objet?**

A. Une variable primitive
B. Une instance d'une classe
C. Une fonction mathématique
D. Un pointeur mémoire
E. Un opérateur logique

**Qu'est-ce qu'une classe en Java?**

A. Une méthode statique
B. Une bibliothèque standard
C. Un type de données primitif
D. Un modèle pour créer des objets
E. Une fonction mathématique avancée

**Qu'est-ce qu'un constructeur en Java?**

A. Une méthode utilisée pour détruire les objets
B. Une méthode utilisée pour initialiser les variables d'instance d'un objet
C. Une méthode statique
D. Une méthode utilisée pour déclarer des variables
E. Une méthode utilisée pour imprimer du texte à la console

**Comment appelez-vous le processus de regroupement de données et de méthodes dans un même conteneur?**

A. Encapsulation
B. Héritage
C. Polymorphisme
D. Abstraction
E. Modulation

**Qu'est-ce que l'héritage en programmation orientée objet?**

A. Un processus permettant à un objet de prendre les propriétés et les comportements d'une autre classe
B. Un processus permettant à un objet de se cacher dans une autre classe
C. Un processus permettant à un objet de réduire la visibilité de ses méthodes
D. Un processus permettant à un objet d'agréger d'autres objets
E. Un processus permettant à un objet de détruire d'autres objets

**Qu'est-ce que le polymorphisme en Java?**

A. Un processus permettant à un objet d'avoir plusieurs formes
B. Un processus permettant à un objet de prendre la forme d'un autre objet
C. Un processus permettant à un objet de réduire sa taille
D. Un processus permettant à un objet de changer sa couleur
E. Un processus permettant à un objet de se diviser en plusieurs objets

**Quelle est la différence entre l'interface et la classe abstraite en Java?**

A. Une interface peut avoir des méthodes implémentées, une classe abstraite ne peut pas.
B. Une interface peut avoir des variables d'instance, une classe abstraite ne peut pas.
C. Une classe abstraite peut être instanciée, une interface ne peut pas.
D. Une interface peut avoir des constructeurs, une classe abstraite ne peut pas.
E. Une classe abstraite peut implémenter plusieurs interfaces, une interface ne peut pas.

**Qu'est-ce que l'encapsulation en Java?**

A. Le processus de cacher les détails de l'implémentation d'une classe
B. Le processus de regrouper des variables et des méthodes dans une même classe
C. Le processus de rendre une classe accessible depuis n'importe où dans le programme
D. Le processus de rendre une classe immuable
E. Le processus de cacher les détails de la déclaration des variables

**Qu'est-ce qu'une exception en Java?**

A. Un objet représentant une situation d'erreur
B. Une méthode statique
C. Une variable primitive
D. Un opérateur de comparaison
E. Un type de données primitif

**Comment gérez-vous les exceptions en Java?**

A. En les ignorants complètement
B. En utilisant la déclaration throws dans la signature de méthode
C. En utilisant un bloc try-catch pour intercepter et traiter les exceptions
D. En modifiant le code source de la JVM
E. En utilisant la déclaration exception dans la signature de méthode

**Qu'est-ce qu'une méthode abstraite en Java?**

A. Une méthode qui a une implémentation dans la classe abstraite
B. Une méthode qui n'a pas de corps et doit être implémentée par les classes dérivées
C. Une méthode qui ne peut pas être appelée
D. Une méthode qui est statique
E. Une méthode qui ne peut pas être héritée

**Quelle est la principale utilisation de l'opérateur instanceof en Java?**

A. Pour vérifier si un objet est une instance d'une classe spécifique
B. Pour convertir un type de données en un autre type
C. Pour comparer deux objets
D. Pour vérifier si un objet est nul
E. Pour vérifier si un objet est immuable

**Comment appelez-vous le processus de création d'une nouvelle classe basée sur une classe existante?**

A. Héritage
B. Polymorphisme
C. Encapsulation
D. Abstraction
E. Instantiation

**Quelle est la sortie de ce code :**

```java

class A {
    void display() {
        System.out.println("A");
    }
}

class B extends A {
    void display() {
        System.out.println("B");
    }
}

public class Main {
    public static void main(String[] args) {
        A obj = new B();
        obj.display();
    }
}
```

A. A
B. B
C. Compilation Error
D. Runtime Error
E. A B

**Quelle est la sortie de ce code :**

```java

class MyClass {
    static void display() {
        System.out.println("Static method");
    }
    
    public static void main(String[] args) {
        MyClass obj = null;
        obj.display();
    }
}
```

A. Static method
B. Compilation Error
C. NullPointerException
D. Runtime Error
E. Aucune sortie

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int x = 5;
        System.out.println(x > 2 ? x < 4 ? 10 : 8 : 7);
    }
}
```

A. 10
B. 8
C. 7
D. Compilation Error
E. Runtime Error

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int i = 1;
        do {
            System.out.println(i);
            i++;
        } while (i <= 5);
    }
}
```

A. 1 2 3 4 5
B. 1 2 3 4
C. 2 3 4 5
D. 1
E. Compilation Error

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int num = 5;
        if (num > 0) {
            System.out.println("Positive");
        } else {
            System.out.println("Negative");
        }
    }
}
```
A. Positive
B. Negative
C. 5
D. Compilation Error
E. Aucune sortie

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int x = 10;
        if (x++ > 10) {
            System.out.println("True");
        } else {
            System.out.println("False");
        }
    }
}
```

A. True
B. False
C. Compilation Error
D. 10
E. Aucune sortie

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int x = 5;
        int y = 10;
        System.out.println(x + y * 2);
    }
}
```

A. 25
B. 30
C. 35
D. 20
E. 15

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            System.out.print(i + " ");
        }
    }
}
```

A. 0 1 2 3 4
B. 1 2 3 4 5
C. 0 1 2 3
D. 1 2 3 4
E. Compilation Error

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        String[] names = {"Alice", "Bob", "Charlie"};
        for (String name : names) {
            System.out.print(name + " ");
        }
    }
}
```

A. Alice Bob Charlie
B. 0 1 2
C. Compilation Error
D. Bob Alice Charlie
E. Aucune sortie

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int x = 5;
        while (x > 0) {
            System.out.print(x + " ");
            x--;
        }
    }
}
```

A. 5 4 3 2 1
B. 1 2 3 4 5
C. 0
D. Compilation Error
E. Aucune sortie

**Quelle est la sortie de ce code :**

```java

public class Main {
    public static void main(String[] args) {
        int x = 10;
        do {
            System.out.print(x + " ");
            x -= 2;
        } while (x > 0);
    }
}
```

A. 10 8 6 4 2
B. 10 6 2
C. 8 6 4 2
D. 10 9 8 7 6 5 4 3 2 1
E. Aucune sortie
