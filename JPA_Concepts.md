## Les 5 concepts importants de JPA

En plus des stratégies de chargement et de génération d'identifiants, JPA fournit plusieurs autres concepts importants.

**Les persister**

La méthode persist() est utilisée pour enregistrer une entité dans la base de données.

**Les flush()**

La méthode flush() est utilisée pour forcer l'enregistrement des entités persistées dans la base de données.

**Les refresh()**

La méthode refresh() est utilisée pour recharger une entité à partir de la base de données.

**Les remove()**

La méthode remove() est utilisée pour supprimer une entité de la base de données.

**Les merge()**
La méthode merge() est utilisée pour fusionner une entité avec une entité existante dans la base de données.

Le lien avec Spring Boot

Spring Boot fournit une prise en charge intégrée de JPA. Cela signifie que vous n'avez pas besoin de configurer manuellement l'unité de persistance JPA. Spring Boot le fera pour vous.

Pour utiliser JPA avec Spring Boot, vous devez ajouter la dépendance suivante à votre projet Maven :

```XML
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>

```

Utilisez le code avec précaution. En savoir plus
Une fois la dépendance ajoutée, vous pouvez commencer à utiliser JPA dans votre application Spring Boot.

Exemple

Voici un exemple simple d'utilisation de JPA avec Spring Boot :


```Java
@Entity
public class Article {

    @Id
    @GeneratedValue(strategy = GenerationType.AUTO)
    private Long id;

    private String titre;

    public Article() {
    }

    public Article(String titre) {
        this.titre = titre;
    }

    public Long getId() {
        return id;
    }

    public void setId(Long id) {
        this.id = id;
    }

    public String getTitre() {
        return titre;
    }

    public void setTitre(String titre) {
        this.titre = titre;
    }
}

```


```Java
@SpringBootApplication
public class DemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(DemoApplication.class, args);
    }

    @Autowired
    private ArticleRepository articleRepository;

    @PostConstruct
    public void saveArticle() {
        Article article = new Article("Mon premier article");
        articleRepository.save(article);
    }

    @GetMapping("/articles")
    public List<Article> getArticles() {
        return articleRepository.findAll();
    }
}

```


Ce code définit une classe Article qui est annotée avec @Entity. Cela indique à JPA que cette classe représente une entité de base de données.

Le code définit également une classe ArticleRepository qui implémente l'interface JpaRepository. Cette interface fournit une série de méthodes permettant d'interagir avec les entités JPA.

La méthode main() de la classe DemoApplication lance l'application Spring Boot.

La méthode saveArticle() enregistre un nouvel article dans la base de données.

La méthode getArticles() renvoie une liste de tous les articles de la base de données.

Conclusion

JPA est un framework puissant qui permet de simplifier le développement d'applications Java avec accès aux données. En comprenant les concepts importants de JPA, vous pouvez créer des applications Java avec accès aux données plus efficaces et plus faciles à maintenir.

## Les stratégies de chargement et la génération d'identifiants dans JPA

JPA fournit plusieurs stratégies de chargement pour les relations entre entités. Ces stratégies déterminent comment les entités liées sont chargées lorsque vous récupérez une entité.

Les stratégies de chargement

Les différentes stratégies de chargement disponibles sont les suivantes :

**EAGER :** toutes les entités liées sont chargées avec l'entité principale.

**LAZY :** les entités liées ne sont chargées que si elles sont explicitement demandées.

**JOIN :** les entités liées sont chargées en même temps que l'entité principale, mais dans une jointure SQL distincte.

**FETCH :** les entités liées sont chargées en même temps que l'entité principale, mais dans une jointure SQL avec l'entité principale.

**Justification**

Le choix de la stratégie de chargement appropriée dépend de plusieurs facteurs, notamment :

La performance : la stratégie EAGER est la plus performante, car toutes les entités liées sont chargées en même temps. La stratégie LAZY est la moins performante, car les entités liées ne sont chargées que si elles ne sont pas explicitement demandées.
La cohérence : la stratégie EAGER garantit que les entités liées sont toujours chargées, même si elles ne sont pas explicitement demandées. La stratégie LAZY ne garantit pas que les entités liées sont chargées, ce qui peut entraîner des incohérences.
La facilité d'utilisation : la stratégie EAGER est plus facile à utiliser, car vous n'avez pas à vous soucier de charger les entités liées manuellement. La stratégie LAZY peut être plus difficile à utiliser, car vous devez explicitement charger les entités liées lorsque vous en avez besoin.
Exemples

**Relation one-to-many**

Supposons que nous avons une classe Article qui a une relation one-to-many avec une classe Commentaire. La stratégie EAGER est la meilleure option dans ce cas, car elle garantit que tous les commentaires associés à un article sont chargés en même temps.


```Java
@Entity
public class Article {

    @Id
    @GeneratedValue(strategy = GenerationType.AUTO)
    private Long id;

    private String titre;

    @OneToMany(mappedBy = "article")
    @Fetch(FetchMode.EAGER)
    private List<Commentaire> commentaires;
}
```

Code


```Java
// Récupération d'un article
Article article = em.find(Article.class, 1L);

// Affichage des commentaires
for (Commentaire commentaire : article.getCommentaires()) {
    System.out.println(commentaire.getContenu());
}

```
**Relation many-to-one**

Supposons que nous avons une classe Client qui a une relation many-to-one avec une classe Commande. La stratégie LAZY est la meilleure option dans ce cas, car elle ne charge les commandes que si elles sont explicitement demandées.


```Java
@Entity
public class Client {

    @Id
    @GeneratedValue(strategy = GenerationType.AUTO)
    private Long id;

    private String nom;

    @OneToMany(mappedBy = "client")
    @Fetch(FetchMode.LAZY)
    private List<Commande> commandes;
}

```




```Java
// Récupération d'un client
Client client = em.find(Client.class, 1L);

// Affichage des commandes
for (Commande commande : client.getCommandes()) {
    System.out.println(commande.getDate());
}

```

**Conclusion**

Le choix de la stratégie de chargement appropriée dans JPA est important pour garantir les meilleures performances et la cohérence de votre application. Il est important de peser les différents facteurs impliqués avant de prendre une décision.

##  Annotation  @GeneratedValue

L'annotation @GeneratedValue est utilisée pour spécifier comment l'identifiant d'une entité est généré. La stratégie GenerationType détermine la méthode utilisée pour générer la valeur de l'identifiant.

Les différentes stratégies disponibles sont les suivantes :

GenerationType.AUTO : la valeur de l'identifiant est générée automatiquement par la base de données. Cette stratégie est la
