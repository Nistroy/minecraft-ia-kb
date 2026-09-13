---
slug: yungs-better-ocean-monuments
nom: YUNG's Better Ocean Monuments
namespaces: [betteroceanmonuments]
version: 1.21.1-Fabric-4.1.2
cote: S
resume: "Monument oceanique plus grand, layout aleatoire, meilleur loot dont Tridents et Coeur de la Mer"
sources:
  m: https://modrinth.com/mod/yungs-better-ocean-monuments
  g: https://github.com/YUNG-GANG/YUNGs-Better-Ocean-Monuments
  j: jar YungsBetterOceanMonuments-1.21.1-Fabric-4.1.2.jar
  c: config betteroceanmonuments-fabric-1_21.toml
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us seulement). `/locate structure betteroceanmonuments:ocean_monument`.
`client_side: unsupported`, `server_side: required`. [j,m]

## Ajoute
- 1 structure `betteroceanmonuments:ocean_monument`, remplace le monument oceanique vanilla, beaucoup plus grand,
  layout completement aleatoire (pas un plan fixe comme vanilla). [j,m]
- Meilleur loot : Tridents et Coeur de la Mer (Heart of the Sea) cites explicitement. [m]
- Loot table dediee `chests/upper_side_chamber`. [j]

## Config serveur
- `disableVanillaMonuments = true` : monuments vanilla desactives. [c]

## Compat
- Prevu compatible YUNG's Better Desert Temples/Mineshafts/Strongholds (presents dans le pack), YUNG's Extras/Bridges. [m]
