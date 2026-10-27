# Récapitulatif des groupes ePack

Page autonome (un seul fichier, aucune dépendance externe) qui affiche le nombre de solutions par groupe, à partir des rapports d'intervention SharePoint (cellule D4 de l'onglet « Listing solutions »).

## Contenu

- `index.html` : la page complète (style ePackPro, thème clair/sombre, FR/EN, recherche, tri, filtres).

## Fonctionnement

- Les chiffres sont dans la constante `const DATA=[...]`, la date de relevé dans `const UPDATED="JJ/MM/AAAA"`.
- Le bloc `<script type="application/json" id="sources">` liste le chemin SharePoint de chaque classeur et la composition des totaux regroupés.
- Mise à jour : relire la valeur de chaque classeur, puis remplacer `DATA` (l'ancienne valeur passe dans `old`) et `UPDATED`.

## Publication

Ouvrir `index.html` directement, ou l'activer via GitHub Pages (Settings > Pages > branche `main`, dossier racine).

> Le fichier contient les chemins internes SharePoint et les chiffres clients : le dépôt doit rester privé.
