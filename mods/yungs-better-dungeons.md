---
slug: yungs-better-dungeons
nom: YUNG's Better Dungeons
namespaces: [betterdungeons]
version: 1.21.1-Fabric-5.1.4
cote: S
resume: "Refonte donjons vanilla + 3 nouveaux : Catacombes (zombie), Fortress of the Undead (squelette), Spider Cave"
sources:
  m: https://modrinth.com/mod/yungs-better-dungeons
  g: https://github.com/YUNG-GANG/YUNGs-Better-Dungeons
  j: jar YungsBetterDungeons-1.21.1-Fabric-5.1.4.jar
  c: config betterdungeons-fabric-1_21.toml
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us seulement). `client_side: unsupported`, `server_side: required`. [j,m]

## Ajoute
- `betterdungeons:small_dungeon` = refonte du donjon vanilla ("upgraded Monster Room", advancement "Quite the Renovation"). [j]
- `betterdungeons:zombie_dungeon` = "Catacombs" (advancement "When in Rome" : "Set foot in a Catacomb"). [j]
- `betterdungeons:skeleton_dungeon` = "Fortress of the Undead" (advancement "A Bone to Pick" : "Enter a Fortress of the Undead"). [j]
- `betterdungeons:spider_dungeon` = "Spider Cave" (advancement "Cobweb Entanglement"). [j]
- `betterdungeons:small_nether_dungeon` = petit donjon Nether, feature opt-in (Nether Update 1.19.2+). [m,j]
- Advancement "Professional Dungeoneer" = explorer tous les Better Dungeons. [j]

## Mecaniques
- `small_nether_dungeon` = feature a activer manuellement en config (desactivee par defaut). [m,c]

## Config serveur
- `removeVanillaDungeons = true` : donjons vanilla desactives, remplaces par les Better Dungeons. [c]
- `enableHeads = true`, `enableNetherBlocks = true` : options actives (defaut). [c]
- `smallNetherDungeon.enabled = false` : donjon Nether desactive sur notre serveur. [c]
- `smallNetherDungeon.witherSkeletonsDropWitherSkulls = true`, `blazesDropBlazeRods = true` (si active un jour). [c]
- `zombieDungeon.zombieDungeonMaxSurfaceStaircaseLength = 20`, `smallDungeon.chestMinCount/MaxCount = 1/2`. [c]

## Compat
- Prevu compatible YUNG's Better Mineshafts/Strongholds, YUNG's Extras/Bridges. Repurposed Structures propose un datapack additionnel pour les petits donjons (non installe ici). [m]
