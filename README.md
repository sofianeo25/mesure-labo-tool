# Projet de Mesure Wi-Fi

Ce projet Django vise à centraliser et à simplifier la gestion et l'analyse des mesures Wi-Fi. Il remplace un système existant basé sur des macros Excel, offrant une interface web plus moderne, une meilleure accessibilité des données, et des fonctionnalités avancées telles que l'authentification des utilisateurs et l'intégration de Bootstrap pour un design réactif.

---

## Démarrage rapide

Suivez ces instructions pour configurer le projet sur votre machine locale à des fins de développement et de test.

### Prérequis

- Python 3.8+
- Django 3.2+
- Git

### Installation

1. **Cloner le dépôt** :

2. **Naviguer dans le dossier du projet** :

3. **Installer les dépendances** dans le repertoire wifi-label-django (dans un environnement virtuel recommandé) :

   ```bash
   python -m venv env
   source env/bin/activate  # Sur Windows, utilisez `env\Scripts\activate`
   pip install -r requirements.txt
   ```

4. **Appliquer les fixtures pour charger les données initiales** :

   Assurez-vous d'avoir lancé le serveur de développement Django et exécutez les commandes suivantes :

   ```bash
   python manage.py loaddata equipments.json
   python manage.py loaddata users.json
   python manage.py loaddata measurements.json
   ```

5. **Lancer le serveur de développement Django** :

   Effectuer les migrations :

   ```bash
   python manage.py migrate
   ```

   Lancer le serveur :

   ```bash
   python manage.py runserver
   ```

   Accédez à http://127.0.0.1:8000/ dans votre navigateur pour voir l'application en action.

## Utilisation

Après avoir lancé le serveur de développement, vous pouvez naviguer dans l'interface web pour créer, visualiser, et analyser les mesures Wi-Fi. Utilisez l'interface d'administration Django pour gérer les utilisateurs et les données de mesure de manière plus détaillée.

### Remarque
Pour créer un superutilisateur (superuser) dans Django en utilisant la commande `manage.py`, vous pouvez exécuter la commande suivante dans votre terminal ou invite de commande :

```bash
python manage.py createsuperuser
```

Cette commande va démarrer un processus interactif où vous devrez fournir les informations nécessaires pour créer le superutilisateur, y compris :

- Nom d'utilisateur (username)
- Adresse e-mail (email)
- Mot de passe (password)

Suivez simplement les instructions interactives après avoir exécuté cette commande. Une fois que vous aurez fourni toutes les informations requises, le superutilisateur sera créé et vous pourrez l'utiliser pour accéder à l'interface d'administration Django et effectuer des tâches d'administration.

## Auteurs

- **OUARDI Sofiane** - *Développement initial* 


## Remerciements

- Mounir BOTI, Patrice GALLEAU pour leurs retours et conseils.

--- 
