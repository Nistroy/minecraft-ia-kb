---
slug: yungs-better-desert-temples
nom: YUNG's Better Desert Temples
namespaces: [betterdeserttemples]
version: 1.21.1-Fabric-4.1.5
cote: S
resume: "Refonte temple du desert : puzzles, pieges, parkour, boss Pharaon, mining fatigue tant que pas nettoye"
sources:
  m: https://modrinth.com/mod/yungs-better-desert-temples
  g: https://github.com/YUNG-GANG/YUNGs-Better-Desert-Temples
  j: jar YungsBetterDesertTemples-1.21.1-Fabric-4.1.5.jar
  c: config betterdeserttemples-fabric-1_21.toml + betterdeserttemples/fabric-1_21/
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us seulement). `/locate structure betterdeserttemples:desert_temple`. [j]

## Ajoute
- 1 structure `betterdeserttemples:desert_temple`, remplace le temple du desert vanilla. [j]
- Puzzles, pieges, parkour ajoutes vs vanilla ; meilleur loot. [m]
- Boss "Pharaoh" en fin de temple (advancement "Eternal Slumber" = tuer le Pharaon et lever la malediction). [j]
- Loot tables dediees : food_storage, lab, library, pharaoh_hidden, pot, statue, storage, tomb, tomb_pharaoh, wardrobe. [j]

## Mecaniques
- Mining fatigue appliquee aux joueurs dans le temple tant qu'il n'est pas nettoye (= Pharaon tue) ; effet leve definitivement apres. Desactivable en config. [m,j]
- Spawn mobs monstres : husk (10-32) dans la structure. [j]

## Config serveur
- `disableVanillaPyramids = true` : temples vanilla desactives, seuls les Better Desert Temples generent. [c]
- `applyMiningFatigue = true` : mining fatigue active. [c]

## Compat
- Prevu compatible avec YUNG's Better Mineshafts/Strongholds/Dungeons, YUNG's Extras/Bridges. [m]
- Repurposed Structures propose un datapack additionnel pour variantes du temple (non installe ici, a verifier). [m]
- `client_side: unsupported`, `server_side: required` sur Modrinth : rien a installer cote joueur. [m]
