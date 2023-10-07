
## TP sur l'E/S en Java

**Objectifs**

Comprendre les concepts de base de l'E/S en Java
Savoir lire et écrire des fichiers texte
Savoir lire et écrire des fichiers binaires
Exercice 1 : Lecture d'un fichier texte

Écrivez un programme Java qui lit le contenu d'un fichier texte et l'affiche sur la console.

**Explications**

Pour lire un fichier texte en Java, nous utilisons la classe FileReader. Cette classe fournit des méthodes pour lire les données d'un fichier texte caractère par caractère.

Pour ouvrir un fichier texte, nous utilisons la méthode open() de la classe FileReader. Cette méthode prend en paramètre un objet File qui représente le fichier à ouvrir.

Une fois le fichier ouvert, nous pouvons utiliser la méthode read() pour lire le prochain caractère du fichier. La méthode read() renvoie un entier représentant le caractère lu. Si le caractère est la fin de fichier, la méthode read() renvoie -1.

Pour fermer le fichier, nous utilisons la méthode close() de la classe FileReader.

### Exemple de code

Java
import java.io.File;
import java.io.FileReader;
import java.io.IOException;

public class LireFichierTexte {

    public static void main(String[] args) throws IOException {

        // Créer un objet File pour représenter le fichier à lire
        File fichier = new File("data.txt");

        // Ouvrir le fichier en lecture
        FileReader lecteur = new FileReader(fichier);

        // Lire le contenu du fichier
        while (true) {
            int caractere = lecteur.read();

            // Si on a atteint la fin de fichier, on s'arrête
            if (caractere == -1) {
                break;
            }

            // Afficher le caractère lu
            System.out.print((char) caractere);
        }

        // Fermer le fichier
        lecteur.close();
    }
}
Utilisez le code avec précaution. En savoir plus

### Exercice 2 : Écriture d'un fichier texte

Écrivez un programme Java qui écrit le contenu d'une chaîne de caractères dans un fichier texte.

Explications

Pour écrire un fichier texte en Java, nous utilisons la classe FileWriter. Cette classe fournit des méthodes pour écrire les données d'un fichier texte caractère par caractère.

Pour ouvrir un fichier texte, nous utilisons la méthode open() de la classe FileWriter. Cette méthode prend en paramètre un objet File qui représente le fichier à ouvrir.

Une fois le fichier ouvert, nous pouvons utiliser la méthode write() pour écrire le prochain caractère dans le fichier. La méthode write() prend en paramètre un entier représentant le caractère à écrire.

Pour fermer le fichier, nous utilisons la méthode close() de la classe FileWriter.

Exemple de code

Java
import java.io.File;
import java.io.FileWriter;
import java.io.IOException;

public class EcrireFichierTexte {

    public static void main(String[] args) throws IOException {

        // Créer un objet File pour représenter le fichier à écrire
        File fichier = new File("data.txt");

        // Ouvrir le fichier en écriture
        FileWriter ecrivain = new FileWriter(fichier);

        // Écrire le contenu dans le fichier
        ecrivain.write("Ceci est un fichier texte.");

        // Fermer le fichier
        ecrivain.close();
    }
}
Utilisez le code avec précaution. En savoir plus
