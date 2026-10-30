# Profil GitHub d'Elior (`eliorpom-cmd/eliorpom-cmd`)

Le `README.md` de ce dépôt s'affiche sur https://github.com/eliorpom-cmd. Tout changement doit être poussé pour être visible : Elior demande les modifs du profil pour qu'elles soient en ligne, on pousse directement (pas de déploiement derrière).

## Structure
- En anglais. Bloc `whoami` / `ls ~/now`, texte de présentation, pastilles de techno (`assets/pill-*.svg`), puis tableaux **Shipped** et **In progress**, **Also**, **Elsewhere**, bouton Ko-fi.
- `variants/` : brouillons des 4 directions de départ (A éditorial, B terminal, C vitrine, D mélange) ; le README actuel vient de D.

## Lignes de projet (décisions d'Elior, 10/10/2026)
- Une ligne de tableau par projet : icône 56 × 44 (`assets/<projet>.png` 112 × 88, ou SVG 52 × 40 avec un carré arrondi de 40 px à gauche, comme `print-on-my-desk.svg` et `gresil.svg`), **titre en gras**, `<br>`, une ou deux phrases.
- Le **titre** mène au site du projet, sinon à son dépôt. Pas de lien si rien de public (Arsène).
- À droite du titre, petites icônes grises 14 px (`#8b949e`, lisible en clair et en sombre) : `assets/source.svg` (logo GitHub → dépôt) **seulement si le dépôt est public**, `assets/app-store.svg` (→ fiche App Store). Pas d'icône site web (le titre fait ce travail) ; ne pas écrire « open source » dans le texte.
- Ordre de Shipped : Freepark, To Be Downloaded, Radiance Wallpapers, GRESIL, noaislop.xyz, Print on my desk (titre → printomatic.byelior.dev), claude-bounce.
- Dépôts publics au 10/10/2026 : accurate-meteo, to-be-downloaded, noaislop.xyz, print-on-my-desk, claude-bounce (+ cronica, bento.cat, obsidian-library-linker, non listés). Freepark, Radiance : pas de dépôt public. Arsène : dépôt repassé en privé le 30/10/2026 ; reste dans Shipped sans lien (choix d'Elior).

## Vérifier le rendu avant de pousser
`gh api -X POST /markdown -f text="$(cat README.md)" -f mode=gfm` puis capture en clair et en sombre (fond `#0d1117`) : une icône mal dessinée se voit tout de suite (la première icône App Store ressemblait à une croix).

## État
- 10/10/2026 : GRESIL ajouté (4e), titres cliquables + icônes source / App Store. Phrase de GRESIL (choix d'Elior : commencer par ce que c'est) : « A weather model built for Grenoble, more accurate there than the 16 leading models it combines. » — identique sur byelior.dev (`src/data/projects.ts`). Icône `assets/gresil.svg` = trame de points bleue (icône du site météo, `Accurate Meteo/prive/concepts/favicon/v5/t5-grosse-trame.svg`). Rien en attente.
- 22/10/2026 : alignement sur byelior.dev (voir `../byelior.dev/CLAUDE.md`, « Projets affichés ») : GRESIL « for your city » + lien Train it, Arsène = extension Chrome, Fovea remplacé par « Hand-drawn QR codes » (sans nom : secret jusqu'au lancement), `ls ~/now` = `arsene/ drawn-qr/ radiance/ client-sites/`. Poussé.
- 23/10/2026 : Macfin ajouté dans Shipped après Arsène (`assets/macfin.png`, icône de l'app arrondie, rayon 20/88). Poussé une fois le dépôt public.
- 23/10/2026 : Lumac ajouté dans Shipped après Macfin (`assets/lumac.png`, icône à plat + liseré blanc 22 % pour rester visible sur le fond sombre). Phrase : « A menu bar app that puts a MacBook to sleep when its lid is closed with an external display connected. » Poussé.
- 23/10/2026 : `ls ~/now` = `drawn-qr/ gresil/ tbd-1.2/ radiance/` (Elior : marketing et extension de GRESIL, version 1.2 de To Be Downloaded ; Arsène sorti, aucun commit client en 2 semaines, grnbl exclu = hackathon). Poussé.
