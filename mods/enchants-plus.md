---
slug: enchants-plus
nom: Enchants Plus
namespaces: [enchantsplus]
version: 1.6B
cote: S
resume: 18 enchantements + 4 malédictions data-driven 1.21, style vanilla, modifie aussi Power/Sharpness/Silk Touch
sources:
  m: https://modrinth.com/mod/enchants-plus
  j: jar "Enchants+ 1.21 - 1.21.1 fabric-forge.jar"
verifie: 2026-09-13
---

## Ajoute
Enchantements `enchantsplus:<id>` (pas de fichier lang, nom en jeu = texte fallback JSON) [j] :
- Breeze Burst (arc, niv. max 1) : flèche tirée fait apparaître une charge de vent à l'impact [m,j].
- Crab's Touch (outils/cisailles, niv. max 3) : augmente la portée d'interaction avec les blocs, jusqu'à ~7.5 blocs
  au niv. 3 ; utilisable en main secondaire pour poser des blocs à distance [m,j].
- Gluttony (outils/épée/cisailles, niv. max 3) : blocs minés vont direct dans l'inventaire ; niv. 3 récupère aussi
  l'XP [m,j].
- Graviole (élytres, niv. max 3) : résiste à la gravité, vol plus long mais plus lent (pas d'accélération par
  chute) [m,j].
- Ice Aspect (épée, niv. max 2) : 10%/20% de chance de geler l'ennemi 3s (immobile). Incompatible Fire Aspect et
  Websnare [m,j].
- Kinetic Protection (casque, niv. max 4) : protège des dégâts cinétiques d'élytre [m,j].
- Luminosity (plastron, niv. max 3) : émet lumière niv. 5/10/15 selon le niveau [m,j].
- Outreach (épée, niv. max 2) : portée d'attaque augmentée à 4 blocs au niv. 2. Incompatible avec Swift Strike
  (`exclusive_set`) [m,j].
- Precision (arc/arbalète, niv. max 2) : réduit la courbe de trajectoire des projectiles, portée d'effet plus
  grande au niv. 2 [m,j].
- Pyrolysis (pioche/hache/pelle, niv. max 1) : auto-fonte des blocs minés. Incompatible Fortune et Silk Touch
  (`exclusive_set: minecraft:exclusive_set/mining`) [m,j].
- Retrieval (plastron, niv. max 4) : chance de récupérer dans l'inventaire les flèches tirées sur soi (jusqu'à 80%
  au niv. 4) ; effets des flèches à potion sont perdus [m,j].
- Scorch Walker (bottes, niv. max 2) : équivalent Frost Walker pour la lave (crée du magma), protège aussi des
  dégâts de magma/neige poudreuse [m,j].
- Skyguard (élytres, niv. max 4) : équivalent Protection pour les élytres [m,j].
- Stride (jambières, niv. max 3) : permet de monter les blocs pleins sans sauter, comme des marches [m,j].
- Swift Strike (épée/hache, niv. max 5) : réduit le temps de recharge d'attaque. Incompatible avec Outreach
  (`exclusive_set`) [m,j].
- Toxic (arc/arbalète, niv. max 1) : flèches empoisonnent la cible 11s, sans effet sur les morts-vivants [m,j].
- Vitality (plastron, niv. max 3) : augmente la vie max, jusqu'à 13 cœurs au niv. 3 [m,j].
- Websnare (épée, niv. max 2) : chance de faire apparaître une toile sous la cible touchée. Incompatible Fire
  Aspect et Ice Aspect [m,j].
- Curse of Breaking (tout équipement, niv. max 1) : durabilité perdue 4x plus vite [m,j].
- Curse of Clumsiness (outils/armes, niv. max 1) : chance de faire tomber l'objet au sol en minant/attaquant [m,j].
- Curse of Displacement (armes, niv. max 1) : téléporte parfois l'ennemi touché derrière le joueur [m,j].
- Curse of Double Edge (armes, niv. max 1) : 40% de chance d'infliger des dégâts au porteur en attaquant [m,j].

## Où trouver
- Table d'enchantement et commerces de villageois pour la plupart des enchants ; certains uniquement en butin :
  Breeze Burst/Ice Aspect (chambres d'épreuves), Crab's Touch (épaves, trésor enfoui, ruines), Graviole/Skyguard
  (cités de l'End), Scorch Walker/Websnare (butin aléatoire seulement, pas de table) — détail par enchant sur la
  page Modrinth [m].

## Compat
- Modifie 3 enchantements vanilla : Power fonctionne aussi sur l'arbalète, Sharpness sur le trident, Silk Touch sur
  l'épée (pour récolter les toiles d'araignée) [m,j].
- Existe un pack de ressources complémentaire "Enchants Plus - Descriptions & Translations" pour les descriptions
  d'enchant en jeu (non installé chez nous, non vérifié) [m].
