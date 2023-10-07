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
