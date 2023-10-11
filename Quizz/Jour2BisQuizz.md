## Série de Questions Hybrides (Difficulté Moyenne)

Quel est le résultat de l'expression 3 * 5 + 4 / 2 en Java ?

A. 8
B. 9
C. 11
D. 13
E. 15
Quelle est la différence entre les variables d'instance et les variables de classe en Java ?

A. Les variables d'instance sont partagées entre toutes les instances de la classe, tandis que les variables de classe sont propres à chaque instance.
B. Les variables d'instance sont déclarées avec le mot-clé static, tandis que les variables de classe ne le sont pas.
C. Les variables d'instance sont utilisées pour stocker des valeurs constantes, tandis que les variables de classe sont utilisées pour stocker des valeurs modifiables.
D. Les variables d'instance sont déclarées à l'intérieur des méthodes, tandis que les variables de classe sont déclarées à l'extérieur des méthodes.
E. Les variables d'instance sont initialisées lors de la création de chaque instance de la classe, tandis que les variables de classe sont initialisées lors de la définition de la classe.
Quel est le résultat de l'exécution du code suivant ?

java
Copy code
String str = "Bonjour";
str.concat(" Monde");
System.out.println(str);
A. "Bonjour"
B. "Bonjour Monde"
C. " Monde"
D. La compilation échouera.
E. Une exception sera levée à l'exécution.
Quelle est la principale différence entre ArrayList et LinkedList en Java ?

A. ArrayList stocke les éléments sous forme de tableau dynamique, tandis que LinkedList stocke les éléments sous forme de liste doublement chaînée.
B. ArrayList ne peut pas stocker d'éléments de types primitifs, tandis que LinkedList le peut.
C. ArrayList utilise moins de mémoire que LinkedList.
D. LinkedList offre un meilleur accès aléatoire aux éléments que ArrayList.
E. LinkedList ne peut pas être modifié après sa création, tandis qu'ArrayList le peut.
Comment peut-on trier une liste d'objets personnalisés en utilisant une méthode de comparaison externe en Java ?

A. En implémentant l'interface Comparable dans la classe de l'objet personnalisé.
B. En appelant la méthode sort() de la classe Collections avec un objet de comparaison personnalisé.
C. En appelant la méthode sort() directement sur la liste avec un objet de comparaison personnalisé.
D. En appelant la méthode sorted() sur la liste avec un objet de comparaison personnalisé.
E. En appelant la méthode order() de la classe Collections avec un objet de comparaison personnalisé.
Quelle est la différence entre une interface fonctionnelle et une interface normale en Java ?

A. Une interface fonctionnelle a une seule méthode abstraite, tandis qu'une interface normale peut avoir plusieurs méthodes abstraites.
B. Une interface fonctionnelle ne peut pas avoir de méthodes abstraites, tandis qu'une interface normale peut en avoir plusieurs.
C. Une interface fonctionnelle peut avoir des méthodes par défaut, tandis qu'une interface normale ne le peut pas.
D. Une interface fonctionnelle ne peut pas être utilisée comme type de référence, tandis qu'une interface normale peut l'être.
E. Il n'y a pas de différence significative entre les deux.
Quelle est la différence entre throw et throws en Java ?

A. throw est utilisé pour lever une exception spécifique, tandis que throws est utilisé pour déclarer que la méthode peut lancer certaines exceptions.
B. throw est utilisé pour déclarer une exception, tandis que throws est utilisé pour lancer une exception.
C. throw est utilisé pour intercepter une exception, tandis que throws est utilisé pour traiter une exception.
D. throw est utilisé pour définir un gestionnaire d'exceptions personnalisé, tandis que throws est utilisé pour déclarer les exceptions standard de Java.
E. Il n'y a pas de différence entre les deux.
Quelle est la différence entre super et this en Java ?

A. super est utilisé pour appeler une méthode de la classe parente, tandis que this est utilisé pour appeler une méthode de la classe courante.
B. super est utilisé pour référencer l'objet courant, tandis que this est utilisé pour référencer l'objet parent.
C. super est utilisé pour référencer une variable de la classe parente, tandis que this est utilisé pour référencer une variable de la classe courante.
D. super est utilisé pour initialiser une variable de la classe parente, tandis que this est utilisé pour initialiser une variable de la classe courante.
E. super et this sont interchangeables et peuvent être utilisés de la même manière.
Quelle est la sortie de ce code ?

java
Copy code
public class Test {
    public static void main(String[] args) {
        String str1 = "Hello";
        String str2 = new String("Hello");
        System.out.println(str1 == str2);
    }
}
A. true
B. false
C. Il y aura une erreur de compilation.
D. "Hello"
E. Cela entraînera une exception à l'exécution.
Quelle est la sortie de ce code ?
java
Copy code
public class Test {
    public static void main(String[] args) {
        int x = 5;
        System.out.println(x++ * ++x);
    }
}
A. 30
B. 35
C. 40
D. 25
E. 42
Quelle déclaration de variable est invalide en Java ?
A. int _value = 10;
B. double 123value = 10.5;
C. float floatVal = 5.6f;
D. String $name = "John";
E. char charVal = 'A';
Comment peut-on créer un thread en Java en implémentant l'interface Runnable de manière anonyme ?
A. Thread t = new Thread(new Runnable() { /* implementation */ });
B. Runnable r = new Runnable() { /* implementation */ }; Thread t = new Thread(r);
C. Thread t = new Thread(Runnable.run() { /* implementation */ });
D. Thread t = new Thread(Runnable { /* implementation */ });
E. Thread t = new Thread(Runnable -> { /* implementation */ });
Quelle méthode de l'interface Runnable est responsable de l'exécution du thread ?
A. run()
B. execute()
C. start()
D. process()
E. begin()
Quelle est la sortie de ce code ?
java
Copy code
public class Test {
    public static void main(String[] args) {
        String str = "hello";
        str.toUpperCase();
        System.out.println(str);
    }
}
A. "hello"
B. "HELLO"
C. "Hello"
D. Cela entraînera une erreur de compilation.
E. Cela entraînera une exception à l'exécution.
Quel est le résultat de l'expression logique suivante ?
java
Copy code
boolean x = true;
boolean y = false;
boolean z = x && (y = true);
System.out.println(z);
A. true
B. false
C. true, mais y reste false
D. false, mais y devient true
E. Cela entraînera une erreur de compilation.
Quel est le rôle de l'annotation @FunctionalInterface en Java ?
A. Indiquer qu'une interface peut avoir une seule méthode abstraite et peut être utilisée pour la programmation fonctionnelle.
B. Indiquer qu'une interface ne peut avoir aucune méthode abstraite et doit être utilisée comme une classe abstraite.
C. Indiquer qu'une interface peut avoir plusieurs méthodes abstraites et doit être implémentée comme une classe concrète.
D. Indiquer qu'une interface ne peut avoir que des méthodes statiques.
E. Indiquer qu'une interface ne peut avoir que des méthodes par défaut.
Quel est le résultat de l'expression suivante ?
java
Copy code
int[] numbers = {1, 2, 3, 4, 5};
int sum = Arrays.stream(numbers)
                .filter(n -> n % 2 == 0)
                .sum();
System.out.println(sum);
A. 6
B. 9
C. 10
D. 15
E. 5
Quelle est la différence entre List.of() et Arrays.asList() en Java ?
A. List.of() crée une liste immuable, tandis que Arrays.asList() crée une liste modifiable.
B. List.of() crée une liste modifiable, tandis que Arrays.asList() crée une liste immuable.
C. Il n'y a pas de différence significative entre les deux.
D. List.of() peut être utilisé uniquement pour des objets de type primitif, tandis que Arrays.asList() peut être utilisé pour tous les types d'objets.
E. Arrays.asList() crée une liste immuable, tandis que List.of() crée une liste modifiable.
Quelle interface est utilisée pour trier des éléments dans un ordre naturel en Java ?
A. Sortable
B. Orderable
C. Comparable
D. Comparator
E. Sorter
Quel est le résultat de l'exécution du code suivant ?
java
Copy code
public class Test {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        list.add("A");
        list.add("B");
        list.add("C");

        list.forEach(System.out::print);
    }
}
A. "ABC"
B. "CBA"
C. "A B C"
D. Cela entraînera une erreur de compilation.
E. Cela entraînera une exception à l'exécution.
Quel est le rôle de l'annotation @SafeVarargs en Java ?
A. Indiquer qu'une méthode peut être appelée de manière sécurisée à partir de plusieurs threads.
B. Indiquer qu'une méthode accepte un nombre variable d'arguments de types sécurisés.
C. Indiquer qu'une méthode utilise des variables de types sécurisés.
D. Indiquer qu'une méthode peut générer une exception de type sécurisé.
E. Indiquer qu'une méthode peut être appelée de manière sécurisée à partir d'autres méthodes.
Quel est le résultat de l'exécution du code suivant ?
java
Copy code
public class Test {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 3, 4, 5};
        int sum = Arrays.stream(numbers)
                        .filter(n -> n % 2 != 0)
                        .map(n -> n * 2)
                        .sum();
        System.out.println(sum);
    }
}
A. 10
B. 12
C. 14
D. 15
E. 20
Quelle interface est utilisée pour effectuer des opérations atomiques sur les données en Java ?
A. Synchronized
B. Atomic
C. Lockable
D. Transactable
E. ThreadSafe
Quel est le résultat de l'exécution du code suivant ?
java
Copy code
public class Test {
    public static void main(String[] args) {
        int x = 5;
        int y = 2;
        int result = ++x * y--;
        System.out.println(result);
    }
}
A. 12
B. 14
C. 15
D. 10
E. 11
Quelle est la sortie de ce code ?
java
Copy code
public class Test {
    public static void main(String[] args) {
        String str = "Hello";
        str.concat(" World").trim();
        System.out.println(str);
    }
}
A. "Hello World"
B. "Hello World "
C. " Hello"
D. "Hello"
E. " World"
Réponses:

C
A
A
A
B
A
D
C
A
B
B
B
A
A
B
A
B
A
C
A
B
D
B
B
D
