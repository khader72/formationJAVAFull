##  Les concepts de la POO en Java avec des exemples codes, des commentaires et des explications, ainsi que la sortie console :

### Concept 1 : Classe

Une classe est un modèle qui définit les propriétés et les comportements d'un objet.


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
```

**Commentaires et explications**

La classe Employe définit trois propriétés : nom, age et salaire.
Le constructeur Employe() permet d'initialiser les propriétés de l'objet.
La méthode afficherSalaire() affiche le salaire de l'employé.

**Sortie console**

Nom : John Doe
Âge : 30
Salaire : 3750000

### Concept 2 : Objet

Un objet est une instance d'une classe.

Exemple de code

Java
public class Main {

    public static void main(String[] args) {

        // Création d'un objet
        Employe employe = new Employe("John Doe", 30, 3750000);

        // Affichage du salaire
        employe.afficherSalaire();

    }

}
Utilisez le code avec précaution. En savoir plus
Commentaires et explications

La ligne Employe employe = new Employe("John Doe", 30, 3750000); crée un objet Employe avec les propriétés nom = "John Doe", age = 30 et salaire = 3750000.
La ligne employe.afficherSalaire(); appelle la méthode afficherSalaire() sur l'objet employe.
Sortie console

Le salaire de l'employé est de 3750000

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
        super.afficherSalaire();
        System.out.println("Le bonus du manager est de " + bonus);
    }

}
```

**Commentaires et explications**

La classe Manager hérite de la classe Employe.
La classe Manager ajoute une propriété bonus.
Le constructeur de la classe Manager appelle le constructeur de la classe Employe pour initialiser les propriétés nom, age et salaire.
La méthode afficherSalaire() de la classe Manager appelle la méthode afficherSalaire() de la classe `Employe
