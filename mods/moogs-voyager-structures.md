---
slug: moogs-voyager-structures
nom: "Moog's Voyager Structures"
namespaces: [mvs]
version: 5.1.1
cote: S
resume: "160+ petites/moyennes structures décoratives vanilla-style (puits, maisons, ruines, chariots), loot + ennemis + villageois"
sources:
  m: https://modrinth.com/mod/moogs-voyager-structures
  w: https://moogs-mods.fandom.com/wiki/Moog%27s_Voyager_Structures
  g: https://github.com/Moog-s-Mods/MoogsVoyagerStructures
  j: "jar MoogsVoyagerStructures-universal-1.21-5.1.1.jar"
  c: config serveur moogs_structures.json
verifie: 2026-09-13
---

`client_side: unsupported`, `server_side: required` : génération serveur only. Pas de nom traduit par structure dans le jar (lang = juste modmenu), ids bruts descriptifs. Faites en blocs/entités 100% vanilla. [j,m]
Chaque structure a son propre structure_set (~122 sets, 1 par structure, sauf `stalls` et `other_wells` qui regroupent plusieurs variantes). [j]

## Ajoute
- Puits (`*_well`) : `well`, `oak_well`, `birch_well`, `spruce_well`, `acacia_well`, `dark_oak_well`, `jungle_well`, `snowy_well`, `mushroom_well`, `desert_well`, `rocky_well`, `nether_well`, `small_copper_well`, `small_well`, `small_tower_well`, `rare_well` (regroupés dans le set `other_wells`). [j]
- Lanternes (`small_*_lantern`) : oak, birch, spruce, acacia, jungle, dark_oak, cherry, mangrove, bamboo + `medium_oak_lantern`, `small_campfire_lantern`. [j]
- Arbres et arbres morts par essence (`*_tree`, `dead_tree_*`) : oak, birch, spruce, acacia, jungle, dark_oak, cherry, mangrove, jungle_palm_tree, big_oak_tree. [j]
- Tas de bûches (`*_log_pile`) : oak, birch, spruce, acacia, jungle, dark_oak. [j]
- Maisons/habitats : `house`, `lil_house`, `tall_house`, `desert_house`, `deepslate_house`, `warped_house`, `azelea_house`, `mud_brick_house_1`, `prismarine_house_1`, `prismarine_house_2`, `small_swamp_house`, `diorite_and_deepslate_house`, `small_igloo`, `medium_igloo_1`, `medium_igloo_2`. [j]
- Tours/bâtiments hauts : `diorite_tower`, `jungle_tower`, `red_tower`, `large_warped_tower`, `cartographer_tower`, `small_pillager_tower`, `ocean_tower`. [j]
- Ruines : `castle_ruins`, `statue_ruins`, `small_ruin`, `log_ruin`. [j]
- Vie de village/ferme : `barn`, `shed`, `windmill`, `wooden_wheat_farm`, `wheat_grain_bin`, `horse_pen`, `horse_campsite`, `fox_hut`, `snowy_dog_hut`, `duck`, `bench`, `out_house`, `railway`, chariots (`cart`, `medium_bamboo_cart`, `large_cart_1`, `large_cart_2`), étals (`blue_stall`, `pink_stall`, `red_stall`, `orange_stall`, regroupés dans le set `stalls`). [j]
- Autres notables : `cathedral` (grande structure religieuse), `bee_dome`, `crystal`, `nether_devil`, `crimson_enchanting_table`, `floating_islands`/`large_floating_island`, `campsite`/`mine_with_campsite`/`horse_campsite`, `small_ship`, `sunzi_gate`, `villager_statue`, `mushroom_statue`, `large_mushroom`, `tree_monument`, `gallows`, `haystack`, `boulder`, `stone_rock`, `stone_pillars`, `stone_fountain`, `lamp_chest`, `lecturn_garden`, `flower_hole`, `small_oak_pond`, `mushroom_pond`, `paths`, `snowy_fossil`, `pile`. [j]

## Où trouver
- `/locate structure mvs:<id>` pour chaque structure ci-dessus. [j]

## Config serveur
- Config par défaut : aucun preset, aucun multiplicateur d'espacement (`universal_multiplier: 1.0`), aucune structure désactivée par nistroy. [c]
