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
- Mob villageois-grenouille `ribbits:ribbit` (pas de trad FR dans le jar), avec métiers : pêcheur,
  jardinier, marchand, idiot du village (nitwit), sorcier — chacun avec son œuf d'apparition
  `ribbits:ribbit_<metier>_spawn_egg` [j].
- Structure Village Ribbit `ribbits:ribbit_village` [j].
- Blocs déco : Tabouret/bloc champignon marron et rouge (`brown_toadstool`/`red_toadstool`),
  Toadstool + tige, Nénuphar géant `giant_lilypad`, Marguerite des marais `swamp_daisy`,
  Lanterne des marais `swamp_lantern`, Feuille-parapluie `umbrella_leaf`, planches/porte/clôture/dalle/
  escalier en chêne moussu `mossy_oak_*` [j].
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
