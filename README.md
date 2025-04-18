# AniTrack

AniTrack est une application Fullstack qui permet aux utilisateurs de suivre leur progression dans leurs **animes et mangas préférés**, de **laisser des avis**, de **noter les œuvres**, et de **découvrir des recommandations personnalisées**.

> Tech stack : React, FastAPI, SQLModel, Supabase, Anilist API

---

## Fonctionnalités

### Côté utilisateur

- Authentification (Inscription, Connexion, Déconnexion)
- Page d’accueil avec recommandations personnalisées
- Recherche d’œuvres par titre, genre, type, etc.
- Fiche détaillée d’une œuvre (synopsis, genres, note, progression)
- Suivi de progression par œuvre
- Notation & avis utilisateurs (en cours)
- Recommandations basées sur les goûts

### Côté technique

- Backend en FastAPI + SQLModel avec PostgreSQL (via Supabase)
- Appels à l’API GraphQL de Anilist
- Frontend React
- Gestion d’état via hooks personnalisés (`useFetch`, `useAuthFetch`)
- Token JWT pour l’auth (stocké en `localStorage`)

---

## Aperçu UI

| Accueil (recommandations)          | Recherche d'œuvres                     |
| ---------------------------------- | -------------------------------------- |
| ![Home](./src/assets/homePage.png) | ![Search](./src/assets/SearchPage.png) |

| Détail d'une œuvre                     |
| -------------------------------------- |
| ![Detail](./src/assets/detailPage.png) |

---

## Installation

### Backend

```bash
cd back
pip install -r requirements.txt
uvicorn main:app --reload
```
