# Formation JAVA Web

Formation  JAVA  Full


## JavaDoc

* https://docs.oracle.com/en/java/javase/11/docs/api/
  
##  TOP  Sites WebS

* https://www.programiz.com/java-programming/hello-world
* https://www.programiz.com/java-programming
* https://www.geeksforgeeks.org/introduction-to-java/


## TOP Autoformation

-https://www.programiz.com/java-programming

  
- https://www.sololearn.com/

- https://ide.geeksforgeeks.org/online-java-compiler

- 

## Les Outils JAVA JEE

- JDK  JAVA 11
- Maven
- ECLIPSE IDE
- VS CODE


## IDE JAVA en Ligne /Web

- https://www.programiz.com/java-programming/online-compiler/
- https://www.programiz.com/java-programming/hello-world

  
## JAVA Web  Spring Boot

## Mots-Clés Java


Java est un langage de programmation orienté objet populaire avec un ensemble spécifique de mots-clés réservés. 
En Java, il y a un total de **50 mots-clés réservés**. 30 sur 50 sont des indispensables.
Voici quelques-uns des mots-clés les plus utilisés en Java :

| Mots-Clés | Explication | Exemple |
| --- | --- | --- |
| **public** | Déclare un membre d'une classe comme accessible depuis n'importe où. | `public class MyClass { }` |
| **private** | Déclare un membre d'une classe comme accessible uniquement à l'intérieur de la classe. | `private int myVar;` |
| **protected** | Déclare un membre d'une classe comme accessible à l'intérieur de la classe et de ses sous-classes. | `protected void myMethod() { }` |
| **static** | Indique qu'une méthode ou un champ appartient à la classe plutôt qu'à une instance spécifique. | `static int myStaticVar;` |
| **final** | Indique que la méthode, la classe ou la variable est immuable et ne peut pas être modifiée. | `final double PI = 3.14;` |
| **abstract** | Indique qu'une classe ou une méthode n'a pas d'implémentation dans le contexte actuel. | `abstract class MyAbstractClass { }` |
| **interface** | Déclare une interface. | `interface MyInterface { }` |
| **implements** | Indique qu'une classe implémente une interface. | `class MyClass implements MyInterface { }` |
| **extends** | Indique qu'une classe hérite d'une autre classe. | `class ChildClass extends ParentClass { }` |
| **super** | Référence à la classe parente immédiate d'un objet. | `super.myMethod();` |
| **this** | Référence à l'instance courante de l'objet. | `this.myVar = 10;` |
| **if** | Conditionnelle (si). | `if (condition) { // code à exécuter }` |
| **else** | Branche alternative dans une structure conditionnelle. | `if (condition) { // code } else { // code }` |
| **for** | Boucle for. | `for (int i = 0; i < 10; i++) { // code }` |
| **while** | Boucle tant que. | `while (condition) { // code }` |
| **do** | Boucle faire... tant que. | `do { // code } while (condition);` |
| **switch** | Structure de commutation. | `switch (variable) { case value: // code; break; }` |
| **case** | Branche d'une structure de commutation. | `case 1: // code; break;` |
| **break** | Sort de la boucle ou de la structure de commutation. | `break;` |
| **continue** | Passe à l'itération suivante d'une boucle. | `continue;` |
| **return** | Renvoie une valeur d'une méthode. | `return result;` |
| **void** | Indique qu'une méthode ne retourne aucune valeur. | `public void myMethod() { }` |
| **try** | Démarre un bloc de code à tester pour des exceptions. | `try { // code }` |
| **catch** | Gère les exceptions attrapées dans un bloc try. | `catch (Exception e) { // gestion de l'exception }` |
| **throw** | Lance une exception explicite. | `throw new MyException();` |
| **throws** | Indique qu'une méthode peut lancer certaines exceptions. | `public void myMethod() throws MyException { }` |
| **finally** | Définit un bloc de code à exécuter après un essai, qu'il y ait eu une exception ou non. | `finally { // code à exécuter }` |
| **new** | Alloue une nouvelle instance d'une classe. | `MyClass obj = new MyClass();` |
| **instanceof** | Vérifie si un objet est une instance d'une classe particulière ou d'une interface. | `if (obj instanceof MyClass) { // code }` |
| **import** | Utilisé pour importer des classes, interfaces, ou paquets. | `import myPackage.MyClass;` |
| **package** | Déclare un paquetage (package) de classes. | `package myPackage;` |

Cette liste n'est pas exhaustive, mais elle comprend certains des mots-clés les plus couramment utilisés en Java.

---


Java, en tant que langage de programmation orienté objet, utilise divers mots-clés pour définir la structure, le comportement et les contrôles dans le code source. Les mots-clés Java peuvent être regroupés en plusieurs catégories selon leur fonction.

---
  #### Catégories de Mots-Clés**

**Modificateurs de Classe**

| Modificateurs | Explication | Exemple |
|---------------|-------------|---------|
| `public`      | Indique que la classe est accessible partout. | `public class MaClasse { ... }` |
| `abstract`    | Indique qu'une classe ne peut pas être instanciée seule. | `abstract class MaClasse { ... }` |
| `final`       | Indique que la classe ne peut pas être étendue. | `final class MaClasse { ... }` |
| `strictfp`    | Assure une stricte conformité des calculs de virgule flottante. | `strictfp class MaClasse { ... }` |

 **Modificateurs d'Accès**

| Modificateurs | Explication | Exemple |
|---------------|-------------|---------|
| `public`      | Accessible partout. | `public int variable;` |
| `protected`   | Accessible dans la classe et ses sous-classes. | `protected int variable;` |
| `private`     | Accessible uniquement dans la classe. | `private int variable;` |

 **Contrôle de Flux**

| Mots-Clés      | Explication | Exemple |
|-----------------|-------------|---------|
| `if`            | Conditionnel, exécute un bloc de code si la condition est vraie. | `if (condition) { ... }` |
| `else`          | Sinon, exécute un bloc de code si la condition de `if` est fausse. | `if (condition) { ... } else { ... }` |
| `switch`        | Sélectionne un des nombreux blocs de code à exécuter. | `switch (variable) { case 1: ... break; case 2: ... break; default: ... }` |
| `case`          | Définit un cas à l'intérieur de la structure `switch`. | `case 1: ... break;` |
| `default`       | Définit le cas par défaut dans une structure `switch`. | `default: ... break;` |
| `while`         | Boucle qui exécute un bloc de code tant qu'une condition est vraie. | `while (condition) { ... }` |
| `do`            | Boucle qui exécute un bloc de code au moins une fois et tant qu'une condition est vraie. | `do { ... } while (condition);` |
| `for`           | Boucle qui est utilisée lorsqu'on connaît à l'avance le nombre d'itérations. | `for (initialisation; condition; mise à jour) { ... }` |
| `break`         | Sort de la boucle ou de la structure de contrôle la plus proche. | `while (true) { ... break; }` |
| `continue`      | Passe à l'itération suivante d'une boucle. | `for (int i = 0; i < 10; i++) { if (i == 5) continue; ... }` |
| `return`        | Termine l'exécution de la méthode et renvoie une valeur. | `return valeur;` |
| `throw`         | Lance une exception explicite. | `throw new MonException();` |
| `throws`        | Indique que la méthode peut lancer certaines exceptions. | `void maMethode() throws MonException { ... }` |

 **Modificateurs de Variable**

| Modificateurs | Explication | Exemple |
|---------------|-------------|---------|
| `final`       | Indique qu'une variable est une constante. | `final int MA_CONSTANTE = 10;` |
| `volatile`    | Indique que la variable peut être modifiée par des threads. | `volatile int maVariable;` |
| `transient`   | Indique que la variable n'est pas sérialisable. | `transient int maVariable;` |
| `static`      | Indique que la variable appartient à la classe plutôt qu'à l'instance. | `static int variableStatique;` |

 **Modificateurs de Méthode**

| Modificateurs | Explication | Exemple |
|---------------|-------------|---------|
| `abstract`    | Indique qu'une méthode n'a pas d'implémentation. | `abstract void maMethode();` |
| `final`       | Indique qu'une méthode ne peut pas être surchargée par les sous-classes. | `final void maMethode() { ... }` |
| `native`      | Indique qu'une méthode est implémentée dans du code natif, généralement en C ou en C++. | `native void maMethode();` |
| `static`      | Indique qu'une méthode appartient à la classe plutôt qu'à l'instance. | `static void maMethode() { ... }` |
| `synchronized`| Indique que la méthode ne peut être accédée que par un seul thread à la fois. | `synchronized void maMethode() { ... }` |
| `public`      | Accessible partout. | `public void maMethode() { ... }` |
| `protected`   | Accessible dans la classe et ses sous-classes. | `protected void maMethode() { ... }` |
| `private`     | Accessible uniquement dans la classe. | `private void maMethode() { ... }` |

**Classes, Objets et Héritage**

| Mots-Clés      | Explication | Exemple |
|-----------------|-------------|---------|
| `class`         | Définit une classe. | `class MaClasse { ... }` |
| `interface`     | Définit une interface. | `interface MonInterface { ... }` |
| `extends`       | Indique que la classe hérite d'une autre classe. | `class MaClasseFille extends MaClasseMere { ... }` |
| `implements`    | Indique qu'une classe implémente une interface. | `class MaClasse implements MonInterface { ... }` |
| `super`         | Référence à la classe mère. | `super.maMethode();` |
| `this`          | Référence à l'instance courante de la classe. | `this.maMethode();` |
| `new`           | Crée une nouvelle instance d'une classe. | `MaClasse monObjet = new MaClasse();` |

**Gestion des Erreurs**

| Mots-Clés      | Explication | Exemple |
|-----------------|-------------|---------|
| `try`           | Définit un bloc de code à tester pour des erreurs. | `try { ... }` |
| `catch`         | Attrape et gère les exceptions générées dans le bloc `try`. | `catch (MonException e) { ... }` |
| `finally`       | Définit un bloc de code à exécuter après l'exécution du bloc `try`, indépendamment de l'exception. | `finally { ... }` |
| `throw`         | Lance une exception explicite. | `throw new MonException();` |
| `throws`        | Indique que la méthode peut lancer certaines exceptions. | `void maMethode() throws MonException { ... }` |

 **Autres Mots-Clés**

| Mots-Clés      | Explication | Exemple |
|-----------------|-------------|---------|
| `package`       | Définit un package dans lequel les classes sont regroupées. | `package monPackage;` |
| `import`        | Importe des classes, des interfaces ou des packages dans le code. | `import java.util.ArrayList;` |
| `instanceof`    | Vérifie si un objet est une instance d'une classe ou d'une interface. | `if (objet instanceof MaClasse) { ... }` |
| `enum`          | Définit un type de données énuméré. | `enum Jours { LUNDI, MARDI, ... }` |

---




## Syntaxe



```java

public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, world!");
    }
}

```

Exemples de Code
Création d'une classe Java simple pour afficher "Hello, world!".

**Syntaxe Java**

| Élément | Syntaxe | Commentaire | Exemple |
|---------|---------|-------------|---------|
| Point-virgule | `;` | Sépare les instructions en Java. | `int x = 10;` |
| Parenthèses | `()` | Encapsule les paramètres dans les déclarations de méthode et dans les expressions. | `int sum = add(3, 5);` |
| Accolades | `{ }` | Encapsule les blocs de code. | `for (int i = 0; i < 5; i++) { /* code ici */ }` |
| Virgule | `,` | Sépare les éléments dans une liste ou les arguments d'une méthode. | `int x = 1, y = 2, z = 3;` |
| Opérateur d'attribution | `=` | Affecte une valeur à une variable. | `int x = 10;` |
| Opérateurs mathématiques | `+, -, *, /, %` | Effectuent des opérations mathématiques. | `int sum = x + y;` |
| Opérateurs de comparaison | `==, !=, >, <, >=, <=` | Comparent des valeurs et retournent un résultat booléen. | `if (x > y) { /* code ici */ }` |
| Opérateurs logiques | `&&, ||, !` | Effectuent des opérations logiques et retournent un résultat booléen. | `if (x > 0 && y > 0) { /* code ici */ }` |
| Opérateurs d'incrémentation/décrémentation | `++, --` | Incrémente ou décrémente une variable. | `x++;` |
| Opérateurs de concaténation | `+` | Concatène deux chaînes de caractères. | `String fullName = firstName + " " + lastName;` |
| Opérateurs ternaires | `? :` | Opérateur conditionnel, retourne une valeur en fonction d'une condition. | `int max = (x > y) ? x : y;` |





