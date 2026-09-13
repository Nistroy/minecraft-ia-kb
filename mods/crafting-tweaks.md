---
slug: crafting-tweaks
nom: Crafting Tweaks
namespaces: [craftingtweaks]
version: 21.1.11+fabric-1.21.1
cote: S+C
resume: Boutons/raccourcis pour tourner, équilibrer, vider ou (dé)compresser la grille de craft
sources:
  m: https://modrinth.com/mod/crafting-tweaks
  w: https://mods.twelveiterations.com/mc/crafting-tweaks
  g: https://github.com/TwelveIterations/CraftingTweaks
  j: jar craftingtweaks-fabric-1.21.1-21.1.11.jar
  c: config serveur craftingtweaks-common.toml
verifie: 2026-09-13
---

## Mécaniques
- Ajoute dans toute interface de craft supportée : tourner la grille (sens et sens inverse), équilibrer, disperser,
  vider, forcer le vide (drop les items si besoin), compresser/décompresser 1/pile/tout, recraft du dernier craft
  (1 ou pile complète) [j].
- Activable par boutons dans l'interface et/ou raccourcis clavier, réglable (`mode`) : boutons seuls, raccourcis
  seuls, les deux (par défaut chez nous, `mode = "DEFAULT"`), ou désactivé [c].
- Clic droit sur le résultat du craft = craft une pile complète (`rightClickCraftsStack = true`) [c].
- (Dé)compression hors interface de craft (juste dans l'inventaire) possible seulement si le mod est aussi installé
  côté serveur (`compressRequiresCraftingGrid = false` sinon) — activé par défaut chez nous donc restreint à la
  grille de craft (`compressRequiresCraftingGrid = true`) [c].
- Liste noire de compression chez nous : sable + trappe de fer ne sont jamais craftés par la touche compresser
  (`compressDenylist`) [c].
- Bouton livre de recettes vanilla non caché (mode par défaut, JEI cohabite) [c].

## Ajoute
- Textes en jeu (fr_fr présent) : "Tourner la grille", "Équilibrer la grille", "Disperser sur la grille", "Vider la
  grille", "Force le vide de la grille" (+ tooltip "Drops les items si nécessaire") [j].
