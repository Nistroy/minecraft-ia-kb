---
slug: yungs-better-witch-huts
nom: YUNG's Better Witch Huts
namespaces: [betterwitchhuts]
version: 1.21.1-Fabric-4.1.1
cote: S
resume: "Nouvelles cabanes de sorciere (variantes) + cercle de sorciere, loot ameliore, via YUNG's API"
sources:
  m: https://modrinth.com/mod/yungs-better-witch-huts
  g: https://github.com/YUNG-GANG/YUNGs-Better-Witch-Huts
  j: jar YungsBetterWitchHuts-1.21.1-Fabric-4.1.1.jar
  c: config betterwitchhuts-fabric-1_21.toml
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us, ru_ru, uk_ua). `client_side: unsupported`, `server_side: required`. [j,m]
Depend de `yungsapi >= 1.21.1-Fabric-5.1.2`, installe (`YungsApi-1.21.1-Fabric-5.1.8.jar`). [j]

## Ajoute
- `betterwitchhuts:witch_hut` : plusieurs variantes de cabane remplacent la witch hut vanilla, meilleur design et loot plus pertinent. [j,m]
- `betterwitchhuts:witch_circle` : nouvelle structure, cercle de sorciere. [j]
- Chaudrons a brasser (brewing stands) des cabanes peuvent contenir des items indiquant des recettes de potions vanilla. [m]

## Mecaniques
- `disableVanillaWitchHuts` : empêche les witch huts vanilla de spawner. [m,c]
- Les deux structures forcent le spawn d'1 `minecraft:witch` (monster) et 1 `minecraft:cat` (creature) sur leur emprise (`spawn_overrides`, bounding_box `piece`). [j]
- `witch_hut` : jigsaw `yungsapi:yung_jigsaw`, pool `betterwitchhuts:starts`, taille 20, place au niveau du sol (`WORLD_SURFACE_WG`). [j]
- `witch_circle` : meme systeme, pool `betterwitchhuts:circles`, taille 20. [j]

## Où trouver
- `/locate structure betterwitchhuts:witch_hut` (cabane) ; `betterwitchhuts:witch_circle` (cercle, id direct, pas de commande d'aide dans le jar). [j]
- Placement cabane : `spacing` 30, `separation` 8 chunks (random_spread). Cercle : `spacing` 40, `separation` 10. [j]
- Loot des coffres de cabane : table `data/betterwitchhuts/loot_table/chests/hut_0.json`. [j]

## Config serveur
- `disableVanillaWitchHuts = true` : witch huts vanilla desactivees sur notre serveur. [c]

## Compat
- Prevu compatible avec YUNG's Better Mineshafts (installe), YUNG's Better Strongholds (installe), YUNG's Better Desert Temples (installe), YUNG's Better Ocean Monuments (installe), YUNG's Extras, YUNG's Bridges (non installes). [m]
