---
slug: bosses-of-mass-destruction
nom: Bosses of Mass Destruction
namespaces: [bosses_of_mass_destruction]
version: 1.10.2-1.21.1
cote: S+C
resume: 4 boss endgame (Night Lich, Obsidilith, Nether Gauntlet, Void Blossom) + arènes générées
sources:
  m: https://modrinth.com/mod/bosses-of-mass-destruction
  g: https://github.com/miyo6032/bosses-of-mass-destruction
  j: jar BOMD-1.10.2-1.21.1.jar
  c: config serveur bosses_of_mass_destruction.json5
verifie: 2026-09-13
---

Pas de traduction FR dans le jar : noms en jeu en anglais (glose FR entre parenthèses). [j]

## Ajoute
- 4 boss (`bosses_of_mass_destruction:*`) :
  - Night Lich (`lich`) - tours rares en biomes froids, repérables via les Soul Star (`soul_star`) qui tombent des morts-vivants tués à proximité. [j,m,c]
  - Obsidilith (`obsidilith`) - structures rares dans les îles de l'End, cadre d'obsidienne (`obsidilith_end_frame`). [j,m]
  - Nether Gauntlet (`gauntlet`) - structures rares du Nether, blackstone spéciale (`gauntlet_blackstone`). [j,m]
  - Void Blossom (`void_blossom`) - grottes rares au fond du monde, repérable via les `void_lily`. [j,m]
- Drops/matériaux des boss : Ancient Anima (`ancient_anima`), Blazing Eye (`blazing_eye`), Obsidian Heart (`obsidian_heart`), Void Thorn (`void_thorn`). [j]
- Crystal Fruit (`crystal_fruit`) : régénération + résistance brèves. [j]
- Charged Ender Pearl (`charged_ender_pearl`) : réutilisable, résistance brève après téléport. [j]
- Earthdive Spear (`earthdive_spear`) : téléport courte portée à travers les blocs. [j]
- Blocs utilitaires : Staff of Suppression (`mob_ward`, aucun spawn de mob à 64 blocs dans toutes les directions), Blast Amplifier (`monolith_block`, +30 % puissance d'explosion à 64 blocs, non cumulable), Table of Elevation (`levitation_block`, vol créatif dans une colonne 7x7). [j]
- Brimstone Nectar (`brimstone_nectar`) : réinitialise les structures de boss proches à l'usage. [j]

## Config serveur (valeurs actuelles)
- Night Lich : 300 PV, nuit éternelle pendant le combat (`eternalNighttime`), 1500 XP au kill ; drop de Soul Star toutes les 50 morts-vivants tués à proximité. [c]
- Obsidilith : 300 PV, 14 armure, 16 attaque, fait apparaître un pilier à sa mort. [c]
- Nether Gauntlet : 250 PV, 8 armure, 16 attaque, fait apparaître des débris antiques à sa mort. [c]
- Void Blossom : 350 PV, 4 armure, 12 attaque. [c]
- Table of Elevation : rayon d'effet 3 blocs. [c]

## Pièges
- Régénération passive des boss hors combat (`idleHealingPerTick`) : un boss laissé tranquille se soigne. [c]
