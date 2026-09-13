---
slug: yungs-better-jungle-temples
nom: YUNG's Better Jungle Temples
namespaces: [betterjungletemples]
version: 1.21.1-Fabric-3.1.2
cote: S
resume: "Refonte complete du temple de la jungle : nouveau design, pieges, puzzles, loot"
sources:
  m: https://modrinth.com/mod/yungs-better-jungle-temples
  g: https://github.com/YUNG-GANG/YUNGs-Better-Jungle-Temples
  j: jar YungsBetterJungleTemples-1.21.1-Fabric-3.1.2.jar
  c: config betterjungletemples-fabric-1_21.toml
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us seulement). `/locate structure betterjungletemples:jungle_temple`.
`client_side: unsupported`, `server_side: required`. [j,m]

## Ajoute
- 1 structure `betterjungletemples:jungle_temple`, remplace le temple de la jungle vanilla. [j]
- Nouveau design, pieges, puzzles, loot ameliore vs vanilla. [m]
- Loot tables : chests/campsite, chests/treasure, archaeology/emerald (fouille archeo). [j]
- Compat optionnelle citee par le mod : Create, Supplementaries, Alex's Mobs (Forge uniquement), Pick Your Poison
  (Fabric 1.19.2 uniquement) -> certaines pieces du temple peuvent utiliser des blocs/pieges de ces mods si presents,
  aucun n'est requis. Supplementaries est installe sur ce pack. [m]

## Config serveur
- `disableVanillaJungleTemples = true` : temples vanilla desactives. [c]

## Compat
- Prevu compatible YUNG's Better Ocean Monuments, YUNG's Better Nether Fortresses (les deux presents dans le pack), YUNG's Extras. [m]
- Supplementaries (installe) : pieces speciales possibles dans le temple, feature optionnelle. [m]
