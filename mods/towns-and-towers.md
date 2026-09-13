---
slug: towns-and-towers
nom: Towns and Towers
namespaces: [towns_and_towers, kaisyn]
version: 1.13.11
cote: S+C
resume: "27 villages + 31 avant-postes pillards par biome (dont variantes exclusives biomes moddés) + village océan naval avec navires"
sources:
  m: https://modrinth.com/mod/towns-and-towers
  j: jar t_and_t-fabric-neoforge-1.13.11.jar
  c: "config serveur towns_and_towers/structure_enable_or_disable_new.json5, structure_rarity_new.json5"
verifie: 2026-09-13
---

Pas de fichier de langue dans le jar : ids bruts, descriptif seulement. Dépend de `cristellib`. `/locate structure towns_and_towers:<id>`. [j,m]

## Ajoute
- 27 villages (`village_<biome>`) : badlands, beach, birch_forest, flower_forest, forest, grove, jungle, meadow, mushroom_fields, ocean, old_growth_taiga, savanna_plateau, snowy_slopes, snowy_taiga, sparse_jungle, sunflower_plains, swamp, wooded_badlands + 9 « exclusives » (classic, iberian, mediterranean, nilotic, piglin, rustic, swedish, tudor, wandering_trader_camp) réservées aux biomes d'autres mods de worldgen (ex. Terralith, cité en commentaire config). [j,c]
- 31 avant-postes pillards (`pillager_outpost_<biome>`), même logique + 8 variantes exclusives (classic, iberian, mediterranean, nilotic, oriental, rustic, swedish, tudor). [c]
- `mimic_desert`, `wreckage_ocean` : structures hors village/avant-poste. [c]
- `village_ocean` : variante navale en océan profond, utilise des structures navires du namespace `kaisyn` (`mothership`, `escort`, `small_ship`) au lieu de bâtiments classiques ; biome tag `towns_and_towers:has_structure/village_deep_oceans_ships`. [j]

## Où trouver
- Ids `towns_and_towers:village_<biome>` / `towns_and_towers:pillager_outpost_<biome>`. [j]

## Config serveur
- Toutes les structures activées (`true`) dans `structure_enable_or_disable_new.json5` — aucune désactivée par nistroy. [c]
- Espacement villages (`towns`) : `spacing: 51` (défaut 48), `separation: 12` (défaut 24) — un peu plus espacés en distance max mais bien plus fréquents en distance mini. [c]
- Espacement avant-postes (`towers`) : `spacing: 48` (défaut), `separation: 12` (défaut 24) — plus fréquents que le défaut du mod. `frequency: 0.2`. [c]
- Structures « other » (`mimic_desert`, `wreckage_ocean`) : `spacing: 32` (défaut), `separation: 16` (défaut). [c]
