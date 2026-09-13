---
slug: yungs-better-nether-fortresses
nom: YUNG's Better Nether Fortresses
namespaces: [betterfortresses]
version: 1.21.1-Fabric-3.1.5
cote: S
resume: "Fortresse du Nether agrandie : reseaux de ponts, le Keep, les Lava Halls en profondeur"
sources:
  m: https://modrinth.com/mod/yungs-better-nether-fortresses
  g: https://github.com/YUNG-GANG/YUNGs-Better-Fortresses
  j: jar YungsBetterNetherFortresses-1.21.1-Fabric-3.1.5.jar
  c: config betterfortresses-fabric-1_21.toml + betterfortresses/fabric-1_21/
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us seulement). `/locate structure betterfortresses:fortress`.
`client_side: unsupported`, `server_side: required`. [j,m]

## Ajoute
- 1 structure `betterfortresses:fortress`, remplace la forteresse du Nether vanilla, plus grande et plus complexe. [j,m]
- 3 parties : reseaux de ponts, le "Keep", les "Lava Halls" qui s'etendent en profondeur sous terre. [m]
- Loot tables dediees : beacon, extra, hall, keep, obsidian, puzzle, quarters, storage, worship (par salle). [j]
- Compat optionnelle Create citee par le mod (1.19.2+ uniquement) : certaines pieces peuvent utiliser des elements
  Create si le mod est present, non requis ; Create n'est pas installe sur ce pack. [m]

## Config serveur
- `disableVanillaFortresses = true` : forteresses vanilla desactivees, seules les Better Fortresses generent. [c]

## Compat
- Prevu compatible YUNG's Better Ocean Monuments, YUNG's Better Witch Huts (presents dans le pack), YUNG's Extras. [m]
- Cite Infernal Expansion, Better Nether et autres mods de biomes Nether comme compatibles ; Apocalyptic Fortress
  (spawn a cote de la Better Fortress) et Bygone Nether (Better Fortress remplace la forteresse ameliore de Bygone
  Nether) — aucun de ces trois n'est installe sur ce pack. [m]
