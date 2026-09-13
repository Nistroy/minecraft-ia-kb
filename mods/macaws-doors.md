---
slug: macaws-doors
nom: Macaw's Doors
namespaces: [mcwdoors]
version: 1.1.5
cote: S+C
resume: Portes déco par essence x ~20 styles (grange, japonaise, moderne...) + herses, porte de garage
sources:
  m: https://modrinth.com/mod/macaws-doors
  g: https://github.com/sketchmacaw/MacawsDoors
  j: jar mcw-doors-1.1.5-mc1.21.1fabric.jar
verifie: 2026-09-13
---

## Ajoute
- Portes par essence de bois (oak, spruce, birch, jungle, acacia, dark_oak, mangrove, cherry, bamboo,
  crimson, warped, pale_oak) déclinées en ~20 styles : barn (grange), bark_glass, beach, classic,
  cottage (chalet), four_panel, glass, japanese/japanese2 (shoji), modern, mystic, nether, paper,
  stable/stable_head (écurie), swamp (marais), tropical, waffle (gaufrée), western, whispering
  (pâleuse). Id type `mcwdoors:<essence>_<style>_door`, ex. `mcwdoors:oak_barn_door`,
  `mcwdoors:oak_japanese_door` [j].
- Portes métal/spéciales : `metal_door`, `metal_hospital_door`, `metal_reinforced_door`,
  `metal_warning_door`, `metal_windowed_door`, `jail_door` (porte de prison),
  `sliding_glass_door` (coulissante en verre), `store_door` (porte de magasin) [j].
- Portes de garage (4 couleurs) : `garage_white_door`, `garage_black_door`, `garage_gray_door`,
  `garage_silver_door` [j].
- Herses : `wooden_portcullis` (bois), `iron_portcullis` (fer) [j].

## Mécaniques
- Fonctionnent comme des portes vanilla (ouverture au clic/redstone), pas de mécanique additionnelle
  identifiée dans le jar [j].

## Compat
- Dépend de `fabric-api` ; nécessite Java 21 [j].
