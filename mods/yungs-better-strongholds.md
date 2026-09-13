---
slug: yungs-better-strongholds
nom: YUNG's Better Strongholds
namespaces: [betterstrongholds]
version: 1.21.1-Fabric-5.1.3
cote: S
resume: "Refonte complete des strongholds vanilla : 15+ salles, pieges, zones cachees, via YUNG's API"
sources:
  m: https://modrinth.com/mod/yungs-better-strongholds
  g: https://github.com/YUNG-GANG/YUNGs-Better-Strongholds
  j: jar YungsBetterStrongholds-1.21.1-Fabric-5.1.3.jar
  c: config betterstrongholds-fabric-1_21.toml + betterstrongholds/fabric-1_21/
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us, ru_ru, uk_ua). `client_side: unsupported`, `server_side: required`. [j,m]
Depend de `yungsapi >= 1.21.1-Fabric-5.1.4`, installe (`YungsApi-1.21.1-Fabric-5.1.8.jar`). [j]

## Ajoute
- `betterstrongholds:stronghold` remplace le stronghold vanilla (tag `better_strongholds` alimente `eye_of_ender_located`). [j]
- Plus de 15 types de salles differentes, tunnels/couloirs varies, escaliers, pieges, zones cachees. [m]
- Salles notees dans la config : Armoury (armor stands), Grand Library (blocs rares), storage/armoury (item frames), treasure rooms (piles de minerai). [c]

## Mecaniques
- Structure generee via `yungsapi:yung_jigsaw`, pool de depart `betterstrongholds:starts`, taille 15, hauteur -30 a 11 (limite `max_y` 60). [j]
- Placement : `spacing` 85, `separation` 50 chunks (structure_set). [j]
- `enableStructureRuin` : autorise les strongholds a etre legerement abimes par les petites grottes "noodle caves" (pas les grandes cavernes). [j,c]
- `filledPortalFrameChance` : chance par bloc de cadre de portail de l'End de spawn deja rempli d'un oeil de l'ender. [j]

## Où trouver
- `/locate structure betterstrongholds:stronghold`. [j]
- Salles a butin : Armoury, Crypt, Grand Library, Library (md), Mess, Prison, Trap, Treasure, Common (`data/betterstrongholds/loot_table/chests/`). [j]

## Config serveur
- `enableStructureRuin = false` : ruine désactivée sur notre serveur. [c]
- `filledPortalFrameChance = 0.1`. [c]
- `betterstrongholds/fabric-1_21/` : `ores.json`/`rareblocks.json` (probabilites de blocs dans treasure/grand library), `armorstands.json`/`itemframes.json` (probabilites d'items). [c]

## Compat
- Prevu compatible avec YUNG's Better Mineshafts (installe), YUNG's Better Dungeons (installe), YUNG's Extras, YUNG's Bridges, Better End, End Remastered. [m]
- Repurposed Structures (non installe) : si ses strongholds sont actives, l'oeil de l'ender vise le plus proche stronghold (RS ou Better Strongholds) ; offre aussi un datapack pour versions Nether/End du stronghold (non installe ici). [m]
