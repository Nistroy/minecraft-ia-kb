---
slug: tide
nom: Tide
namespaces: [tide]
version: 2.1.1
cote: S+C
resume: Refonte de la pêche — 102 poissons, minijeu de ferrage, cannes personnalisables, journal, caisses
sources:
  m: https://modrinth.com/mod/tide
  w: https://lightning-64.github.io/tide-wiki/
  g: https://github.com/Lightning-64/Tide-2
  j: jar tide-fabric-1.21.1-2.1.1.jar
  c: config serveur tide/tide_server.json, tide/tide_client.json
verifie: 2026-09-13
---

## Ajoute
- 102 poissons/créatures aquatiques (chaque avec item, seau et œuf d'apparition), ex. Abyss Angler,
  Alpha Fish, Amber Rockfish, Anchovy, Angelfish, Anglerfish, Aquathorn, Arapaima, Ash Perch, Bedrock Bug,
  Bedrock Tetra, Black Crappie... `tide:<id>` (compte exact = 102 œufs d'apparition, pas de trad FR) [j].
- Blocs : Table de pêche/accastillage `angling_table` (personnalisation des cannes), Présentoir à poissons
  `fish_display`, Torche méduse `jelly_torch`, Calendrier lunaire `lunar_calendar`, Radio météo
  `weather_radio`, Caisses en bois/obsidienne/purpurine `wooden_crate`/`obsidian_crate`/`purpur_crate` [j].
- Item Appât `bait`, variantes d'appât (dont `abyss_bait`), bobbers cosmétiques (pomme, améthyste,
  noir...) `<x>_bobber` [j].

## Mécaniques
- Canne : lancer en maintenant clic droit puis relâcher, attendre une touche [m].
- Minigame de ferrage à chaque prise : clic droit quand la barre est dans la zone colorée, chaque
  poisson a son propre comportement/force [m].
- Table d'accastillage `angling_table` : ajoute hameçons/lignes/bobbers à la canne, effets variés
  (prises plus faciles, chance, pêche dans la lave ou le vide) [m].
- Appâts : augmentent la vitesse de pêche ou donnent des bonus spéciaux, cumulables si différents [m].
- Journal de pêche (livre spécial) : suit les prises, records, habitats ; des notes trouvées dans les
  caisses indiquent où pêcher certains poissons [m].
- Système de données de poisson (JSON) extensible par datapack ; compatible mods tiers listés par
  l'auteur (Hybrid Aquatic, Nether Depths Upgrade, Stardew Fishing, Fishing Real, Fish of Thieves,
  Serene/Fabric/Ecliptic Seasons) [m].

## Config serveur
- `overrideVanillaRod: true` — la canne vanilla profite aussi des mécaniques Tide [c].
- `holdToCast: true` (maintenir clic pour lancer, défaut) [c].
- `rodDurabilityMultiplier: 1.0` (défaut, pas de modif durabilité) [c].
- Zones de pêche dans le vide configurées : Overworld/Nether jusqu'à -6 depuis le fond, End jusqu'à
  hauteur 50 [c].
- `enableBedrockBreakingItems: true` (objets capables de casser la bedrock activés, défaut) [c].
- `doMinigame: true`, difficulté x1.0, minijeux/fish data tiers activables séparément
  (`useThirdPartyMinigames: true`, `useThirdPartyFishData: false`) [c].
- `giveJournal: true` — le journal de pêche est donné (comportement par défaut) [c].
