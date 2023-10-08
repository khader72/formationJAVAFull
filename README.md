# Formation JAVA Web

Formation  JAVA  Full

## JavaDoc

* https://docs.oracle.com/en/java/javase/11/docs/api/
  
##  TOP  Sites WebS

* https://github.com/sanogotech/java-cheat-sheet.git

## TOP Autoformation

- https://www.sololearn.com/

## Les Outils JAVA JEE

- JDK  JAVA 11
- Maven
- ECLIPSE IDE
- VS CODE

## Visualer les Ficheir  MD  Markdown

**Utilisez un Serveur Local :**

Si vous avez Node.js installé, vous pouvez utiliser le package http-server pour créer un serveur local facilement. Installez-le via npm si vous ne l'avez pas déjà fait :

```
npm install -g http-server
```

Ensuite, dans le dossier où se trouve votre fichier HTML et votre fichier Markdown, exécutez la commande suivante pour lancer le serveur local :

```
http-server
```

Le serveur sera accessible à l'adresse http://localhost:8080 par défaut.

Modifiez votre script pour faire appel au serveur local :

Modifiez le script JavaScript dans votre fichier HTML: **indexformationjava.html** pour récupérer le fichier Markdown à partir du serveur local :

```javascript

fetch('http://localhost:8080/your-markdown-file.md')
    .then(response => response.text())
    .then(markdown => {
        const markdownContent = document.getElementById('markdown-content');
        markdownContent.innerHTML = marked(markdown);
    });
```

Assurez-vous de remplacer 'your-markdown-file.md' par le chemin relatif du fichier Markdown par rapport au dossier du serveur local.

En utilisant un serveur local, vous évitez les problèmes de CORS pendant le développement local. Une fois votre application déployée sur un vrai serveur, ces problèmes ne se poseront pas.

  
## IDE JAVA en Ligne /Web


## JAVA Web  Spring Boot


