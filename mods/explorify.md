---
slug: explorify
nom: Explorify
namespaces: [explorify]
version: v1.6.5
cote: S+C
resume: "Datapack de 14 nouvelles petites structures d'exploration (surface, Nether, End), vanilla-friendly"
sources:
  m: https://modrinth.com/mod/explorify
  j: "jar Explorify v1.6.5.mod.jar"
  c: config cristellib/explorify/
verifie: 2026-09-13
---

Pas de fichier lang dans le jar (structures sans nom en jeu). `client_side: optional`, `server_side: required`. [j,m]
Description Modrinth : "simplistic, vanilla-friendly collection of new structures". Version Fabric requiert Fabric API ; config geree par Cristel Lib (installe : `cristellib-fabric-1.21.1-3.1.7.jar`), sinon reglable par datapack. [m,j]

## Ajoute
- 14 structures (`data/explorify/worldgen/structure_set/`) : `badlands_pyramids`, `black_spirals`, `campsites`, `dark_forest_settlements`, `desert_shrines`, `end_shipwrecks`, `farmsteads`, `guide_posts`, `mangrove_huts`, `mausoleums`, `ruins`, `supply_caches`, `taverns`, `watchtowers`. [j]
- `guide_posts` a 2 variantes : `explorify:guide_post_cold`, `explorify:guide_post_warm`. [j]
- `supply_caches` a 7 variantes : `explorify:supply_cache/{birch,dark,desert,forest,jungle,mangrove,taiga}`. [j]
- `watchtowers` a 3 variantes : `explorify:watchtower/{plains,savanna,taiga}`. [j]

## Où trouver
- `/locate structure explorify:<id>` (ex. `explorify:badlands_pyramid`, `explorify:black_spiral`, `explorify:campsite`, `explorify:dark_forest_settlement`, `explorify:desert_shrine`, `explorify:end_shipwreck`, `explorify:farmstead`, `explorify:mangrove_hut`, `explorify:mausoleum`, `explorify:ruins`, `explorify:tavern`) ; variantes avec sous-chemin pour guide_post/supply_cache/watchtower ci-dessus. [j]
- `badlands_pyramid` genere en hauteur -12 a -9 (jigsaw vanilla, biome badlands via tag). [j]
- Loot notables : `dark_forest_settlement`, `mausoleum` (pot), `supply_cache` (table dediee, inclut butin de coffre village tannery vanilla en 1er pool). [j]

## Config serveur
- Cristel Lib genere `cristellib/explorify/structure_toggle_config.json5` (toutes structures/variantes `true`) et `structure_placement_config.json5` (spacing/separation/frequency par structure_set). [c]

## Pièges
- Auteur previent : mod encore en developpement, structures peuvent changer/disparaitre entre versions ; ca ne corrompt pas la sauvegarde mais backup conseille avant maj. [m]
