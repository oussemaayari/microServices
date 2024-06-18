# Gestion des Utilisateurs Microservices

Ce projet implémente un système de gestion des utilisateurs en utilisant une architecture de microservices. Chaque microservice est responsable d'une fonction spécifique de la gestion des utilisateurs, tels que l'ajout, la modification, et la supression.

## Aperçu du Projet

Ce projet vise à démontrer l'utilisation des microservices pour créer une application évolutive et maintenable pour la gestion des utilisateurs. Chaque microservice est développé de manière indépendante, ce qui facilite le déploiement, la mise à jour et l'évolutivité de l'application.

## Architecture

L'architecture du projet est basée sur plusieurs microservices interconnectés, chacun responsable d'une tâche spécifique. Les services communiquent entre eux via des API REST et utilisent un bus de messages pour la communication asynchrone.

## Services

### 1. Service d'Authentification

- Gère l'enregistrement et la connexion des utilisateurs.

## Prérequis

- Docker
- Docker Compose
- Node.js
- NVM 

## Installation

1. Clonez le dépôt:

    ```bash
    git clone https://github.com/oussemaayari/microServices.git
    ```

2. Naviguez dans le répertoire du projet:

    ```bash
    cd microServices
    ```

3. Construisez et démarrez les services Docker:

    ```bash
    docker compose up -d
    ```

## Utilisation

1. Vérifiez que les services sont en cours d'exécution:

    ```bash
    docker compose ps
    ```

2. Accédez à l'API d'authentification pour vous inscrire ou vous connecter:

    ```bash
    POST http://localhost:8000/auth/register
    POST http://localhost:8000/auth/login
    ```

3. Utilisez le token JWT pour accéder aux autres services:

    ```bash
    GET http://localhost:8000/profile
    ```

## Contribuer

Les contributions sont les bienvenues ! Veuillez suivre les étapes suivantes pour contribuer :

1. Forker le dépôt.
2. Créer une nouvelle branche (`git checkout -b feature/amazing-feature`).
3. Commiter vos changements (`git commit -m 'Add some amazing feature'`).
4. Pousser la branche (`git push origin feature/amazing-feature`).
5. Ouvrir une Pull Request.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
