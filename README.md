# 🐝 QueenBee — Frontend web

Application web de QueenBee pour les coordinateurs régionaux, les gestionnaires de l'association et les administrateurs : tableau de bord des sites, carte des ruches, visites, récoltes, alertes et supervision DevOps.

Fait partie de la plateforme **QueenBee**, qui aide les coopératives apicoles d'Afrique de l'Ouest et centrale à suivre 400 ruches connectées sur 8 sites, même sans réseau.

| Dépôt | Contenu |
|---|---|
| [queenbee-backend](https://github.com/lahatraR/queenbee-backend) | API Spring Boot, base PostgreSQL/PostGIS, simulateur, infrastructure et déploiement |
| [queenbee-frontend](https://github.com/lahatraR/queenbee-frontend) | Application web Angular |
| [queenbee-mobile](https://github.com/lahatraR/queenbee-mobile) | Application mobile Flutter hors ligne |

📋 Backlog : [Trello QueenBee — Dev & DevOps](https://trello.com/b/lfFjpVWK)

## Stack

- Angular, TypeScript
- Leaflet / OpenStreetMap pour la carte
- Client d'API généré depuis le contrat OpenAPI de `queenbee-backend`

## Structure

```
queenbee-frontend/
├── src/                 # Code Angular (créé par QB-009)
├── docs/
│   └── adr/             # Choix techniques propres au web
└── .github/workflows/   # CI, sécurité, conventions de PR, release
```

## Démarrer en local

> À compléter par la carte QB-009. L'objectif : cloner, puis lancer le projet en une ou deux commandes.

```bash
git clone https://github.com/lahatraR/queenbee-frontend.git
cd queenbee-frontend
git switch develop
npm ci
npm start
```

## Branches et environnements

| Branche | Environnement | Déploiement |
|---|---|---|
| `main` | Production | À chaque tag `vX.Y.Z` |
| `preprod` | Préproduction (recette) | À chaque merge |
| `develop` | Développement (intégration) | À chaque merge |

Tout changement passe par une Pull Request relue et une CI verte. Les règles complètes sont dans **[CONTRIBUTING.md](CONTRIBUTING.md)** : à lire avant ta première PR.

## Équipe

Clément · Brice · Aimé-Césaire · Riantsoa — Master 1, INGETIS / ITIS, projet fil rouge 2026-2027.

## Licence

Code publié pour consultation uniquement, tous droits réservés : voir [LICENSE](LICENSE).
