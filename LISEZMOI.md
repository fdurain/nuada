# Nuada – fiche de personnage (PWA)

## Mise en ligne sur GitHub Pages
1. Créer un dépôt public, par ex. `nuada`, sur github.com/fdurain.
2. Y déposer tous les fichiers de ce dossier (index.html, manifest.webmanifest, sw.js, icônes) à la racine.
3. Settings → Pages → Source : « Deploy from a branch », branche `main`, dossier `/ (root)`.
4. L'appli est disponible après une minute sur https://fdurain.github.io/nuada/

## Installation sur le téléphone
Ouvrir l'adresse dans Chrome → menu ⋮ → « Installer l'application » (ou « Ajouter à l'écran d'accueil »).

## Données
Tout est stocké sur le téléphone. Utiliser « Exporter la sauvegarde » de temps en temps
pour garder une copie (.json), restaurable avec « Importer une sauvegarde ».

## Mise à jour
Après une modification, changer `nuada-v1` en `nuada-v2` dans sw.js pour vider l'ancien cache.
