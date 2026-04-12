# 💄 BeautyStore — Plateforme E-Commerce Beauté 💄

<div align="center">

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![Blade](https://img.shields.io/badge/Blade-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white)
![PayPal](https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)

**Application e-commerce de produits beauté — catalogue, commandes et paiement en ligne 🛍️**

[✨ Fonctionnalités](#fonctionnalités) · [🛠️ Stack](#stack-technique) · [🚀 Installation](#installation) · [📁 Structure](#structure-du-projet) · [🗄️ Base de données](#base-de-données)

</div>

---

## 📖 Description

**Beauty Farah** est une application web e-commerce complète dédiée aux produits de beauté, développée avec **Laravel** et **Blade**. Elle offre une expérience d'achat fluide côté client — navigation dans le catalogue, gestion du panier, commandes et paiement sécurisé — ainsi qu'un espace d'administration pour gérer les produits et les commandes.

---

## ✨ Fonctionnalités

### 👤 Utilisateur
| Fonctionnalité | Description |
|---|---|
| 🔐 **Authentification** | Inscription, connexion, déconnexion, mot de passe oublié |
| 👤 **Profil** | Consultation et modification des informations personnelles |
| 🔍 **Recherche** | Recherche de produits par nom, catégorie ou marque |
| 🛍️ **Catalogue** | Navigation par catégories, filtres et tri des produits |
| 🛒 **Panier** | Ajout, modification de quantité, suppression d'articles |
| 📦 **Commandes** | Passage de commande, historique et suivi de statut |
| 💳 **Paiement** | Paiement sécurisé via Stripe ou PayPal |

### 🛠️ Administration
| Fonctionnalité | Description |
|---|---|
| 📋 **Gestion produits** | Ajout, modification, suppression et mise en ligne |
| 🗂️ **Catégories** | Création et organisation des catégories |
| 📊 **Commandes** | Consultation et mise à jour du statut des commandes |
| 👥 **Utilisateurs** | Gestion des comptes clients |

---

## 🛠️ Stack technique

```
Beauty Farah
├── ⚙️  Laravel (PHP)       → Framework backend MVC
├── 🎨 Blade               → Moteur de templates frontend
├── 🗄️  MySQL               → Base de données relationnelle
├── 💳 Stripe              → Paiement en ligne sécurisé
├── 🔐 Laravel Auth        → Authentification & autorisation
├── 📁 Laravel Storage     → Gestion des images produits
└── 🐘 Composer            → Gestion des dépendances PHP
```

## 🚀 Installation

### Prérequis

- PHP 8.1+
- Composer
- MySQL 8.0+
- Node.js & npm (pour les assets front)
- Compte [Stripe](https://stripe.com) et/ou [PayPal Developer](https://developer.paypal.com)

### Étapes

```bash
# 1. Cloner le dépôt
git clone https://github.com/farah-benhadjali/beautystore-ecommerce.git
cd beautystore-ecommerce

# 2. Installer les dépendances PHP
composer install

# 3. Installer les dépendances JS
npm install && npm run dev

# 4. Copier le fichier d'environnement
cp .env.example .env

# 5. Générer la clé d'application
php artisan key:generate

# 6. Configurer la base de données (voir section suivante)

# 7. Lancer les migrations et les seeders
php artisan migrate --seed

# 8. Créer le lien symbolique pour le stockage
php artisan storage:link

# 9. Lancer le serveur de développement
php artisan serve
```

L'application est accessible sur **http://localhost:8000**

---

## ⚙️ Configuration

Renseigner les variables suivantes dans le fichier `.env` :

```env
# Base de données
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=beauty_farah
DB_USERNAME=root
DB_PASSWORD=

# Stockage des images
FILESYSTEM_DISK=public
```

---

## 🗄️ Base de données

### Migrations & Seeders

```bash
# Créer la base de données
php artisan migrate

# Peupler avec des données de test
php artisan db:seed

# Ou tout en une commande
php artisan migrate:fresh --seed
```

---

## 🔐 Rôles & Accès

| Rôle | Accès |
|---|---|
| **Visiteur** | Catalogue, recherche, fiche produit |
| **Client** | + Panier, commandes, profil, paiement |
| **Admin** | + Gestion produits, catégories, commandes, utilisateurs |

---

## 📸 Captures d'écran

> 📸 *Captures d'écran à ajouter*

```

```

---

## 📄 Licence

Ce projet est sous licence **MIT** — voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

<div align="center">

Développé avec 💄 par [Farah Benhadjali](https://github.com/farah-benhadjali)

</div>
