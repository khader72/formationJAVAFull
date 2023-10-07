##  Les concepts de la POO en Java avec des exemples codes, des commentaires et des explications, ainsi que la sortie console :

### Concept 1 : Classe

Une classe est un modèle qui définit les propriétés et les comportements d'un objet.

Exemple de code

Java
public class Employe {

    // Propriétés
    private String nom;
    private int age;
    private float salaire;

    // Constructeur
    public Employe(String nom, int age, float salaire) {
        this.nom = nom;
        this.age = age;
        this.salaire = salaire;
    }

    // Méthodes
    public void afficherSalaire() {
        System.out.println("Le salaire de l'employé est de " + salaire);
    }

}


**Commentaires et explications**

La classe Employe définit trois propriétés : nom, age et salaire.
Le constructeur Employe() permet d'initialiser les propriétés de l'objet.
La méthode afficherSalaire() affiche le salaire de l'employé.

**Utilité du concept**

Le concept de classe permet de créer des objets avec des propriétés et des comportements similaires.
Cela permet de réduire la duplication de code et de faciliter la maintenance du code.
Les classes peuvent être réutilisées dans différents projets.

**Exemple d'utilisation**

La classe Employe peut être utilisée pour représenter un employé dans une entreprise.
Les propriétés nom, age et salaire peuvent être utilisées pour stocker les informations sur l'employé.
La méthode afficherSalaire() peut être utilisée pour afficher le salaire de l'employé.

### Concept 2 : Objet

Un objet est une instance d'une classe.

Exemple de code

```Java
public class Main {

    public static void main(String[] args) {

        // Création d'un objet
        Employe employe = new Employe("John Doe", 30, 3750000);

        // Affichage du salaire
        employe.afficherSalaire();

    }

}
```


**Commentaires et explications**

```
La ligne Employe employe = new Employe("John Doe", 30, 3750000); crée un objet Employe avec les propriétés nom = "John Doe", age = 30 et salaire = 3750000.
La ligne employe.afficherSalaire(); appelle la méthode afficherSalaire() sur l'objet employe.
```

**Utilité du concept**

Le concept d'objet permet de créer des instances uniques d'une classe.
Cela permet de représenter des objets du monde réel dans le code.
Les objets peuvent être utilisés pour stocker des données et exécuter des actions.

**Exemple d'utilisation**

L'objet employe créé dans l'exemple de code représente un employé spécifique.
Les propriétés nom, age et salaire stockent les informations sur l'employé.
La méthode afficherSalaire() permet d'afficher le salaire de l'employé.



### Concept 3 : Héritage

L'héritage est une relation entre deux classes où une classe, la classe fille, hérite des propriétés et des comportements de l'autre classe, la classe mère.

Exemple de code

```Java
public class Employe {

    // Propriétés
    private String nom;
    private int age;
    private float salaire;

    // Constructeur
    public Employe(String nom, int age, float salaire) {
        this.nom = nom;
        this.age = age;
        this.salaire = salaire;
    }

    // Méthodes
    public void afficherSalaire() {
        System.out.println("Le salaire de l'employé est de " + salaire);
    }

}

public class Manager extends Employe {

    // Propriétés
    private float bonus;

    // Constructeur
    public Manager(String nom, int age, float salaire, float bonus) {
        super(nom, age, salaire);
        this.bonus = bonus;
    }

    // Méthodes
    public void afficherSalaire() {
        // Affiche le salaire de l'employé
        super.afficherSalaire();

        // Affiche le bonus du manager
        System.out.println("Le bonus du manager est de " + bonus);
    }

}
```

**Commentaires et explications**

La classe Manager hérite de la classe Employe.
La classe Manager ajoute une propriété bonus.
Le constructeur de la classe Manager appelle le constructeur de la classe Employe pour initialiser les propriétés nom, age et salaire.
La méthode afficherSalaire() de la classe Manager appelle la méthode afficherSalaire() de la classe Employe.

**Utilité du concept**

Le concept d'héritage permet de réutiliser le code et de simplifier la conception des classes.
Cela permet de créer des classes plus complexes avec moins de code.

**Exemple d'utilisation**

La classe Manager peut être utilisée pour représenter un manager dans une entreprise.
La propriété bonus peut être utilisée pour stocker le bonus du manager.
La méthode afficherSalaire() peut être utilisée pour afficher le salaire et le bonus du manager.
