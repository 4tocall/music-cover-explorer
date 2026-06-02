# Music Cover Explorer

Un petit site-outil pour explorer et télécharger les pochettes (covers) d'albums et de singles par style musical, artiste ou pays. Aucune installation, aucune clé API : une seule page HTML qui interroge l'API publique iTunes Search.

## Fonctionnalités

- **Recherche libre** : artiste, titre, label ou style exact (ex. « gwo ka », « kizomba »).
- **Filtre par style** : Rap, R'n'b, Raï, Zouk, Kompa, Reggae, Dancehall, Afrobeat… ou « Tous styles ».
- **Filtre par pays** : France, Haïti, Jamaïque, Algérie, Maroc, Sénégal, Brésil… (change le catalogue iTunes) ou « Tous pays ».
- **Albums ou singles/titres**.
- **Affichage en miniatures** avec **lazy load** au scroll.
- **Téléchargement** des covers en haute résolution (~1000 px) ; clic sur une miniature pour l'ouvrir en grand.

## Utilisation

Ouvre simplement `index.html` dans un navigateur (double-clic), ou via GitHub Pages.

Astuce : les styles de niche (Kompa…) ne sont pas des genres officiels iTunes — ils fonctionnent comme mots-clés. Combine-les avec le bon pays pour de meilleurs résultats :

| Style     | Pays conseillé        |
|-----------|-----------------------|
| Kompa     | Haïti / France        |
| Zouk      | France (Antilles)     |
| Raï       | Algérie / France      |
| Dancehall | Jamaïque              |

## Limites

L'API iTunes renvoie au maximum ~200 résultats par recherche. Pour élargir, varie le mot-clé, le style ou le pays.

## Technique

HTML/CSS/JavaScript pur, sans dépendance ni build. Les requêtes utilisent JSONP, donc le site fonctionne même ouvert en `file://`.
