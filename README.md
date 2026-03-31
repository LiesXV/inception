# 🚀 Inception - 42

![42 Badge](https://img.shields.io/badge/42-Inception-blue)
![Unix Badge](https://img.shields.io/badge/Unix-Compatible-brightgreen)
![GitHub last commit](https://img.shields.io/github/last-commit/seyhalxv/inception)
![GitHub top language](https://img.shields.io/github/languages/top/seyhalxv/inception)

## 📖 Présentation

**Inception** est un projet de l’école 42 visant à te faire **maîtriser Docker et la conteneurisation**.  
Le but est de construire un environnement complet avec plusieurs services conteneurisés, en utilisant :

- **Dockerfiles** pour créer des images personnalisées.
- **Docker Compose** pour orchestrer plusieurs containers.
- Gestion des **volumes** et **réseaux** pour que les services communiquent correctement.
- Installation et configuration d’un **stack web complet** (WordPress + MySQL ou équivalent).

---

## 📌 Contraintes
- Chaque service doit avoir **sa propre image** et container.
- Respect strict des bonnes pratiques Docker (pas de root inutile, ports exposés correctement, données persistantes…).
- Le projet doit pouvoir être **recréé facilement** avec docker-compose up.
- Les logs doivent être consultables et clairs.

---

## 📁 Structure du projet

```bash
inception/
├── srcs/
│   ├── docker-compose.yml
│   ├── requirements/
│   │   ├── nginx/
│   │   │   ├── Dockerfile
│   │   │   ├── conf/
│   │   │   └── tools/
│   │   ├── mariadb/
│   │   │   ├── Dockerfile
│   │   │   ├── conf/
│   │   │   └── tools/
│   │   ├── wordpress/
│   │   │   ├── Dockerfile
│   │   │   ├── conf/
│   │   │   └── tools/
│   │   └── ...
├── Makefile
├── .env
└── README.md

