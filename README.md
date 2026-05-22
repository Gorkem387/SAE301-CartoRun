# 🏃‍♂️ CartoRun — Plateforme de Gestion de Raids Sportifs

Une application web Full-Stack MVC moderne conçue pour centraliser l'organisation de raids sportifs, la gestion des clubs et le suivi des inscriptions.

---

## 🎯 Le projet en bref

CartoRun résout la complexité de l'organisation d'événements sportifs multi-courses en proposant une plateforme unifiée où interagissent plusieurs types d'acteurs (organisateurs, clubs, participants).

**Challenge relevé en équipe :**
- ✅ Architecture MVC robuste et modélisation de base de données complexe
- ✅ Système complet de gestion multi-rôles sécurisé
- ✅ Module d'importation automatisé pour les données massives
- ✅ Collaboration agile au sein d'une équipe de développement de 8 personnes

---

## 🚀 Fonctionnalités Clés

### 👥 Système Multi-Rôles & Sécurité

| Rôle | Responsabilités |
|------|----------------|
| **Administrateurs** | Supervision globale de la plateforme, validation des comptes et maintenance |
| **Responsables de Raids** | Création d'événements, configuration des courses, gestion des tracés et des difficultés |
| **Responsables de Clubs** | Gestion de leur structure, inscription groupée de coureurs et suivi administratif |
| **Coureurs** | Espace personnel, consultation des raids disponibles, inscription et accès aux résultats |

### 📊 Automatisation & Traitement de Données

- **Importation CSV automatisée :** Module d'intégration de fichiers externes pour automatiser le chargement massif de coureurs, de membres de clubs ou de grilles de résultats sans saisie manuelle.
- **Modélisation BD Relationnelle :** Base de données MySQL optimisée avec contraintes d'intégrité, indexations et clés étrangères pour garantir la fiabilité des inscriptions et éviter les doublons de courses.

### 📐 Gestion de Projet

- Développement mené en **Méthode Agile** (répartition des tâches, sprints logiciels)
- Gestion des branches Git stricte (`main`, `dev`, `stable`) avec intégration continue

---

## 🏗️ Architecture du Projet

Le projet respecte l'architecture standard de **Laravel (MVC)** pour isoler proprement la logique métier, les accès aux données et les interfaces graphiques :

```text
src/
├── app/
│   ├── Http/
│   │   ├── Controllers/   # Logique de contrôle (RaidController, InscriptionController...)
│   │   └── Middleware/    # Filtres de sécurité et gestion des rôles (Admin, ClubResponsable...)
│   └── Models/            # Modèles Eloquent (Raid, Club, Coureur, Equipe...)
├── database/
│   ├── migrations/        # Historique et structure de la base de données SQL
│   └── seeders/           # Données de test pour les démonstrations et soutenances
├── resources/
│   └── views/             # Interfaces utilisateur dynamiques (Blade, Tailwind CSS)
└── routes/
    └── web.php            # Définition des points d'accès de l'application
```

---

## 🛠️ Stack Technique

| Couche | Technologies |
|--------|-------------|
| **Back-End** | PHP — Framework Laravel 11 |
| **Front-End** | Blade Engine, Tailwind CSS, JavaScript |
| **Base de données** | MySQL / Oracle SQL |
| **DevOps** | Git, GitLab CI/CD |

---

## 📦 Installation et Lancement Local

### Prérequis

- PHP 8.2+
- Composer
- Un serveur de base de données (MySQL/SQLite)

### Démarrage rapide

```bash
# 1. Cloner le projet
git clone https://github.com/Gorkem387/CartoRun.git
cd CartoRun/laravel

# 2. Installer les dépendances Back-End
composer install

# 3. Installer les dépendances Front-End
npm install
npm run dev

# 4. Configurer l'environnement
cp .env.example .env
php artisan key:generate

# 5. Configurer votre base de données dans le fichier .env, puis lancer les migrations et les données de test
php artisan migrate --seed

# 6. Lancer le serveur local
php artisan serve
```

---

## 📚 Contexte du Projet

Projet majeur réalisé dans le cadre de la **SAE S3** (Situation d'Apprentissage et d'Évaluation) au **BUT Informatique** de l'IUT Grand Ouest Normandie — Campus 3 Ifs.

**Compétences démontrées :**
- Conception logicielle orientée objet et modélisation de données (UML / Conceptuel)
- Industrialisation et travail collaboratif à 8 développeurs sous Git
- Développement web Full-Stack sécurisé avec un framework industriel

---

## 🤝 Équipe de Développement

**Gorkem Yildiz** — Développeur Full-Stack  
Réalisé en collaboration avec 7 autres étudiants de la promotion.
