---
slug: dungeons-and-taverns
nom: Dungeons and Taverns
namespaces: [nova_structures, dnt]
version: v4.4.4+mod
cote: S+C
resume: "136 structures overworld/nether/end (donjons, tavernes, camps, ruines) + minibosses, clés, cartes de quête via tavernier"
sources:
  m: https://modrinth.com/mod/dungeons-and-taverns
  j: jar dungeons-and-taverns-v4.4.4.jar
verifie: 2026-09-13
---

Gros datapack (23,7 Mo), `client_side: optional`, `server_side: required`. Namespace worldgen `nova_structures`, namespace items/lang/avancements `dnt`. Lang fr_fr complète dans le jar. [j,m]

## Mécaniques
- Quête : échanger avec un cartographe tavernier (Tavern Cartographer) donne accès à une carte de quête (advancement « Appel à l'aventure », `tavern_quest`). [j]
- Clés de donjon par structure : `citadel_key`/`citadel_boss_key`, `end_castle_key`, `end_ship_key`, `nether_keep_key`, `ominous_swamp_village_key`, `ominous_toxic_key`/`toxic_key`/`toxic_boss_key`, `piglin_donjon_key`, `piglin_outstation_key`, `shrine_key`, `trident_trial_key`/`trident_trial_boss_key`, `creeper_key` — ouvrent des coffres/portes spécifiques à leur structure. [j]
- Minibosses dans certaines structures ; advancement « C'est moi le Maître de jeu » (`kill_all_minibosses`) = tuer chaque miniboss du mod une fois. Liste des minibosses non documentée dans le jar. [j]
- Cartes d'exploration en loot (`filled_map.dnt.*`) pour de nombreuses structures : hameau/donjon/avant-poste de Piglins, avant-poste de pillards, cité ancienne, villa de sorcière, avant-poste minier des badlands, refuge d'illageois, village, crypte de morts-vivants, monument des épreuves du Trident, repère toxique, fort vagabond, citadelle isolée, ruines de la jungle, manoir d'illageois, ruines du désert, crypte sifflante, phare/château de l'End. [j]
- Potions/flèches custom : lévitation, nausée, décomposition (wither), cécité persistante. [j]

## Ajoute
- 136 fichiers de structure (`data/nova_structures/worldgen/structure/`), thèmes principaux :
  - Tavernes par essence de bois : `tavern_oak/birch/spruce/jungle/acacia/dark_oak/mangrove/cherry`, + `tavern_desert`, `tavern_snowy`, `tavern_swamp`. [j]
  - Tours de guet (« firewatch ») par biome : `firewatch_tower` + variantes birch/cherry/dark_oak/forest/jungle/mangrove/savanna/swamp/taiga. [j]
  - Camps/tours de squelette du Nether : `skeleton_camp_crimson/soul/warped/waste`, `nether_skeleton_tower_crimson/soul/warped/waste`. [j]
  - Piglins : `piglin_camp`, `piglin_donjon`, `piglin_outstation`. [j]
  - Illageois/sorcières : `illager_camp`, `illager_hideout`, `illager_manor`, `mangrove_witch_hut`, `witch_villa`. [j]
  - Ruines/hameaux « remnant_* » (petites structures overworld variées : ferme d'abeilles, cimetière, forge, ranch, école, château de taïga...). [j]
  - End : `end_castle`, `end_ship`, `end_lighthouse`. [j]
  - Autres majeures : `ancient_city` (variante custom), `bastion_remnant` (variante custom), `nether_fortress` (variante custom), `lone_citadel`, `shrine` (+ `shrine_combat_tier_1` à `5`), `trident_trial_monument`, `toxic_lair`, `undead_crypt`, `creeping_crypt`, `stray_fort`, `desert_ruins`, `jungle_ruins`, `ruin_town`, `deepslate_camp`, `badlands_miner_outpost`, `bunker`, `conduit_ruin`, `wild_ruin`. [j]
  - Puits/villages custom par biome : `well_oak/birch/spruce/jungle/dark_oak/savana`, `village_birch/jungle/swamp/taiga`. [j]

## Où trouver
- `/locate structure nova_structures:<id>` pour toutes les structures ci-dessus. [j]
