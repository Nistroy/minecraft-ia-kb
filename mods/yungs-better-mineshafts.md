---
slug: yungs-better-mineshafts
nom: YUNG's Better Mineshafts
namespaces: [bettermineshafts]
version: 1.21.1-Fabric-5.1.1
cote: S
resume: "Mineshafts abandonnes refaits en reseaux de tunnels varies, 13 variantes de biome, ateliers abandonnes, gisements de minerai"
sources:
  m: https://modrinth.com/mod/yungs-better-mineshafts
  g: https://github.com/YUNG-GANG/YUNGs-Better-Mineshafts
  j: jar YungsBetterMineshafts-1.21.1-Fabric-5.1.1.jar
  c: config bettermineshafts-fabric-1_21.toml
verifie: 2026-09-13
---

Pas de traduction FR dans le jar (en_us seulement). `client_side: unsupported`, `server_side: required`. [j,m]

## Ajoute
- 13 variantes de biome (ids `bettermineshafts:mineshaft_<biome>`) : acacia, desert, dripstone, ice, jungle, lush,
  mesa, mushroom (rare), oak, overgrown, red_desert, spruce, spruce_snowy. [j,m]
- Ateliers abandonnes (frequents), caves d'ateliers (moins frequentes), avant-postes de mineurs abandonnes (rares),
  ouvertures en surface (tres rares). [m]
- Loot dans coffres caches dans les ateliers ou en evidence dans des minecarts. [m]
- Gisements de minerai en bout de tunnel : charbon, fer, redstone, or, lapis, emeraude, diamant (tres rare). [m]

## Config serveur
- `disableVanillaMineshafts = true` : mineshafts vanilla desactives, remplaces par les Better Mineshafts. [c]
- Plage verticale : `minY = -55`, `maxY = 30`. [c]
- Taux de spawn ajustables : ores (`enabled = true`, poids cobble 50 / coal 20 / iron 9 / redstone 7 / gold 7 /
  lapis 3 / emerald 3 / diamond 1), lanternes/torches/toiles d'araignee, minecarts coffre/TNT, salle villageois zombie
  (`zombieVillagerRoomSpawnChance = 2`) — valeurs par defaut du mod, non modifiees sur ce serveur. [c]

## Compat
- Prevu compatible YUNG's Better Strongholds/Dungeons (les deux presents dans le pack), YUNG's Extras/Bridges. [m]
