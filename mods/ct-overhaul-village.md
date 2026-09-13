---
slug: ct-overhaul-village
nom: "ChoiceTheorem's Overhauled Village"
namespaces: [ctov]
version: 3.6.3
cote: S
resume: "Remplace villages + avant-postes pillards vanilla par des versions enrichies : 22 variantes de village en 3 tailles, 12 avant-postes"
sources:
  m: https://modrinth.com/mod/ct-overhaul-village
  w: https://github.com/ChoiceTheorem/ChoiceTheorem-s-overhauled-village/wiki
  g: https://github.com/ChoiceTheorem/ChoiceTheorem-s-overhauled-village
  j: "jar [Fabric]ctov-3.6.3.jar"
  c: config serveur ctov.json
verifie: 2026-09-13
---

`client_side: unsupported`, `server_side: required` : génération 100 % serveur, rien à installer côté joueur. Dépend de `lithostitched`. [j,m]

## Ajoute
- Villages en 3 tailles (`small`/`medium`/`large`), 22 variantes chacune : `beach`, `christmas`, `dark_forest`, `desert`, `desert_oasis`, `jungle`, `jungle_tree`, `mesa`, `mesa_fortified`, `mountain`, `mountain_alpine`, `mushroom`, `plains`, `plains_fortified`, `savanna`, `savanna_na`, `snowy_igloo`, `swamp`, `swamp_fortified`, `taiga`, `taiga_fortified`, `underground`. [j]
- 12 avant-postes de pillards : `badlands`, `beach`, `dark_forest`, `desert`, `jungle`, `mesa`, `mountain`, `plains`, `savanna`, `snowy`, `swamp`, `taiga`. [j]
- Structures ajoutées au tag vanilla `minecraft:village` (via `ctov:village`). [j]

## Où trouver
- Ids : `ctov:<taille>/village_<variante>`, `ctov:pillager_outpost_<biome>`. Ex. `/locate structure ctov:large/village_plains`. [j]

## Config serveur
- Villages petits/moyens/grands et avant-postes tous générés (`generate*Village`, `generatePillagerOutpost` = true). [c]
- Poids : petit village 10, moyen 4, grand 1, avant-poste 1 → petits villages les plus fréquents. [c]
- Villages activés : les 21 variantes sauf `underground`. [c]
- Avant-postes activés : 11, tous sauf `mesa`. [c]
