---
slug: ct-overhaul-village
nom: "ChoiceTheorem's Overhauled Village"
namespaces: [ctov]
version: 3.6.3
cote: S
resume: "Remplace villages + avant-postes pillards vanilla par des versions enrichies (3 tailles), 11 biomes de village + 11 d'avant-poste"
sources:
  m: https://modrinth.com/mod/ct-overhaul-village
  w: https://github.com/ChoiceTheorem/ChoiceTheorem-s-overhauled-village/wiki
  g: https://github.com/ChoiceTheorem/ChoiceTheorem-s-overhauled-village
  j: "jar [Fabric]ctov-3.6.3.jar"
  c: config serveur ctov.json
verifie: 2026-09-13
---

`client_side: unsupported`, `server_side: required` : génération 100% serveur, rien à installer côté joueur. Dépend de `lithostitched`. [j,m]

## Ajoute
- Villages en 3 tailles (petit/moyen/grand) pour 11 biomes : plage, forêt sombre, désert, jungle, badlands/mesa, montagne, champignon, plaines, savane, enneigé, marais, taïga (`structure.ctov.small/medium/large.village_<biome>`). [j]
- Avant-postes de pillards enrichis pour 11 biomes : plage, forêt sombre, désert, jungle, badlands, montagne, plaines, savane, enneigé, marais, taïga (`structure.ctov.pillager_outpost_<biome>`). [j]
- 106 fichiers de structure au total (`data/ctov/worldgen/structure/`) : villages/avant-postes + pièces de génération jigsaw associées. [j]

## Où trouver
- Ids réels : `ctov:small/village_<biome>`, `ctov:medium/village_<biome>`, `ctov:large/village_<biome>`, `ctov:pillager_outpost_<biome>`. Ex. `/locate structure ctov:large/village_plains`. [j]
- Pas de nouveau structure_set dans le jar : le mod ajoute ses structures au tag vanilla `minecraft:village` (via `ctov:village`), donc génère à la place des villages/avant-postes vanilla. [j]
- Variantes supplémentaires activées côté config : `desert_oasis`, `jungle_tree`, `mesa_fortified`, `mountain_alpine`, `savanna_na`, `snowy_igloo`, `swamp_fortified`, `taiga_fortified`, `christmas` (village de Noël saisonnier). [c]

## Config serveur
- Tailles activées : `generatesmallVillage`, `generatemediumVillage`, `generatelargeVillage`, `generatePillagerOutpost` toutes `true`. [c]
- Poids de génération : petit village 10, moyen 4, grand 1, avant-poste 1 (petit village le plus fréquent). [c]
- 21 variantes de village activées, 11 variantes d'avant-poste activées (voir `enabledvillage`/`enabledpillageroutpost` du fichier config). [c]
