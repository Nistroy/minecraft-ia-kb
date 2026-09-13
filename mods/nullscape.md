---
slug: nullscape
nom: Nullscape
namespaces: [nullscape]
version: 1.2.14
cote: S
resume: Refonte de l'End vanilla (terrain alien, 3 biomes, structures)
sources:
  m: https://modrinth.com/mod/nullscape
  w: https://stardustlabs.miraheze.org/wiki/Nullscape
  g: https://github.com/Stardust-Labs-MC/Nullscape
  j: jar Nullscape_1.21.x_v1.2.14.jar
verifie: 2026-09-13
---

## Ajoute
- Datapack pur : remplace directement le générateur de `minecraft:the_end` (aucun bloc/item/mob propre, aucune traduction dans le jar). [j]
- Noms FR ci-dessous = traductions descriptives, pas des noms en jeu (datapack sans fichier de langue) ; chercher par id : `/locate biome nullscape:<id>`, `/locate structure nullscape:<id>`. [j]
- 3 biomes : Landes du néant (`void_barrens`), Terres d'ombre (`shadowlands`), Pics de cristal (`crystal_peaks`). [j]
- 2 structures jigsaw : Squelette de dragon (`dragon_skeleton`), Faille (`rift`, pool `gateways_shadow`). [j]
- ~107 placed_feature / ~118 configured_feature ajoutés pour le terrain (décor, formations). [j]

## Où trouver
- `dragon_skeleton` : hauteur 20-240, distance max 112 blocs du centre du chunk de génération, biomes tagués `nullscape:has_structure/dragon_skeleton`. [j]
- `rift` : hauteur fixe au niveau du sol (`WORLD_SURFACE`), distance max 32 blocs, biomes tagués `nullscape:has_structure/rift`. [j]

## Compat
- `client_side: optional` côté Modrinth : rejoindre sans le mod possible, mais le terrain généré par le serveur ne sera pas rendu correctement côté client sans lui. [m]
