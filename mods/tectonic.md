---
slug: tectonic
nom: Tectonic
namespaces: [tectonic]
version: 3.0.28-fabric-21.1
cote: S+C
resume: "Refonte du générateur de terrain overworld (montagnes, rivières souterraines, piliers de jungle), pas de nouveau bloc/structure"
sources:
  m: https://modrinth.com/mod/tectonic
  w: https://github.com/Apollounknowndev/tectonic/wiki/Config
  g: https://github.com/Apollounknowndev/tectonic
  j: jar tectonic-3.0.28-fabric-21.1.jar
  c: config serveur tectonic.json
verifie: 2026-09-13
---

Terrain shaping only : aucun item/bloc/structure custom, aucun biome ajouté dans le jar. `client_side: optional`, `server_side: required`. [j,m]
Dépend de `apollib` et `lithostitched` (`fabric.mod.json`), compatible Terralith (namespace `data/terralith/` présent dans le jar pour intégration). [j]

## Mécaniques
- Étire le terrain vertical au-dessus du niveau de la mer (« Vertical Scale ») : doubler la valeur double la hauteur du terrain à un point donné. [j]
- Rivières souterraines : les rivières qui atteignent des chaînes de montagnes continuent sous terre, navigables en barque. [j]
- Piliers de jungle : certaines jungles génèrent des piliers pouvant dépasser 100 blocs de haut. [j]
- « Rolling Hills » : certaines plaines génèrent un relief vallonné et lisse. [j]
- « Ultrasmooth » : lissage fort du terrain (façon Tectonic v2), au prix de générations étranges/cassées dans les océans profonds et biomes venteux. [j]
- Grottes classiques (cheese/spaghetti/noodle) reconfigurables, coupure de profondeur des cavernes proche surface réglable. [j,c]

## Config serveur
- `vertical_scale: 1.125` — étirement vertical du terrain au-dessus du niveau de la mer (voir Mécaniques). [c]
- `min_y: -64`, `max_y: 320` (bornes vanilla standard). [c]
- `underground_rivers: true`, `jungle_pillars: true`, `rolling_hills: true`, `river_lanterns: true`. [c]
- `ultrasmooth: false`, `improved_jungle_pillars: false` (options avancées désactivées). [c]
- `ocean_offset: -0.8`. [c]
- `lava_tunnels: true` — rares tunnels de lave profonds en fond de monde. [c]
- `carvers_enabled: true` (grottes/ravins classiques actifs), `ore_fix: false`. [c]
