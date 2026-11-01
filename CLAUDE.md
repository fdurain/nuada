# Nuada – fiche de personnage (PWA)

PWA de fiche de personnage pour les livres-jeux de Fabien Olicard (tome 1 « La Harpe des Quatre Saisons », tome 2 « La Confrérie de Nuada »), publiée sur GitHub Pages : https://fdurain.github.io/nuada/

- Tout est dans `index.html` (HTML, CSS et JS inline) ; `sw.js` est le service worker.
- À chaque modification de l'appli, incrémenter la version du cache dans `sw.js` (`nuada-vN` → `nuada-vN+1`), sinon les téléphones gardent l'ancienne version. La version actuelle est celle de la constante `CACHE` dans `sw.js`.
- Le livre actif est stocké dans localStorage sous `ariane-livre`. Chaque tome a sa propre clé : `harpe-fiche-v1` et `nuada-fiche-v1`.
- Les données du tome 1 (renvois, énigmes à numéro calculé, combats avec leurs issues) sont dans la constante `HARPE`. Elle contient uniquement la mécanique, jamais le texte du livre.

## Règle importante : aucun spoiler du tome 1
L'utilisateur n'a pas encore lu le tome 1 : aucun spoiler, ni lieux, ni personnages, ni issues. Cela vaut pour les réponses comme pour le code, les libellés et les messages de commit.

## Après chaque modification
Commit et push sur `main`. Si Git n'a pas d'identité configurée, utiliser celle des commits existants :
`git -c user.name=fdurain -c user.email=florent.durain@aglconsult.fr commit ...`
