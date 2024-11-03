---

# Next Event - Gestion d'Événements

**Next Event** est une application Django destinée à la gestion d'événements. Ce projet vise à simplifier l'organisation, la gestion des contributeurs, et le suivi des événements en temps réel, en utilisant Django et des événements asynchrones pour une expérience utilisateur fluide. 
Ce projet est à but de formation et n'a pas d'objectif commercial.

## Fonctionnalités

- **Création et Gestion d'Événements** : Créez des événements, avec des informations détaillées (date, lieu, description, etc.).
- **Gestion des Contributeurs** : Ajoutez, mettez à jour, et supprimez des contributeurs pour chaque événement grâce à une logique asynchrone.
- **Notifications en Temps Réel** : Utilise des événements asynchrones pour notifier les contributeurs des mises à jour importantes.
- **Tests Unitaires** : Des tests unitaires robustes pour garantir la stabilité des fonctionnalités CRUD des contributeurs et des événements.

## Installation

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/lebequin/nextEvent.git
   ```
2. Accédez au répertoire :
   ```bash
   cd nextEvent
   ```
3. Installez les dépendances :
   ```bash
   pip install -r requirements.txt
   ```
4. Appliquez les migrations de la base de données :
   ```bash
   python manage.py migrate
   ```
5. Lancez le serveur :
   ```bash
   python manage.py runserver
   ```

## Configuration

Assurez-vous de configurer les variables d'environnement (comme `DATABASE_URL`, `SECRET_KEY`, etc.) dans votre fichier `.env`.

## Structure du Projet

- `events/` : Contient les modèles, vues et gestionnaires pour les événements.
- `contributors/` : Gère la logique des contributeurs, incluant les événements asynchrones pour les notifications en temps réel.
- `tests/` : Regroupe les tests unitaires pour les fonctionnalités de l'application.
- `settings.py` : Configuration du projet, incluant les réglages pour l'ORM asynchrone et la gestion des événements.

## Utilisation

Pour créer et gérer des événements, accédez à l'interface admin Django (disponible par défaut à `/admin`). Vous pouvez y ajouter des contributeurs, visualiser les événements, et gérer l’ensemble du flux d'organisation.

## Contributions

Les contributions sont les bienvenues ! Veuillez ouvrir une **issue** pour signaler les bugs ou proposer de nouvelles fonctionnalités. Avant de soumettre une pull request, assurez-vous que votre code respecte les normes de style et est bien documenté.

## Licence

Ce projet est sous licence MIT. Veuillez consulter le fichier [LICENSE](LICENSE) pour plus de détails.

## Contact

Pour toute question ou demande d’assistance, contactez-nous via le chat sur la plateforme [Dyma](https://dyma.fr)
