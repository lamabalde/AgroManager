# AgroManager
# 🌱 AgroManager API

**Système de gestion d'une organisation de producteurs agricoles au Sénégal.**

AgroManager est une API REST développée avec Django et Django REST Framework. Elle permet de digitaliser la gestion des coopératives agricoles, des producteurs, des produits et des activités de production.

L'objectif est de proposer une solution centralisée, sécurisée et évolutive pour faciliter le suivi des activités agricoles.

## 🚀 Objectifs du projet

- Digitaliser la gestion des organisations agricoles.
- Centraliser les informations des producteurs.
- Gérer les produits agricoles.
- Suivre les productions et les récoltes.
- Fournir des statistiques sur les activités agricoles.
- Sécuriser l'accès aux données.

## 🛠️ Technologies

| Technologie | Utilisation |
|---|---|
| Python | Langage principal |
| Django | Framework backend |
| Django REST Framework | API REST |
| PostgreSQL | Base de données |
| JWT | Authentification |
| Docker | Conteneurisation |
| Git / GitHub | Gestion du code |

## 📁 Architecture du projet

```text
agromanager/
│
├── config/
│   ├── settings.py
│   ├── urls.py
│   └── asgi.py
│
├── organizations/
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│   └── admin.py
│
├── producers/
├── products/
├── productions/
│
├── manage.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## ⚙️ Installation

### 1. Cloner le projet

```bash
git clone <URL_DU_DEPOT>
cd agromanager
```

### 2. Créer un environnement virtuel

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Installer les dépendances

```bash
pip install -r requirements.txt
```

### 4. Configurer les variables d'environnement

Créer un fichier `.env` :

```env
SECRET_KEY=your-secret-key
DEBUG=True

DB_NAME=agromanager
DB_USER=postgres
DB_PASSWORD=your-password
DB_HOST=localhost
DB_PORT=5432
```

### 5. Appliquer les migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Créer un administrateur

```bash
python manage.py createsuperuser
```

### 7. Lancer le serveur

```bash
python manage.py runserver
```

API disponible sur :

```text
http://127.0.0.1:8000/
```

## 📦 Modules fonctionnels

### Organizations
- Création d'organisations.
- Modification des informations.
- Gestion des coopératives.

### Producers
- Enregistrement des producteurs.
- Gestion des profils.
- Association aux organisations.

### Products
- Gestion des produits agricoles.
- Catégorisation des produits.
- Suivi des informations commerciales.

### Productions
- Enregistrement des récoltes.
- Suivi des quantités produites.
- Statistiques de production.

## 🔐 Sécurité

Les fonctionnalités prévues comprennent :

- Authentification JWT.
- Gestion des permissions.
- Validation des données.
- Protection des endpoints.
- Gestion des rôles utilisateurs.
- Configuration sécurisée des variables d'environnement.

## 🧪 Tests

Les tests automatisés seront exécutés avec :

```bash
python manage.py test
```

## 🗺️ Roadmap

- [x] Initialisation du projet Django.
- [x] Création des applications.
- [ ] Conception des modèles de données.
- [ ] Développement des serializers.
- [ ] Développement des API Views et ViewSets.
- [ ] Authentification JWT.
- [ ] Permissions et gestion des rôles.
- [ ] Recherche, filtrage et pagination.
- [ ] Statistiques et tableaux de bord.
- [ ] Tests automatisés.
- [ ] Dockerisation.
- [ ] Déploiement en production.

## 👨‍💻 Auteur

**Mamadou Lamarana Balde**

Développeur Full Stack | Backend Engineering | DevSecOps

---

*AgroManager API — Digitaliser et moderniser la gestion agricole.*