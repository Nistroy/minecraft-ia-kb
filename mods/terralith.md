---
slug: terralith
nom: Terralith
namespaces: [terralith]
version: 2.6.2
cote: S+C
resume: "95 biomes overworld (surface + cavernes) + structures custom (villages fortifiés, tours de mage, ruines), datapack pur vanilla"
sources:
  m: https://modrinth.com/mod/terralith
  w: https://stardustlabs.miraheze.org/wiki/Terralith
  g: https://github.com/Stardust-Labs-MC/Terralith
  j: jar Terralith_1.21.x_v2.6.2.jar
  c: config serveur terralith.json
verifie: 2026-09-13
---

Datapack de worldgen, aucun bloc/item custom (que du vanilla). `client_side: optional`, `server_side: required` : fonctionne sans mod côté client mais recommandé pour cohérence visuelle. [m]

## Ajoute
- 95 biomes overworld dans `data/terralith/worldgen/biome/`, dont 11 cavernes `terralith:cave/<id>` : Cavernes d'andésite `andesite_caves`, Cavernes profondes `deep_caves`, Cavernes de diorite `diorite_caves`, Cavernes de Feugivre `frostfire_caves`, Cavernes fongiques `fungal_caves`, Cavernes de granite `granite_caves`, Cavernes infestées `infested_caves`, Cavernes palléales `mantle_caves`, Cavernes thermales `thermal_caves`, Cavernes de tuf `tuff_caves`, Jungle souterraine `underground_jungle`. [j]
- 34 fichiers de structure custom (`data/terralith/worldgen/structure/`) : villages fortifiés (`fortified_village`, `fortified_desert_village`), tours de mage (`mage_tower` + variantes saison), avant-poste désertique (`desert_outpost`), huttes/spires (`glacial_hut`, `spire`, `witch_hut`), ruines (`rubble_*`), structures souterraines (`underground/giant_bee_hive`, `underground/oak_cabin`, `underground/mining_outpost`, `underground/old_refinery`, `underground/sunken_tower`, `underground/witch_hut`, `underground/frosted_dungeon`). [j]
- Structure sets : `mage`, `rare_dungeon`, `rare_village`, `regular`, `rubble`, `underground`, `underground_dungeon`. [j]
- Îles volantes : 4 biomes saisonniers au-dessus des océans profonds, Îles volantes (Printemps/Été/Automne/Hiver) `skylands_spring/summer/autumn/winter` ; module `skylands` activable séparément. [j,c]

## Où trouver
- Biomes overworld classiques : `/locate biome terralith:<id>` (ex. `terralith:yellowstone`, `terralith:bryce_canyon`, `terralith:sakura_grove`). [j]
- Structures : `/locate structure terralith:<id>` (ex. `terralith:fortified_village`, `terralith:mage_tower`). Noms FR dans le jar (« Village fortifié », « Spire », « Hutte glaciale »...). [j]
- Biomes de caverne : sous terre, id `terralith:cave/<id>` (visible en F3). [j]

## Config serveur
- `custom_structures: true` — structures custom actives (villages fortifiés, tours de mage...). [c]
- `skylands: true` — îles volantes générées. [c]
- `terrain_slabs: true`, `vanilla_stone_gen: false`, `recipe_changes: false`, `intro_message: true`. [c]

