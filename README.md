## Introduction

_Avant de commencer, je voulais juste préciser que j'avais dans un premier temps fais ce tutoriel dans un principe d'imitation pur et dur. J'ai trouvé les instructions initiales claires et bien structurées pour commencer. Cependant, j'ai été un peu dérouté par la terminologie spécifique d'Angular, notamment la notion de modules et de composants._

_L'ayant fait en anglais, plusieurs notions étaient compliquées à comprendre pour moi._

_Après ma semaine d'entreprise, j'ai décidé de tout recommencer pour pouvoir faire ce read me et espérer comprendre un peu mieux._

## Partie 1 : Initiation

>Cette partie du tutoriel est une introduction à Angular Elle couvre les bases fondamentales, y compris l'installation d'Angular CLI, la création d'un projet, et l'explication des composants, des modèles et des >services. L'accent est mis sur la structure d'un projet Angular et la compréhension de l'architecture de base.

>Nous avons donc appris dans un premier temps à ajouté les bouttons "Share" et "Notify Me" ainsi qu'à leur associé les alertes correspondantes soit "The product has been shared!" et "You will be notified when the >product goes on sale" lorsque l'utilisateur clique sur celui-ci. Pour générer les alertes nous avons dû faire la commande :
>```ts
>ng generate component product-alerts
>```
>qui nous a permis de créer les fichiers suivants :
>
>* product-alerts.component.ts
>* product-alerts.component.html
>* product-alerts.component.css

>l'utilisation de StackBlitz comme environnement de développement en ligne n'étant pour notre cas pas possible, nous sommes passé sur VSCode qui a été à l'inverse très pratique sauf dans le cas du "Simple >Browser" car en entrant l'URL de notre application était bien présent mais par contre ça ne mettait pas les alertes "Focus lock" ce que j'ai trouvé dommage, mais un p'tit coup d'oeil sur le navigateur et on est >vite rassuré.

## Partie 2 : Routing

>La partie sur le routage d'Angular explique comment ajouter la navigation à une application. Elle montre comment créer des routes pour différentes vues, comment associer des URL à des composants spécifiques, et >comment utiliser le RouterLink pour naviguer à l'intérieur d'une application à une seule page. Elle enseigne également comment afficher des détails de produits uniques à l'aide des routes et du Router.

>Dans cette seconde partie, nous avons commencer par générer un nouveau composant pour le détail des produits à l'aide de la commande : 
>```ts
>ng generate component product-details
>```
>afin de nous permettre de naviguer d'une page à l'autre, dans cet exemple, cliquer sur un téléphone nous permetgtait d'aller sur une deuxième page qui nous affichait la fiche du produit.

>Comprendre comment configurer les routes et naviguer entre les pages était un peu difficile au début, j'ai eu du mal à assimiler pleinement comment les paramètres de l'URL étaient transmis aux composants pour >afficher des données spécifiques. Les exemples fournis étaient utiles, mais j'aurais aimé plus de détails sur les interactions entre les composants et les routes.

## Partie 3 : Data

>La gestion des données dans Angular est abordée dans cette partie. Elle inclut la création d'un service de panier, permettant aux utilisateurs d'ajouter des produits à un panier et de visualiser son contenu. >Elle explique comment utiliser HttpClient pour récupérer des données d'un fichier externe (shipping.json), afficher les articles du panier, et obtenir des prix de livraison.

>Pour cette troisième partie, nous avons dû générer une carte en écrivant ce code : 
>```ts
>ng generate service cart
>```
>cela nous a permis en suivant étape par étape, de créer un bouton "Buy" avec le message "Your product has been added to the cart!" une fois cliqué dessus, afin d'ajouter le produit. Ensuite, nous avons créé le >composant carte grâce à cette ligne de commande : 
>```ts
>ng generate component cart
>```
>qui nous permettra d'avoir un panier dans lequel se trouveront les produits que l'utilisateur aura choisi d'acheter. Nous avons enfin généré un composant livraison par la commande suivante : 
>```ts
>ng generate component shipping
>```
>afin de rajouter la possibilité de consulter les différents types de livraison accessible depuis le panier.

>La création du service de panier et son utilisation pour ajouter des articles étaient relativement simples à comprendre. Cependant, lorsque le tutoriel est passé à l'utilisation d'HttpClient pour récupérer les >données de livraison, j'ai été un peu perdu. La connexion entre le service, la récupération des données et leur affichage dans le composant ShippingComponent n'était pas évidente pour moi.

## Partie 4 : Formulaire

>La dernière partie du tutoriel explique comment utiliser les formulaires dans Angular pour collecter des informations des utilisateurs lors du processus de paiement. Elle montre comment configurer un formulaire >de paiement basique avec FormBuilder pour récupérer le nom et l'adresse de l'utilisateur. Elle explique également comment gérer la soumission du formulaire pour finaliser un achat et vider le panier.

>Dans cette dernière partie, nous avons appris comment créer un formulaire afin que l'utilisateur puisse renseigner son nom et son adresse une fois sa commande prête à passer au paiement.

>La création du formulaire avec FormBuilder était relativement simple à saisir, mais j'ai eu du mal à comprendre comment lier chaque champ du formulaire avec les contrôles du formulaire dans le composant. La >manipulation des données du formulaire lors de la soumission était bien expliquée, mais j'ai ressenti le besoin de plus d'exemples concrets pour saisir pleinement les concepts.

## Conclusion

_J'ai apprécié la simplicité et la clarté du tutoriel, mais j'aimerais davantage d'explications approfondies et d'exemples détaillés pour mieux comprendre les concepts plus complexes d'Angular. Des explications pas à pas avec des exemples plus détaillés pourraient aider à mieux visualiser comment les différentes parties d'Angular interagissent entre elles. Il m'a fallu un certain temps pour comprendre comment ces éléments s'imbriquent et interagissent entre eux. J'ai hâte d'en découvrir plus !_
