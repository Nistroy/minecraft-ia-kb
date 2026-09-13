---
slug: ribbits
nom: Ribbits
namespaces: [ribbits]
version: 1.21.1-Fabric-4.1.6
cote: S+C
resume: Villages de grenouilles-villageois dans les marais, commerce, musique, entretien des cultures
sources:
  m: https://modrinth.com/mod/ribbits
  g: https://github.com/yungnickyoung/Ribbits
  j: jar Ribbits-1.21.1-Fabric-4.1.6.jar
  c: config serveur ribbits-fabric-1_21_1.toml
verifie: 2026-09-13
---

## Ajoute
Pas de traduction FR dans le jar : noms en jeu anglais (glose FR entre parenthèses). [j]
- Mob Ribbit `ribbits:ribbit` (villageois-grenouille), 5 métiers d'après les œufs d'apparition : Fisherman
  (pêcheur), Gardener (jardinier), Merchant (marchand), Sorcerer (sorcier), Nitwit (idiot du village) —
  œufs `ribbits:ribbit_<métier>_spawn_egg` [j].
- Structure Village Ribbit `ribbits:ribbit_village` [j].
- Blocs déco : Brown Toadstool Block `brown_toadstool`, Red Toadstool Block `red_toadstool`, Toadstool
  `toadstool`, Toadstool Stem `toadstool_stem`, Lush Lily Pad `giant_lilypad`, Swamp Daisy `swamp_daisy`,
  Swamp Lantern `swamp_lantern`, Umbrella Leaf `umbrella_leaf`, Mossy Oak Planks/Stairs/Slab/Fence/Fence
  Gate/Door (`mossy_oak_*`) [j].
- Item Maraca `ribbits:maraca` [j].

## Mécaniques
- Marchand + pêcheur ribbit : commerce contre objets divers, dont blocs plantes du mod et maracas [m].
- Sorcier ribbit : lance occasionnellement des sorts qui buffent le joueur [m].
- Jardinier ribbit : arrose les cultures automatiquement [m].
- Ribbits jouent de la musique en groupe (maraca), le joueur peut se joindre [m].
- Rentrent chez eux la nuit ; clic droit avec de l'améthyste sur un ribbit = reset son point de
  rattachement (« home ») sur sa position actuelle, pour les reloger [m].

## Où trouver
- Village Ribbit : biome marais (`minecraft:swamp`, + tags forge/c compat) [j].

## Config serveur
- `prideFlagAllYear = false` — décoration cosmétique désactivée hors période dédiée (réglage par défaut) [c].
