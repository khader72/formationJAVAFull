Jour 3: Java Avancée, Collections, Threads, Exceptions, Logs, Javadoc, Tests Unitaires, et Maven

Quelle interface Java est utilisée pour implémenter des listes ordonnées ?

A. List
B. SortedSet
C. Map
D. Queue
E. Set
Comment pouvez-vous trier une liste d'objets en Java en utilisant une méthode de comparaison personnalisée ?

A. En implémentant l'interface Sortable pour chaque objet
B. En utilisant la méthode Collections.sort(list, comparator)
C. En appelant la méthode list.sort(comparator)
D. En appelant la méthode list.order(comparator)
E. En utilisant la méthode list.sortBy(comparator)
Quel mécanisme Java permet d'exécuter plusieurs threads simultanément ?

A. Héritage de la classe Thread
B. Implémentation de l'interface Runnable
C. Utilisation de la classe ExecutorService
D. Toutes les réponses ci-dessus
E. Aucune des réponses ci-dessus
Quelle classe Java est utilisée pour gérer les exceptions liées aux entrées-sorties (I/O) ?

A. IOException
B. FileException
C. InputOutputException
D. ExceptionIO
E. IOExceptionHandler
Quelle est la différence entre System.out.print() et System.out.println() en termes de sortie ?

A. System.out.print() imprime sur une nouvelle ligne, System.out.println() imprime sur la même ligne
B. System.out.print() imprime en rouge, System.out.println() imprime en bleu
C. System.out.print() n'imprime rien, System.out.println() imprime sur une nouvelle ligne
D. System.out.print() imprime sur une nouvelle ligne, System.out.println() imprime sur la même ligne et ajoute une nouvelle ligne
E. System.out.print() imprime en majuscules, System.out.println() imprime en minuscules
Quelle annotation est utilisée pour générer la documentation à partir du code source Java ?

A. @DocGen
B. @GenerateDoc
C. @Documentation
D. @JavaDoc
E. @Documented
Quel outil est utilisé pour générer automatiquement la documentation à partir des commentaires Java dans le code source ?

A. JavaDoc
B. JavaDocs
C. JavaDocumentor
D. JavaDocGen
E. JavaDocBuilder
Quelle méthode est utilisée pour générer une exception personnalisée en Java ?

A. throw CustomException("Message")
B. throw new Exception("Message")
C. throw CustomException("Message").build()
D. throw new CustomException("Message")
E. throw Exception("Message")
Quelle classe est utilisée pour implémenter des logs dans une application Java ?

A. Logger
B. LogManager
C. LogWriter
D. LogFactory
E. LogHandler
Comment pouvez-vous capturer et gérer les logs dans un fichier dans Java ?

A. En utilisant un système de fichiers spécifique pour les logs
B. En utilisant System.out.println() pour imprimer les logs dans un fichier
C. En configurant un gestionnaire de logs (Handler) qui écrit dans un fichier
D. En écrivant manuellement les logs dans un fichier à l'aide de FileWriter
E. Java ne prend pas en charge l'écriture des logs dans un fichier
Quelle est la méthode principale utilisée pour écrire un commentaire dans Javadoc ?

A. @comment
B. // Comment
C. /* Comment */
D. # Comment
E. /** Comment */
Quel est le framework de test unitaire standard pour les applications Java ?

A. JUnit
B. TestNG
C. JavaUnit
D. UnitTest
E. TestJava
Quelle annotation est utilisée pour indiquer que la méthode annotée est un test unitaire dans JUnit ?

A. @Test
B. @UnitTest
C. @TestUnit
D. @Unit
E. @JUnitTest
Quel outil est utilisé pour gérer les dépendances, construire et tester des projets Java de manière automatisée ?

A. Gradle
B. Ant
C. Maven
D. Jenkins
E. Eclipse
Quelle est la commande Maven pour exécuter les tests unitaires d'un projet ?

A. mvn test
B. mvn run-tests
C. mvn unit-test
D. mvn execute-tests
E. mvn test-unit
Quelle méthode est utilisée pour écrire un message d'erreur dans les logs en utilisant le framework de logging SLF4J ?

A. Log.error("Message")
B. Logger.error("Message")
C. Log.error("Message", exception)
D. Logger.error("Message", exception)
E. SLF4J.error("Message")
Quel est l'avantage principal de l'utilisation de l'annotation @Override dans Java ?

A. Elle permet d'indiquer qu'une méthode est privée et ne peut pas être modifiée.
B. Elle indique que la méthode annotée est une surcharge d'une méthode parente.
C. Elle indique que la méthode annotée est une implémentation d'une interface.
D. Elle provoque une erreur de compilation si la méthode annotée ne surcharge pas correctement une méthode parente.
E. Elle indique que la méthode annotée est publique et peut être appelée depuis n'importe où dans le code.
Quel est l'avantage principal de l'utilisation de l'opérateur synchronized en Java ?

A. Il garantit qu'une méthode est exécutée par un seul thread à la fois.
B. Il permet d'accéder aux éléments d'une liste de manière synchronisée.
C. Il effectue une opération de tri synchronisé sur une collection.
D. Il autorise l'accès concurrent à des ressources partagées sans conflits.
E. Il interrompt l'exécution d'un thread de manière synchronisée.
Comment pouvez-vous créer un thread en Java en implémentant l'interface Runnable ?

A. En instanciant un objet de la classe Thread et en lui passant une instance de la classe implémentant Runnable.
B. En instanciant directement un objet de la classe Runnable.
C. En appelant la méthode run() de l'interface Runnable.
D. En utilisant l'annotation @RunnableThread.
E. En étendant la classe Runnable et en implémentant la méthode run().
Quel est le rôle de l'instruction finally dans un bloc try-catch-finally en Java ?

A. Le bloc finally est exécuté uniquement si une exception est levée.
B. Le bloc finally est exécuté uniquement si aucune exception n'est levée.
C. Le bloc finally est toujours exécuté, qu'une exception soit levée ou non.
D. Le bloc finally est ignoré et n'a aucun effet sur l'exécution du programme.
E. Le bloc finally est utilisé pour déclarer une exception personnalisée.
Quelle est la méthode principale de la classe Object que vous pouvez surcharger pour fournir une représentation textuelle de votre objet ?

A. toString()
B. getText()
C. getString()
D. represent()
E. textRepresentation()
Comment pouvez-vous arrêter l'exécution d'un thread en Java ?

A. En appelant la méthode stop() sur le thread.
B. En appelant la méthode halt() sur le thread.
C. En appelant la méthode end() sur le thread.
D. En appelant la méthode interrupt() sur le thread.
E. En appelant la méthode finish() sur le thread.
Quel est le format de fichier standard utilisé pour générer la documentation Javadoc ?

A. .java
B. .doc
C. .md
D. .html
E. .txt
Quelle commande Maven est utilisée pour effectuer un build du projet et générer un fichier JAR exécutable ?

A. mvn compile
B. mvn package
C. mvn build
D. mvn deploy
E. mvn generate-jar
Quelle est l'utilité de l'instruction assert en Java ?

A. Elle arrête l'exécution du programme si la condition spécifiée est fausse.
B. Elle imprime un message d'erreur à la console si la condition spécifiée est vraie.
C. Elle crée un nouvel objet assert pour la gestion des erreurs.
D. Elle vérifie la validité syntaxique du code Java.
E. Elle génère un avertissement de compilation pour la ligne de code spécifiée.
