## Visitez le site : https://mika-exercice-random-ideas.netlify.app/ 
Le premier appel au serveur est un peu long car Heroku met le serveur en stand-by au bout d'un certain moment sur la version gratuite.
La partie client est hébergée sur Netlify.

# Consignes de l'exercice : 
# ------------------------

## Le projet est en deux parties et consiste à monter une mini boîte à idées.

### Backend

Créer un projet NodeJS avec une seule route "/api/ideas" qui renvoie un tableau d'idées aléatoires (entre 10 et 50). 
Pas de base de données. 

Une idée est un objet avec ces caractéristiques:
- id: int
- title: string
- createdAt: datetime
- author: string
- score: int (positive)

Les contraintes sont les suivantes:
- renvoyer un tableau en JSON
- utiliser Faker (https://github.com/Marak/faker.js) pour les données.
- les dates doivent être aléatoire dans les 6 derniers mois
- les ids se suivent et sont uniques
- le score est compris entre 0 et 50

### Frontend

Créer un projet React avec https://github.com/facebook/create-react-app et récupérer les idées depuis le point d'api NodeJS, les mettre en forme et ajouter des filtres et tris:

- tri par date (ASC et DESC) avec la fonction "sort" en javascript
- tri par score (ASC et DESC) avec la fonction "sort" en javascript
- filtre par titre avec la fonction "filter" en javascript: étant donné un champ de texte, je veux récupérer les idées dont le titre contient le texte inscrit. Utiliser https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/String/includes

### Les deux projets sont à rendre dans le même répertoire Github.