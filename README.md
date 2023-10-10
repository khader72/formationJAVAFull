# Formation JAVA Web

Formation  JAVA  Full

## JavaDoc

* https://docs.oracle.com/en/java/javase/11/docs/api/
  
##  TOP  Sites WebS

* https://www.geeksforgeeks.org/introduction-to-java/


## TOP Autoformation

- https://www.sololearn.com/

- https://ide.geeksforgeeks.org/online-java-compiler

- 

## Les Outils JAVA JEE

- JDK  JAVA 11
- Maven
- ECLIPSE IDE
- VS CODE


## IDE JAVA en Ligne /Web


## JAVA Web  Spring Boot


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

 ** Pour changer le port sur lequel le serveur local fonctionne avec http-server**, 
 
 vous pouvez spécifier le port lors du démarrage du serveur en utilisant l'option -p ou --port. Voici comment vous pouvez faire cela :


```bash

http-server -p 9090  --cors
```

Dans cet exemple, le serveur local sera démarré sur le port 9090. Vous pouvez remplacer 9090 par n'importe quel numéro de port de votre choix. Assurez-vous simplement de ne pas utiliser un port qui est déjà utilisé par un autre service sur votre système.

