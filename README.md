# DailyNews

Un lecteur de flux RSS pour suivre en un seul endroit les actualités de ses sources préférées. Application Vue.js : on enregistre ses flux, on les parcourt et on lit chaque article.

## Fonctionnalités

- Ajouter un flux RSS (titre et adresse)
- Liste de ses flux, avec suppression
- Parcourir les articles d'un flux, puis ouvrir le détail d'un article
- Préférences enregistrées : flux favoris mémorisés d'une visite à l'autre
- Données conservées dans le navigateur (`localStorage`), sans compte à créer
- Page dédiée pour les adresses introuvables

## Technologies

- Vue 3
- Vue Router 4
- Vite 6
- Analyse des flux XML avec le `DOMParser` du navigateur

## Pages

| Adresse | Contenu |
|---|---|
| `/` | liste des flux |
| `/add` | formulaire d'ajout d'un flux |
| `/preferences` | préférences enregistrées |
| `/news/:Index` | articles d'un flux |
| `/news/:Index/:newsIndex` | détail d'un article |

## Lancer le projet

Prérequis : Node.js 18 ou plus récent.

```bash
git clone https://github.com/imene-be/dailynews-rss.git
cd dailynews-rss
npm install
npm run dev
```

L'application est disponible sur [http://localhost:5173](http://localhost:5173).

Certains flux refusent les requêtes faites directement depuis un navigateur (règle CORS) : si un flux ne se charge pas, essayez-en un autre.

---

Développé par [Imène Bentifraouine](https://imenebe.fr) et Nassim Bentifraouine.
