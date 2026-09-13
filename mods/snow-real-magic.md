---
slug: snow-real-magic
nom: Snow! Real Magic!
namespaces: [snowrealmagic]
version: 12.2.2+fabric
cote: S+C
resume: retouche la neige vanilla (gravité, accumulation, fonte, dégâts de chute, blizzards)
sources:
  m: https://modrinth.com/mod/snow-real-magic
  g: https://github.com/Snownee/SnowRealMagic
  j: jar SnowRealMagic-1.21.1-Fabric-12.2.2.jar
  c: config serveur snowrealmagic-common.yaml
verifie: 2026-09-13
---

## Ajoute
- Blocs : Dalle Enneigée `snowrealmagic:slab`, Escalier Enneigé `snowrealmagic:stairs`, Mur Enneigé
  `snowrealmagic:wall`, Barrière Enneigée `snowrealmagic:fence`, Portillon Enneigé `snowrealmagic:fence_gate` [j].
- Gamerules : `snowrealmagic:blizzardStrength` (1~8, nombre max de couches de neige qui tombent en blizzard),
  `snowrealmagic:blizzardFrequency` (probabilité N/10000 par tick et par chunk) [j].

## Mécaniques
- Neige tombe comme le sable si gravité activée (`snowGravity`) [j,c].
- Neige qui touche l'eau en tombant peut se transformer en glace (`snowMakingIce`) [j,c].
- Accroupi + clic sur une couche de neige donne une boule de neige et consomme une couche (`sneakSnowball`) [j,c].
- Chute sur la neige réduit les dégâts de chute selon le nombre de couches (`snowReduceFallDamage`) [j,c].
- L'herbe ne redevient pas terre sous la neige si l'épaisseur >1 couche (`sustainGrassIfLayerMoreThanOne`) [j,c].
- Neige fond avec le temps si épaisseur >1 (`naturalMelting`), jamais si `snowNeverMelt` actif (désactivé
  chez nous) [j,c].
- Accumulation façon chute de neige progressive, lissée (`smoothAccumulation`) [j,c].
- Les mobs ne spawnent que si la couche de neige ne dépasse pas `mobSpawningMaxLayers` [j,c].

## Config serveur
- `snowGravity: true`, `snowMakingIce: true`, `snowAlwaysReplaceable: true`, `thinnerBoundingBox: true` [c].
- `snowNeverMelt: false`, `snowReduceFallDamage: true` [c].
- `snowSpawnMaxLightLevel: 9`, `snowPersistMaxLightLevel: 11` [c].
- `mobSpawningMaxLayers: 8` [c].
- Accumulation : `maxLayers: 6`, `naturalMelting: true`, `smoothAccumulation: true`,
  `snowAndIceMeltInWarmBiomes: false`, `accumulatesDuringSnowstorm: true`, `accumulatesDuringSnowfall: false` [c].
- `snow-cover` : `replaceWorldgenFeature: true`, `placeSnowOnBlock: true`, `placeNaturally: true`,
  `restoreOriginalBlocks: false` [c].
