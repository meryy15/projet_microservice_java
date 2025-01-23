Microservice Commandes & Produits
Description du projet
Ce projet consiste en la création de deux microservices :

Microservice Commandes : Permet de gérer les commandes via des opérations CRUD.
Microservice Produits : Fournit des informations sur les produits.
Le projet utilise Spring Cloud pour la configuration centralisée et Eureka pour l'enregistrement des services.

Fonctionnalités
Étude de cas 1
Gestion des commandes avec une structure simple [id, description, quantité, date, montant].
Propriété personnalisée pour afficher les commandes des derniers jours via Spring Cloud Config.
Supervision de la santé du service via Actuator.
Étude de cas 2
Gestion avancée des commandes avec une relation produit [id, description, quantité, date, montant, id_produit].
Enregistrement des microservices dans Eureka.
Implémentation d'une API Gateway pour centraliser les appels.
Résilience des services via Hystrix en cas de timeout.
Architecture
L'application est composée des modules suivants :

API Gateway : Point d'entrée unique pour les microservices.
Eureka Server : Service de registre des microservices.
Config Server : Centralisation des configurations.
Microservice Commandes : Gestion des commandes.
Microservice Produits : Gestion des produits.
Prérequis
Java 17
Maven 3.8+
Git
Postman (pour les tests)
Docker (facultatif, pour les bases de données ou la conteneurisation)
