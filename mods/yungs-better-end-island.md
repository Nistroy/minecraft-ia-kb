---
slug: yungs-better-end-island
nom: YUNG's Better End Island
namespaces: [betterendisland]
version: 1.21.1-Fabric-3.1.2
cote: S
resume: "Refonte ile centrale de l'End : piliers, gateways, plateforme de spawn, portail au sommet d'une tour"
sources:
  m: https://modrinth.com/mod/yungs-better-end-island
  g: https://github.com/yungnickyoung/YUNGs-Better-End-Island
  j: jar YungsBetterEndIsland-1.21.1-Fabric-3.1.2.jar
  c: config betterendisland-fabric-1_21.toml
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us + ru_ru seulement). Pas de structure `/locate` : ce mod modifie directement
la generation de l'ile de l'End (structures NBT placees par mixin/processeurs), rien a chercher via commande. [j,m]

## Mecaniques
- Piliers d'obsidienne, gateways de l'End, plateforme de spawn et portail central redessines. [m]
- Le dragon ne spawn plus au demarrage : il faut s'approcher du beffroi (bell tower) au centre de l'ile pour le faire apparaitre. [m]
- Pour re-invoquer le dragon : 4 blocs de bedrock au sol dans la tour (un par aile), poser les cristaux dessus (au lieu des positions vanilla autour du portail) ; les positions vanilla restent aussi supportees. [m]
- IA du dragon inchangee. [m]
- Commande `/end_island reset` (variante `/end_island reset true` pour forcer le portail en surface) pour reinitialiser le combat + portail/piliers sur un monde existant. Faire une sauvegarde avant : operation lourde sur les donnees de la dimension. [m]
- Simple suppression des fichiers de la dimension End ne suffit pas : il faut lancer la commande. [m]

## Config serveur
- `resummonedDragonDropsEgg = false` : pas d'œuf de dragon à chaque ré-invocation. [c]
- `useVanillaSpawnPlatform = false`, `useVanillaEndGateways = false` : versions retravaillees utilisees (pas vanilla). [c]
- `playBellSound = true`, `spawnCentralTowerInitially = true`, `spawnCentralTowerOnResummon = true`. [c]

## Pièges
- `/end_island reset` : sauvegarder le monde avant (conseil explicite du mod). [m]
