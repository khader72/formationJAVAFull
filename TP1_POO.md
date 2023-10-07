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


### Concept 4 : Polymorphisme

Le polymorphisme est la capacité d'une variable d'une classe mère à référencer un objet d'une classe fille.

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

public class Main {

    public static void main(String[] args) {

        // Création d'un objet Manager
        Manager manager = new Manager("John Doe", 30, 3750000, 50000);

        // Affichage du salaire
        afficherSalaire(manager);

    }

    public static void afficherSalaire(Employe employe) {
        employe.afficherSalaire();
    }

}


Commentaires et explications

La méthode afficherSalaire() de la classe Main accepte un paramètre de type Employe.
Dans la ligne afficherSalaire(manager);, le paramètre manager est un objet de type Manager.
La méthode afficherSalaire() appelle la méthode afficherSalaire() de la classe Manager.
Utilité du concept

Le polymorphisme permet de simplifier le code en permettant de traiter des objets de différentes classes de manière uniforme.
Cela permet d'écrire du code qui est plus générique et plus extensible.
Exemple d'utilisation

Dans l'exemple de code, la méthode afficherSalaire() peut être utilisée pour afficher le salaire de n'importe quel objet de type Employe, qu'il s'agisse d'un employé ou d'un manager.

### Concept 5 : Encapsulation

L'encapsulation est la pratique de cacher les détails d'une classe aux utilisateurs de la classe.

Exemple de code

Java
public class Employe {

    // Propriétés privées
    private String nom;
    private int age;
    private float salaire;

    // Constructeur
    public Employe(String nom, int age, float salaire) {
        this.nom = nom;
        this.age = age;
        this.salaire = salaire;
    }

    // Méthodes publiques pour accéder aux propriétés privées
    public String getNom() {
        return nom;
    }

    public void setNom(String nom) {
        this.nom = nom;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    public float getSalaire() {
        return salaire;
    }

    public void setSalaire(float salaire) {
        this.salaire = salaire;
    }

}
Utilisez le code avec précaution. En savoir plus
Commentaires et explications

Les propriétés nom, age et salaire sont déclarées privées.
Les méthodes getNom(), setNom(), getAge(), setAge() et getSalaire() sont déclarées publiques.
Les méthodes getNom()
Sources
gayerie.dev/epsi-b3-javaee/javaee_web/jsf.html
github.com/Orann/gestion_parc_attraction


### Concept 6 : Abstraction

L'abstraction est le processus de masquage des détails d'une classe aux utilisateurs de la classe.

Exemple de code

Java
public abstract class Vehicule {

    // Propriétés
    private String marque;
    private String modele;

    // Constructeur
    public Vehicule(String marque, String modele) {
        this.marque = marque;
        this.modele = modele;
    }

    // Méthodes abstraites
    public abstract void rouler();

    public abstract void freiner();

}

public class Voiture extends Vehicule {

    // Propriétés
    private int nombreDePortes;

    // Constructeur
    public Voiture(String marque, String modele, int nombreDePortes) {
        super(marque, modele);
        this.nombreDePortes = nombreDePortes;
    }

    // Méthodes implémentées
    @Override
    public void rouler() {
        System.out.println("La voiture roule.");
    }

    @Override
    public void freiner() {
        System.out.println("La voiture freine.");
    }

}

public class Moto extends Vehicule {

    // Propriétés
    private int nombreDeCylindres;

    // Constructeur
    public Moto(String marque, String modele, int nombreDeCylindres) {
        super(marque, modele);
        this.nombreDeCylindres = nombreDeCylindres;
    }

    // Méthodes implémentées
    @Override
    public void rouler() {
        System.out.println("La moto roule.");
    }

    @Override
    public void freiner() {
        System.out.println("La moto freine.");
    }

}
Utilisez le code avec précaution. En savoir plus
Commentaires et explications

La classe Vehicule est une classe abstraite.
Les classes Voiture et Moto héritent de la classe Vehicule.
Les classes Voiture et Moto implémentent les méthodes abstraites rouler() et freiner().
Utilité du concept

L'abstraction permet de simplifier le code en permettant de regrouper des propriétés et des comportements communs dans une classe abstraite.
Cela permet d'écrire du code qui est plus générique et plus extensible.
Exemple d'utilisation

Dans l'exemple de code, la classe Vehicule représente un concept générique de véhicule.
Les classes Voiture et Moto représentent des types spécifiques de véhicules.


### Concept 7 : Composition

La composition est une relation entre deux classes où une classe, la classe composite, contient une référence à une autre classe, la classe composante.

Exemple de code

Java
public class Voiture {

    // Propriétés
    private Moteur moteur;

    // Constructeur
    public Voiture(Moteur moteur) {
        this.moteur = moteur;
    }

    // Méthodes
    public void rouler() {
        moteur.demarrer();
        moteur.accelerer();
    }

}

public class Moteur {

    // Propriétés
    private int cylindre;

    // Constructeur
    public Moteur(int cylindre) {
        this.cylindre = cylindre;
    }

    // Méthodes
    public void demarrer() {
        System.out.println("Le moteur démarre.");
    }

    public void accelerer() {
        System.out.println("Le moteur accélère.");
    }

}
Utilisez le code avec précaution. En savoir plus
Commentaires et explications

La classe Voiture contient une référence à la classe Moteur.
La classe Moteur est une composante de la classe Voiture.
Utilité du concept

La composition permet de modéliser des objets complexes composés de plusieurs objets plus simples.
Cela permet d'écrire du code


### Concept 8 : Agrégation

L'agrégation est une relation entre deux classes où une classe, la classe agrégée, contient une référence à une autre classe, la classe agrégée.

Exemple de code

Java
public class Voiture {

    // Propriétés
    private Moteur moteur;

    // Constructeur
    public Voiture(Moteur moteur) {
        this.moteur = moteur;
    }

    // Méthodes
    public void rouler() {
        moteur.demarrer();
        moteur.accelerer();
    }

}

public class Moteur {

    // Propriétés
    private int cylindre;

    // Constructeur
    public Moteur(int cylindre) {
        this.cylindre = cylindre;
    }

    // Méthodes
    public void demarrer() {
        System.out.println("Le moteur démarre.");
    }

    public void accelerer() {
        System.out.println("Le moteur accélère.");
    }

}
Utilisez le code avec précaution. En savoir plus
Commentaires et explications

La classe Voiture contient une référence à la classe Moteur.
La classe Moteur n'est pas une composante de la classe Voiture.
Utilité du concept

L'agrégation permet de modéliser des objets complexes composés de plusieurs objets plus simples.
Cela permet d'écrire du code qui est plus flexible.
Exemple d'utilisation

Dans l'exemple de code, la classe Voiture représente un objet complexe composé d'un objet Moteur.
La classe Moteur n'est pas une composante de la classe Voiture, elle peut être remplacée par une autre classe Moteur.

### Concept 9 : Interface

Une interface est une définition d'un ensemble de méthodes.

Exemple de code

Java
public interface Vehicule {

    void rouler();

    void freiner();

}

public class Voiture implements Vehicule {

    // Propriétés
    private String marque;
    private String modele;

    // Constructeur
    public Voiture(String marque, String modele) {
        this.marque = marque;
        this.modele = modele;
    }

    // Méthodes implémentées
    @Override
    public void rouler() {
        System.out.println("La voiture roule.");
    }

    @Override
    public void freiner() {
        System.out.println("La voiture freine.");
    }

}

public class Moto implements Vehicule {

    // Propriétés
    private String marque;
    private String modele;

    // Constructeur
    public Moto(String marque, String modele) {
        this.marque = marque;
        this.modele = modele;
    }

    // Méthodes implémentées
    @Override
    public void rouler() {
        System.out.println("La moto roule.");
    }

    @Override
    public void freiner() {
        System.out.println("La moto freine.");
    }

}
Utilisez le code avec précaution. En savoir plus
Commentaires et explications

L'interface Vehicule définit les méthodes rouler() et freiner().
Les classes Voiture et Moto implémentent l'interface Vehicule.
Utilité du concept

Les interfaces permettent de définir un contrat entre les classes.
Cela permet d'écrire du code qui est plus flexible et plus réutilisable.
Exemple d'utilisation

Dans l'exemple de code, l'interface Vehicule définit le comportement de base d'un véhicule.
Les classes Voiture et Moto implémentent l'interface Vehicule pour fournir des implementations spécifiques de ce comportement.
