---
slug: macaws-bridges
nom: Macaw's Bridges
namespaces: [mcwbridges]
version: 3.1.2
cote: S+C
resume: Ponts déco par matériau (piles, escaliers, balustrades) + lanterne/torche de pont
sources:
  m: https://modrinth.com/mod/macaws-bridges
  g: https://github.com/sketchmacaw/Bridges
  j: jar mcw-bridges-3.1.2-mc1.21.1fabric.jar
verifie: 2026-09-13
---

## Ajoute
- Ponts par matériau (bois, pierre, brique, verre...) : bloc de base `<materiau>_bridge`, pile
  `<materiau>_bridge_pier`, escalier `<materiau>_bridge_stair`. Ex. `mcwbridges:bridge`,
  `mcwbridges:cobblestone_bridge`, `mcwbridges:glass_bridge`, `mcwbridges:asian_red_bridge` [j].
- Balustrades de pont par matériau : `mcwbridges:balustrade_<materiau>_bridge` (andesite, blackstone,
  bricks, cobblestone, deepslate_bricks, deepslate_tiles, diorite, end_stone_bricks, granite,
  mossy_cobblestone, mossy_stone_bricks, mud_bricks, nether_bricks, orange_sandstone, prismarine_bricks,
  sandstone, stone_bricks) [j].
- Variantes spéciales : Pont Bambou Sec `dry_bamboo_bridge` (+ pile/escalier), Pont Rondins
  `log_bridge_middle`/`log_bridge_stair`, Pont de Fer (pile/escalier seulement) `iron_bridge_pier`/
  `iron_bridge_stair` [j].
- Déco : Lanterne de Pont `mcwbridges:bridge_lantern`, Torche de Pont `mcwbridges:bridge_torch` [j].

## Mécaniques
- Blocs purement décoratifs (structure de pont), pas de mécanique redstone identifiée dans le jar [j].

## Compat
- Dépend de `fabric-api` ; nécessite Java 21 [j].
