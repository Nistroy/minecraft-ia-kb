---
slug: when-dungeons-arise
nom: When Dungeons Arise
namespaces: [dungeons_arise]
version: 2.1.68
cote: S
resume: 39 grandes structures hostiles (illagers, ciel, industriel, mer, antique) + cartes d'exploration
sources:
  m: https://modrinth.com/mod/when-dungeons-arise
  j: jar DungeonsArise-1.21.1-2.1.68-fabric-release.jar
verifie: 2026-09-13
---

Pas de traduction FR dans le jar. Chercher par id : `/locate structure dungeons_arise:<id>`. Regroupement par thème = descriptif. [j]

## Ajoute
- 39 structures (`data/dungeons_arise/worldgen/structure/`), grands bâtiments peuplés d'ennemis. [j,m]
- Illagers : `illager_campsite`, `illager_fort`, `illager_windmill`, `illager_corsair`, `illager_galley`. [j]
- Ciel / volant : `heavenly_rider`, `heavenly_conqueror`, `heavenly_challenger`, `small_blimp`, `aviary`, `mechanical_nest`. [j]
- Antique / temples : `ceryneian_hind`, `typhon`, `shiraz_palace`, `kisegi_sanctuary`, `keep_kayra`, `abandoned_temple`, `infested_temple`, `plague_asylum`, `monastery`, `coliseum`. [j]
- Industriel / mines : `foundry`, `mining_system`, `mining_complex`, `scorched_mines`. [j]
- Mer : `undead_pirate_ship`, `lighthouse`, `fishing_hut`. [j]
- Villages / divers : `bandit_village`, `bandit_towers`, `thornborn_towers`, `mushroom_village`, `mushroom_house`, `mushroom_mines`, `giant_mushroom`, `merchant_campsite`, `wishing_well`, `greenwood_pub`, `jungle_tree_house`, `bathhouse`. [j]

## Où trouver
- Cartes d'exploration : 31 types (`filled_map.dungeons_arise:*`, nom en jeu « <Structure> Explorer Map ») ; en loot de coffres de certaines structures (ex. `abandoned_temple`, `illager_campsite`, `merchant_campsite`, `monastery`). [j]
- `merchant_campsite` et `monastery` contiennent des villageois (template pools `villagers`). [j]

## Compat
- `client_side: unsupported` côté Modrinth : génération de structures côté serveur uniquement, rien à installer côté joueur. [m]
