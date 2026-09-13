---
slug: deeperdarker
nom: Deeper and Darker
namespaces: [deeperdarker]
version: 1.3.3-plus-b-fabric+1.21
cote: S+C
resume: Dimension Otherside (sculk), équipement Warden, nouveaux mobs de sculk
sources:
  m: https://modrinth.com/mod/deeperdarker
  g: https://github.com/KyaniteMods/DeeperAndDarker
  j: jar deeperdarker-fabric-1.21-1.3.3-plus-b.jar
  c: config serveur deeperdarker.json5
verifie: 2026-09-13
---

## Ajoute
- Dimension `deeperdarker:otherside` (« sous la bedrock » selon l'advancement), accessible par un portail `deeperdarker:otherside_portal` ; salles de portail dans le sous-sol du Temple antique. Construction du cadre non documentée dans le jar ni sur Modrinth. [j]
- 4 biomes : Cavernes fleuries (`blooming_caverns`), Terres profondes (`deeplands`), Forêt en écho (`echoing_forest`), Colonnes voilées (`overcast_columns`). [j]
- 1 structure : Temple antique (`ancient_temple`), contient un Ancien vase (`ancient_vase`, peut faire apparaître mobs/sangsues de sculk). [j,c]
- Mobs : Mille-pattes de sculk (`sculk_centipede`), Sangsue de sculk (`sculk_leech`), Mordeur de sculk (`sculk_snapper`), Ver hurleur (`shriek_worm`), Stalker (`stalker`), Shattered (`shattered`). Pas de boss identifié (aucune barre de vie dédiée dans le jar). [j]
- Équipement complet Warden (`warden_*`) : armure + carapace, outils et épée, hache, houe, pelle, modèle de forge dédié. [j]
- Bois d'écho (`echo_*`) et bois fleuri (`bloom_*`) : planches/bûches/portes/bateaux, etc. [j]
- Pierres : ardoise sombre (`gloomslate`), roche de sculk (`sculk_stone`), glaise (`sculk_grime`) - variantes taillées/polies/dalles/escaliers. [j]
- Objets : Bâton sonore (`sonorous_staff`, arme à distance), Élytres des âmes (`soul_elytra`), Cristal d'âmes, Coeur des profondeurs (`heart_of_the_deep`), Émetteur de sculk (`sculk_transmitter`, transmet redstone à distance via liaison). [j]

## Mécaniques
- Portail Otherside : dimensions min 2x2, max 48x24 blocs ; portail généré par le mod fait 8x4. [c]
- Émetteur de sculk : bloc "connecté" à un autre émetteur pour transmettre un signal ; état lié/non lié affiché en jeu. [j]

## Config serveur
- `addWardenDrops` = true : le Warden lâche du loot supplémentaire du mod. [c]
- `addAncientCityLoot` = true : loot du mod ajouté aux coffres des cités antiques. [c]
- `sculkLeechesFromAncientVaseChance` = 0.7 : chance qu'un ancien vase brisé fasse apparaître des sangsues de sculk. [c]
- `sonorousStaffDamage` = 50, `sonorousStaffCooldown` = 20 ticks, portée 40 : réglages du Bâton sonore. [c]
