<div align="center">

<img src="https://www.arcadia-echoes-of-power.fr/storage/img/arcadialogotransparent.webp" alt="Arcadia: Echoes Of Power" width="300"/>

# Arcadia: Echoes Of Power

**Une aventure moderne au cœur du cuivre et de la création.**  
Serveur Minecraft moddé — Technologie Create · Magie · Économie joueur

[![Joueurs inscrits](https://img.shields.io/badge/Joueurs%20inscrits-1075-blue?style=flat-square)](https://www.arcadia-echoes-of-power.fr/players)
[![Discord](https://img.shields.io/badge/Discord-Rejoindre-5865F2?style=flat-square&logo=discord&logoColor=white)](https://arcadia-echoes-of-power.fr/discord)
[![Site web](https://img.shields.io/badge/Site-arcadia--echoes--of--power.fr-green?style=flat-square)](https://www.arcadia-echoes-of-power.fr)
[![Hébergé sur OVH](https://img.shields.io/badge/Hébergé-OVH%20France-000E9C?style=flat-square)](https://www.ovhcloud.com/fr/)

</div>

---

## 🗺️ À propos

Ce dépôt contient le code source du **site web officiel** d'Arcadia: Echoes Of Power, un serveur Minecraft moddé propulsé par [Azuriom](https://azuriom.com) avec un thème personnalisé.

Le site sert de hub central pour la communauté : actualités, wiki, votes, boutique, gestion des membres et support.

---

## ✨ Fonctionnalités du site

- 📰 **Actualités** — Articles, événements, changelog et roadmap
- 🗳️ **Système de vote** — Classement mensuel avec récompenses
- 🎁 **Coffre quotidien** — Récompense journalière pour les joueurs
- 🛒 **Boutique** — Donations et avantages exclusifs via Arcadia Tokens
- 📖 **Wiki** — Documentation complète du modpack et du serveur
- 🎟️ **Giveaway** — Tirages au sort communautaires
- 👥 **Espace membres** — Profils, classements, activité en temps réel
- 💬 **Support** — Suggestions, recrutement, contact

---

## 🛠️ Stack technique

| Composant | Technologie |
|-----------|------------|
| CMS / Framework | [Azuriom](https://azuriom.com) (Laravel) |
| Thème | Arcadia par *vyrriox* |
| Hébergement | OVH — France |
| Frontend | HTML · CSS · JavaScript |

---

## 🚀 Installation locale

> Prérequis : PHP 8.1+, Composer, Node.js, une base de données (MySQL/MariaDB)

```bash
# Cloner le dépôt
git clone https://github.com/<org>/arcadia-echoes-of-power.git
cd arcadia-echoes-of-power

# Installer les dépendances PHP
composer install

# Installer les dépendances JS
npm install && npm run build

# Copier et configurer l'environnement
cp .env.example .env
php artisan key:generate

# Lancer les migrations
php artisan migrate --seed

# Démarrer le serveur de développement
php artisan serve
```

---

## 📁 Structure du projet

```
.
├── app/                # Logique métier (Laravel / Azuriom)
├── public/             # Assets publics (images, JS, CSS compilés)
├── resources/
│   ├── views/          # Templates Blade
│   └── assets/         # Sources SCSS / JS
├── routes/             # Définition des routes
├── storage/            # Uploads, logs, cache
└── themes/
    └── arcadia/        # Thème personnalisé Arcadia
```

---

## 🤝 Contribuer

Les contributions sont les bienvenues ! Pour proposer une amélioration :

1. Fork le dépôt
2. Crée une branche : `git checkout -b feature/ma-fonctionnalite`
3. Commit tes changements : `git commit -m "feat: description"`
4. Push : `git push origin feature/ma-fonctionnalite`
5. Ouvre une **Pull Request**

Pour les bugs ou suggestions, utilise les [Issues GitHub](../../issues) ou passe par le [formulaire de suggestion](https://www.arcadia-echoes-of-power.fr/suggest) du site.

---

## 📬 Contact

- 📧 Email : [contact@arcadia-echoes-of-power.fr](mailto:contact@arcadia-echoes-of-power.fr)
- 💬 Discord : [arcadia-echoes-of-power.fr/discord](https://arcadia-echoes-of-power.fr/discord)
- 🌐 Site : [arcadia-echoes-of-power.fr](https://www.arcadia-echoes-of-power.fr)

---

## 📜 Licence

Ce projet est propriétaire. Le thème Arcadia est développé par *vyrriox*.  
Le CMS Azuriom est distribué sous licence [MIT](https://github.com/Azuriom/Azuriom/blob/master/LICENSE).

© 2026 Arcadia: Echoes Of Power — Tous droits réservés.
