---
slug: macaws-windows
nom: Macaw's Windows
namespaces: [mcwwindows]
version: 2.4.2
cote: S+C
resume: Fenêtres/vitraux déco par matériau + volets, stores, rideaux, fentes d'archer, verre unidirectionnel
sources:
  m: https://modrinth.com/mod/macaws-windows
  j: jar mcw-mcwwindows-2.4.2-mc1.21.1fabric.jar
verifie: 2026-09-13
---

## Ajoute
- Fenêtres par matériau (bois, pierre, brique, métal...) : bloc simple `<materiau>_window`, variante
  `_window2`, en croix `_four_window`, en vitre `_pane_window`. Ex. `mcwwindows:planks_window`,
  `mcwwindows:bricks_window`, `mcwwindows:metal_window` [j].
- Fenêtres gothiques par brique : `mcwwindows:<materiau>_gothic` (stone_brick, end_brick, nether_brick,
  prismarine_brick, mud_brick, dark_prismarine_brick) [j].
- Fentes d'archer (arrow slit) par matériau : `mcwwindows:<materiau>_arrow_slit` (stone_brick,
  cobblestone, nether_brick, ender_brick, mud_brick, dark_prismarine_brick) [j].
- Parapets (garde-corps) par essence de bois/tronc : `mcwwindows:<bois>_log_parapet`,
  `mcwwindows:<bois>_stem_parapet` [j].
- Volets (Shutter) par essence de bois + fer : `mcwwindows:<bois>_shutter`, `mcwwindows:iron_shutter` ;
  Volets à Lamelles `louvered_shutter` [j].
- Stores (Blinds) par essence : `mcwwindows:<bois>_blinds` [j].
- Rideaux (Curtain) 16 couleurs + tringle (Curtain Rod) par essence : `mcwwindows:<couleur>_curtain`,
  `mcwwindows:<bois>_curtain_rod` (dont `golden_curtain_rod`, `metal_curtain_rod`) [j].
- Mosaïque de verre (Mosaic Glass) 16 couleurs, en bloc et en vitre : `mcwwindows:<couleur>_mosaic_glass`
  (+ `_pane`) [j].
- Verre unidirectionnel : `mcwwindows:one_way_glass` (+ `_pane`) — visible d'un seul côté [j].

## Mécaniques
- Rideaux/stores/volets/fenêtres : purement décoratifs (pas de mécanique redstone identifiée dans
  le jar) [j].

## Compat
- Dépend de `fabric-api` ; nécessite Java 21 [j].
