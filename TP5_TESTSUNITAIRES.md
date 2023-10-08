# TP 1 : Définition des tests unitaires

## Objectif

Découvrir la définition des tests unitaires.

## Étapes

1. Lire la définition des tests unitaires


Les tests unitaires sont des tests logiciels qui vérifient le bon fonctionnement d'une unité de code, généralement une méthode ou une classe. Ils sont essentiels pour garantir la qualité du code et éviter les bugs.

Les tests unitaires doivent être :

* **Indépendants** : chaque test doit tester une seule unité de code.
* **Réutilisables** : les tests doivent pouvoir être exécutés à tout moment, sans avoir à modifier le code source.
* **Autonomiser** : les tests doivent pouvoir être exécutés sans avoir à démarrer l'application complète.


2. Identifier les avantages des tests unitaires

* Garantie de la qualité du code
* Prévention des bugs
* Amélioration de la productivité
* Réduction des coûts de développement

3. Discuter des inconvénients des tests unitaires

* Temps et effort supplémentaires
* Coût de maintenance
* Complexité des tests

## Conclusion

Les tests unitaires sont une partie essentielle du développement logiciel. Ils permettent de garantir la qualité du code et éviter les bugs.

## Exercices supplémentaires

* Écrire une définition des tests unitaires en vos propres mots.
* Discuter des avantages et des inconvénients des tests unitaires avec un collègue.

# TP 2 : Écrire des tests unitaires

## Objectif

Apprendre à écrire des tests unitaires.

## Étapes

1. Identifier les unités de code à tester


Dans cet exemple, nous allons tester la méthode `somme()` qui calcule la somme de deux nombres.



2. Définir les cas de test

* **Cas de test 1 : Les deux nombres sont positifs.**
* **Cas de test 2 : Un des deux nombres est négatif.**

### Écrire le code des tests

```java
import org.junit.jupiter.api.Assertions;
import org.junit.jupiter.api.Test;

public class SommeTest {

    @Test
    public void sommeDeDeuxNombresPositifs() {
        int a = 10;
        int b = 20;

        int resultatAttendu = 30;
        int resultatReel = Somme.somme(a, b);

        Assertions.assertEquals(resultatAttendu, resultatReel);
    }

    @Test
    public void sommeDeDeuxNombresUnNombreNegatif() {
        int a = 10;
        int b = -20;

        int resultatAttendu = -10;
        int resultatReel = Somme.somme(a, b);

        Assertions.assertEquals(resultatAttendu, resultatReel);
    }

}
```

**Execution**

```
├── src
│   └── main
│       └── java
│           └── com
│               └── tests
│                   └── SommeTest.java
└── test
    └── resources
        └── log4j.properties

```

```
[INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.025 s - in com.tests.SommeTest
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  0.055 s
[INFO] Finished at: 2023-07-20T15:39:50+02:00
[INFO] ------------------------------------------------------------------------
```
## Résultat

Les deux tests ont réussi.

## Commentaires

Les tests sont écrits dans un fichier .java avec l'annotation @Test. Chaque test contient une méthode qui teste...

