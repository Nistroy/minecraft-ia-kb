---
slug: immersive-paintings
nom: Immersive Paintings
namespaces: [immersive_paintings]
version: 0.7.8+1.21.1
cote: S+C
resume: importer ses propres images comme tableaux/graffitis en jeu (taille, cadre, dither réglables)
sources:
  m: https://modrinth.com/mod/immersive-paintings
  w: https://github.com/Luke100000/ImmersivePaintings/wiki
  g: https://github.com/Luke100000/ImmersivePaintings
  j: jar immersive_paintings-fabric-1.21.1-0.7.8.jar
  c: config serveur immersive_paintings/common_config.toml + client_config.toml
verifie: 2026-09-13
---

## Ajoute
- Items/entités : Peinture `immersive_paintings:painting`, Peinture lumineuse `immersive_paintings:glow_painting`,
  Graffiti `immersive_paintings:graffiti`, Graffiti lumineux `immersive_paintings:glow_graffiti` [j].

## Mécaniques
- Création : dépose une image (fichier, chemin ou URL) ou une capture d'écran dans l'écran dédié [j].
- Réglages à la création : largeur/hauteur en blocs, % dither, nombre de couleurs, offsets X/Y, zoom, mode
  pixelart (désactive le post-traitement) [j].
- Image avec transparence : le mod suggère un graffiti plutôt qu'une peinture [j].
- Cadres dispo : Aucun, Simple, Vintage, Maigre ; plusieurs matériaux de cadre (acacia, améthyste, bambou,
  bouleau, calcite...) [j].
- Une peinture peut être marquée NSFW (floutée pour les joueurs qui l'ont désactivé) ou cachée (invisible
  dans l'écran de sélection des autres joueurs) [j].
- Supprimer un tableau vide aussi tous les tableaux déjà placés utilisant ce nom (confirmation demandée avant) ;
  on peut les remplacer en réutilisant le même nom [j].
- Onglets de sélection : Créées, Datapacks, Joueurs, Nouvelle peinture [j].

## Config serveur
- `uploadPermissionLevel = 0` — tout le monde peut importer une image [c].
- `paintingsHaveCollision = false`, `testIfSpaceEmpty = false` [c].
- `maxUserImageWidth/Height = 4096`, `maxUserImages = 1000` par joueur [c].
- `minPaintingResolution = 8`, `maxPaintingResolution = 256` [c].
- `enableBundledPaintings = true` (peintures fournies par datapacks activées) [c].
- Client par défaut livré : `showNSFWPaintings = true`, `nsfwBlurAmount = 0.25` — réglable par chaque joueur
  côté client [c].
