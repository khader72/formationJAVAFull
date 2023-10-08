# TPs  Collections en JAVA


## Travail Pratique 1: Création et Manipulation de Listes

**Objectif :**

Créer une liste de chaînes de caractères, ajouter et supprimer des éléments, puis parcourir la liste.

```java

import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        // Création d'une liste de chaînes de caractères
        List<String> liste = new ArrayList<>();

        // Ajout d'éléments à la liste
        liste.add("Java");
        liste.add("Python");
        liste.add("C++");

        // Suppression d'un élément de la liste
        liste.remove("Python");

        // Parcours de la liste et affichage des éléments
        for (String langage : liste) {
            System.out.println(langage);
        }
    }
}
```

## Travail Pratique 2: Utilisation d'un Set pour Éliminer les Duplications

**Objectif :**

Utiliser un ensemble (Set) pour stocker des éléments uniques et comprendre comment il élimine les duplications automatiquement.

```java

import java.util.HashSet;
import java.util.Set;

public class Main {
    public static void main(String[] args) {
        // Création d'un ensemble de chaînes de caractères
        Set<String> ensemble = new HashSet<>();

        // Ajout d'éléments à l'ensemble (élimine automatiquement les doublons)
        ensemble.add("Java");
        ensemble.add("Python");
        ensemble.add("Java");

        // Affichage des éléments de l'ensemble
        for (String langage : ensemble) {
            System.out.println(langage);
        }
    }
}
```

## Travail Pratique 3: Utilisation d'une Map pour Stocker des Paires Clé-Valeur

**Objectif :**

Utiliser une carte (Map) pour stocker des paires clé-valeur et comprendre comment accéder aux éléments via leurs clés.

```java

import java.util.HashMap;
import java.util.Map;

public class Main {
    public static void main(String[] args) {
        // Création d'une carte de langages et de leurs années de création
        Map<String, Integer> langages = new HashMap<>();

        // Ajout de paires clé-valeur à la carte
        langages.put("Java", 1995);
        langages.put("Python", 1991);
        langages.put("C++", 1985);

        // Accès aux éléments via leurs clés et affichage
        System.out.println("Année de création de Java : " + langages.get("Java"));
        System.out.println("Année de création de Python : " + langages.get("Python"));
    }
}
```

## Travail Pratique 4: Tri d'une Liste d'Objets Personnalisés

**Objectif :**

Créer une liste d'objets personnalisés, puis trier cette liste en fonction de certains critères.

```java

import java.util.ArrayList;
import java.util.Collections;
import java.util.List;

class Personne {
    String nom;

    Personne(String nom) {
        this.nom = nom;
    }
}

public class Main {
    public static void main(String[] args) {
        // Création d'une liste de personnes
        List<Personne> personnes = new ArrayList<>();
        personnes.add(new Personne("Alice"));
        personnes.add(new Personne("Bob"));
        personnes.add(new Personne("Charlie"));

        // Tri de la liste de personnes par leur nom
        Collections.sort(personnes, (p1, p2) -> p1.nom.compareTo(p2.nom));

        // Affichage des personnes triées
        for (Personne personne : personnes) {
            System.out.println(personne.nom);
        }
    }
}
```

## Travail Pratique 5: Utilisation d'une Queue pour un Système de Files d'Attente

**Objectif :**

Utiliser une file (Queue) pour implémenter un système de files d'attente pour un service.

```java

import java.util.LinkedList;
import java.util.Queue;

class ServiceClient {
    String nom;

    ServiceClient(String nom) {
        this.nom = nom;
    }
}

public class Main {
    public static void main(String[] args) {
        // Création d'une file d'attente pour le service
        Queue<ServiceClient> fileAttente = new LinkedList<>();

        // Ajout de clients à la file d'attente
        fileAttente.offer(new ServiceClient("Client 1"));
        fileAttente.offer(new ServiceClient("Client 2"));
        fileAttente.offer(new ServiceClient("Client 3"));

        // Traitement des clients dans l'ordre de leur arrivée
        while (!fileAttente.isEmpty()) {
            ServiceClient client = fileAttente.poll();
            System.out.println("Service en cours pour : " + client.nom);
        }
    }
}
```
