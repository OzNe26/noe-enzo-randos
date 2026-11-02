# 🏔️ Noé & Enzo — Carnet de randonnées

Carte du monde interactive avec nos randonnées : le globe tourne, on zoome sur l'Europe, la carte passe en relief 3D et chaque rando est marquée par un point rouge.

## Mettre le site en ligne avec GitHub Pages

1. Crée un compte sur https://github.com puis clique sur **New repository** (par ex. `randos`), en **Public**.
2. Clique sur **uploading an existing file**, glisse `index.html` (et ce `README.md`), puis **Commit changes**.
3. Va dans **Settings → Pages**. Dans *Source*, choisis **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis **Save**.
4. Attends environ 1 minute : le site est en ligne sur `https://TON-PSEUDO.github.io/randos/`.

## Modifier les randonnées

Tout se passe dans `index.html`, dans le bloc `const RANDOS = [ ... ]` (en haut du script) :

- **Ajouter une rando** : copie une ligne et change le nom, la région, le pays, les coordonnées (`lng`, `lat`), la distance, le D+ et l'altitude.
  Pour avoir les coordonnées : clic droit sur le lieu dans Google Maps, le premier chiffre est `lat` et le second `lng`.
- **Marquer une rando comme faite** : remplace `statut:"a-venir"` par `statut:"fait"` et le point devient vert.
- Une info inconnue ? Mets `null` et la fiche affichera « — ».

Sur GitHub tu peux modifier le fichier directement : ouvre `index.html` puis clique sur le crayon ✏️ et sur **Commit changes**.

## Crédits
Carte : MapLibre GL JS · Imagerie satellite © Esri · Relief : AWS Terrain Tiles (Mapzen) · Textures des planètes : James Hastings-Trew (Planet Pixel Emporium), via threex.planets
