
## TP sur l'E/S en Java

**Objectifs**

Comprendre les concepts de base de l'E/S en Java
Savoir lire et écrire des fichiers texte
Savoir lire et écrire des fichiers binaires

### Exercice 1 : Lecture d'un fichier texte

Écrivez un programme Java qui lit le contenu d'un fichier texte et l'affiche sur la console.

**Explications**

Pour lire un fichier texte en Java, nous utilisons la classe FileReader. Cette classe fournit des méthodes pour lire les données d'un fichier texte caractère par caractère.

Pour ouvrir un fichier texte, nous utilisons la méthode open() de la classe FileReader. Cette méthode prend en paramètre un objet File qui représente le fichier à ouvrir.

Une fois le fichier ouvert, nous pouvons utiliser la méthode read() pour lire le prochain caractère du fichier. La méthode read() renvoie un entier représentant le caractère lu. Si le caractère est la fin de fichier, la méthode read() renvoie -1.

Pour fermer le fichier, nous utilisons la méthode close() de la classe FileReader.

Exemple de code

```Java
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
```

### Exercice 2 : Écriture d'un fichier texte

Écrivez un programme Java qui écrit le contenu d'une chaîne de caractères dans un fichier texte.

Explications

Pour écrire un fichier texte en Java, nous utilisons la classe FileWriter. Cette classe fournit des méthodes pour écrire les données d'un fichier texte caractère par caractère.

Pour ouvrir un fichier texte, nous utilisons la méthode open() de la classe FileWriter. Cette méthode prend en paramètre un objet File qui représente le fichier à ouvrir.

Une fois le fichier ouvert, nous pouvons utiliser la méthode write() pour écrire le prochain caractère dans le fichier. La méthode write() prend en paramètre un entier représentant le caractère à écrire.

Pour fermer le fichier, nous utilisons la méthode close() de la classe FileWriter.

Exemple de code

```Java
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
```

### Exercice 3 : Lecture d'un fichier binaire

Explications

Pour lire un fichier binaire en Java, nous utilisons la classe DataInputStream. Cette classe fournit des méthodes pour lire les données d'un fichier binaire octet par octet.

Pour ouvrir un fichier binaire, nous utilisons la méthode open() de la classe DataInputStream. Cette méthode prend en paramètre un objet File qui représente le fichier à ouvrir.

Une fois le fichier ouvert, nous pouvons utiliser les méthodes read(), readInt(), readDouble(), etc. pour lire les données du fichier.

Pour fermer le fichier, nous utilisons la méthode close() de la classe DataInputStream.

Cas d'usages

La lecture de fichiers binaires est utile dans de nombreux cas, notamment :

La lecture de fichiers d'images, de fichiers audio ou de fichiers vidéo.
La lecture de fichiers de données, tels que des fichiers CSV ou des fichiers JSON.
La lecture de fichiers de configuration.
Exemples de code

Voici quelques exemples de code pour lire un fichier binaire :

**Lecture d'un entier**

```Java
import java.io.File;
import java.io.DataInputStream;
import java.io.IOException;

public class LireFichierBinaire {

    public static void main(String[] args) throws IOException {

        // Créer un objet File pour représenter le fichier à lire
        File fichier = new File("data.bin");

        // Ouvrir le fichier en lecture
        DataInputStream lecteur = new DataInputStream(new FileInputStream(fichier));

        // Lire l'entier
        int entier = lecteur.readInt();

        // Fermer le fichier
        lecteur.close();

        // Afficher l'entier
        System.out.println(entier);
    }
}
```

Lecture d'une chaîne de caractères

```Java
import java.io.File;
import java.io.DataInputStream;
import java.io.IOException;

public class LireFichierBinaire {

    public static void main(String[] args) throws IOException {

        // Créer un objet File pour représenter le fichier à lire
        File fichier = new File("data.bin");

        // Ouvrir le fichier en lecture
        DataInputStream lecteur = new DataInputStream(new FileInputStream(fichier));

        // Lire la chaîne de caractères
        String chaine = lecteur.readUTF();

        // Fermer le fichier
        lecteur.close();

        // Afficher la chaîne de caractères
        System.out.println(chaine);
    }
}
```

**Lecture d'un tableau d'entiers**

```Java
import java.io.File;
import java.io.DataInputStream;
import java.io.IOException;

public class LireFichierBinaire {

    public static void main(String[] args) throws IOException {

        // Créer un objet File pour représenter le fichier à lire
        File fichier = new File("data.bin");

        // Ouvrir le fichier en lecture
        DataInputStream lecteur = new DataInputStream(new FileInputStream(fichier));

        // Lire le tableau d'entiers
        int[] entiers = new int[lecteur.readInt()];
        for (int i = 0; i < entiers.length; i++) {
            entiers[i] = lecteur.readInt();
        }

        // Fermer le fichier
        lecteur.close();

        // Afficher le tableau d'entiers
        for (int entier : entiers) {
            System.out.println(entier);
        }
    }
}
```

**Conclusion**

La lecture de fichiers binaires est une opération courante en Java. La classe DataInputStream fournit une API simple et efficace pour lire les données d'un fichier binaire.
Utilisez le code avec précaution. En savoir plus
