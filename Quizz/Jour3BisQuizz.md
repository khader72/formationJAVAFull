Série de Questions Hybrides (Difficulté Haute)

Question sur la Programmation Objet :
Considérez la classe suivante :

java
Copy code
class Animal {
    protected String sound;

    public Animal() {
        this.sound = "Unknown";
    }

    public void makeSound() {
        System.out.println("Animal sound: " + sound);
    }
}

class Dog extends Animal {
    public Dog() {
        this.sound = "Bark";
    }

    @Override
    public void makeSound() {
        System.out.println("Dog sound: " + sound);
    }
}
Quel sera le résultat de l'appel suivant :

java
Copy code
Animal myDog = new Dog();
myDog.makeSound();
A. "Animal sound: Unknown"
B. "Dog sound: Bark"
C. "Bark"
D. Cela entraînera une erreur de compilation.
E. Cela entraînera une exception à l'exécution.
Question sur les Collections :
Considérez le code suivant :

java
Copy code
List<String> list = new ArrayList<>();
list.add("A");
list.add("B");
list.add("C");
list.add("A");
list.add("B");
System.out.println(list.stream().distinct().count());
Quel sera le résultat de l'exécution de ce code ?

A. 3
B. 4
C. 5
D. 2
E. 6
Question sur les Exceptions :
Considérez le code suivant :

java
Copy code
class CustomException extends Exception {
    public CustomException(String message) {
        super(message);
    }
}

public class Example {
    public static void main(String[] args) throws CustomException {
        try {
            throw new CustomException("An error occurred");
        } catch (CustomException e) {
            System.out.println(e.getMessage());
            throw e;
        } finally {
            System.out.println("Finally block executed");
        }
    }
}
Quel sera le résultat de l'exécution de ce code ?

A. "An error occurred" suivi de "Finally block executed".
B. "An error occurred".
C. "Finally block executed".
D. Une exception sera levée sans message.
E. Cela entraînera une erreur de compilation.
Question sur les Lambdas :
Considérez le code suivant :

java
Copy code
List<String> names = Arrays.asList("Alice", "Bob", "Charlie", "David");

names.stream()
     .filter(name -> name.length() > 4)
     .map(String::toUpperCase)
     .forEach(System.out::println);
Quelle sera la sortie de ce code ?

A. "Alice", "Bob", "Charlie", "David"
B. "ALICE", "BOB", "CHARLIE", "DAVID"
C. "Charlie", "David"
D. "ALICE", "CHARLIE", "DAVID"
E. Aucune sortie, une exception sera levée.
Question sur les Threads :
Considérez le code suivant :

java
Copy code
public class Example {
    private static int count = 0;

    public static synchronized void increment() {
        count++;
    }

    public static void main(String[] args) {
        Thread t1 = new Thread(() -> {
            for (int i = 0; i < 1000; i++) {
                increment();
            }
        });

        Thread t2 = new Thread(() -> {
            for (int i = 0; i < 1000; i++) {
                increment();
            }
        });

        t1.start();
        t2.start();

        try {
            t1.join();
            t2.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        System.out.println("Count: " + count);
    }
}
Quel sera le résultat de l'exécution de ce code ?

A. "Count: 1000"
B. "Count: 2000"
C. Un nombre différent à chaque exécution.
D. Une exception sera levée.
E. "Count: 0"
Question sur les Streams :
Considérez le code suivant :

java
Copy code
List<String> words = Arrays.asList("Java", "is", "a", "powerful", "and", "flexible", "language");

String result = words.stream()
                   .filter(s -> s.length() > 3)
                   .map(String::toUpperCase)
                   .reduce((s1, s2) -> s1 + " " + s2)
                   .orElse("");

System.out.println(result);
Quelle sera la sortie de ce code ?

A. "JAVA IS POWERFUL FLEXIBLE LANGUAGE"
B. "Java is powerful flexible language"
C. "Java Powerful Flexible Language"
D. "Java IS Powerful AND Flexible Language"
E. Aucune sortie, une exception sera levée.
Question sur les Annotations :
Considérez le code suivant :

java
Copy code
public class Example {
    @Deprecated
    public void oldMethod() {
        System.out.println("This is an old method.");
    }

    public static void main(String[] args) {
        Example obj = new Example();
        obj.oldMethod();
    }
}
Quel sera le comportement de ce code ?

A. Il ne compilera pas en raison de l'annotation @Deprecated.
B. Il compilera et affichera "This is an old method.".
C. Il compilera mais affichera un avertissement indiquant que la méthode est obsolète.
D. Il compilera et ne produira aucune sortie.
E. Il compilera mais l'exécution entraînera une exception.
Question sur les Expressions Régulières :
Considérez le code suivant :

java
Copy code
import java.util.regex.Matcher;
import java.util.regex.Pattern;

public class Example {
    public static void main(String[] args) {
        String text = "The price of the product is $25.50";
        Pattern pattern = Pattern.compile("\\$(\\d+\\.\\d+)");
        Matcher matcher = pattern.matcher(text);

        if (matcher.find()) {
            System.out.println("Price: " + matcher.group(1));
        } else {
            System.out.println("Price not found.");
        }
    }
}
Quel sera le résultat de l'exécution de ce code ?

A. "Price: $25.50"
B. "Price: 25.50"
C. "Price not found."
D. Il y aura une erreur de compilation.
E. "The price of the product is $25.50"
Question sur les Classes Internes :
Considérez le code suivant :

java
Copy code
public class Outer {
    private int data = 10;

    class Inner {
        public void display() {
            System.out.println("Data is " + data);
        }
    }

    public static void main(String[] args) {
        Outer outer = new Outer();
        Outer.Inner inner = outer.new Inner();
        inner.display();
    }
}
Quel sera le résultat de l'exécution de ce code ?

A. "Data is 0"
B. "Data is 10"
C. Il y aura une erreur de compilation.
D. "Data is null"
E. "Data is not accessible."
Question sur JavaFX :
Considérez le code suivant :

java
Copy code
import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.layout.StackPane;
import javafx.stage.Stage;

public class Example extends Application {
    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {
        primaryStage.setTitle("JavaFX Example");

        Button btn = new Button("Click Me!");
        btn.setOnAction(event -> System.out.println("Button clicked!"));

        StackPane root = new StackPane();
        root.getChildren().add(btn);
        primaryStage.setScene(new Scene(root, 300, 250));
        primaryStage.show();
    }
}
Quel sera le comportement de ce programme JavaFX ?

A. Il ne compilera pas en raison d'une erreur liée à JavaFX.
B. Il compilera mais ne produira aucune sortie.
C. Il compilera et affichera une fenêtre avec un bouton. En cliquant sur le bouton, il affichera "Button clicked!" dans la console.
D. Il compilera mais ne permettra pas de cliquer sur le bouton.
E. Il compilera mais affichera une exception à l'exécution.
Réponses :

B
A
A
D
C
A
C
B
B
C
