# Km-food
application de commande de restaurant
`Projet réalisez par les étudiants KONA MBOG ERIC DACIER et Lionel NGUEPI DOUNTSOP`

## Explication du projet

Pour notre projet, nous avons choisis de créer une application web TypeScript à pile complète permettant de passer des commandes dans un restaurant avec une API backend simple Nest.js un frontend en ANGULAR(pas react car nous avons deja fait un projet en react et surtout parceque  Nest.js est fortement inspiré par Angular).
cette application est une application simple pour les restaurants où les utilisateurs pourront commander des articles en ligne. Il existe des règles commerciales pour cette application :

tout utilisateur peut voir les éléments de ce menu ;
seuls les utilisateurs identifiés peuvent ajouter des articles à un panier (commander de la nourriture en ligne) ;
et seuls les utilisateurs administrateurs peuvent ajouter de nouveaux éléments au menu.

`La gestion des identités est géré sur la plateforme Auth0,car nous avons rencontré des difficultés avec mongoose et Auth0 nous apporte aussi une belle couche de sécurité. pour simplifier les chose, nous admettons en tant qu'utilisateur/administrateur tous les utilisateurs ayant le nom de domain gmail.com dans son adresse email`

Pour simplifier les choses, nous n'allons pas interagir avec une base de données externe, ni implémenter la fonctionnalité de panier d'achat.

## Comment executer le projet

cd nest-restaurant-backend
`npm run start:dev`

cd angular-restaurant-frontend
`ng serve --open`

## intégration Angular avec Nest.JS
Afin d'interagir avec le service backend, nous avons traiter avec CORS (Cross Request Origin Sharing)
enfin executer 
`ng serve --proxy-config proxy.config.js --open`
Et dirigez-vous vers votre application  `localhost:4200`
