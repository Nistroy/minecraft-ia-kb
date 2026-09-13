---
slug: travelersbackpack
nom: Traveler's Backpack
namespaces: [travelersbackpack]
version: 1.21.1-10.1.39
cote: S+C
resume: Sacs à dos équipables 5 tiers + upgrades (four, aimant, réservoirs...), +45 skins
sources:
  m: https://modrinth.com/mod/travelersbackpack
  w: https://github.com/Tiviacz1337/Travelers-Backpack/wiki
  g: https://github.com/Tiviacz1337/Travelers-Backpack
  j: jar travelersbackpack-fabric-1.21.1-10.1.39.jar
  c: config serveur travelersbackpack.json5
verifie: 2026-09-13
---

## Ajoute
- Bloc/item de base `travelersbackpack:travelers_backpack`, tiers Standard/Fer/Or/Diamant/Netherite
  (`standard`, `iron`, `gold`, `diamond`, `netherite`) [j].
- +45 skins cosmétiques (mêmes stats que le tier, ex `travelersbackpack:creeper`, `:enderman`, `:villager`,
  `:end`, `:nether`, `:cake`...) [j,m].
- Sacs de couchage par couleur de laine `travelersbackpack:<couleur>_sleeping_bag` [j].
- Upgrades (items à insérer dans le sac) : Mise à niveau de tier (fer/or/diamant/netherite), Amélioration de
  Fabrication `crafting_upgrade`, Tanks Upgrade, Furnace/Smoker/Blast Furnace Upgrade, Pickup Upgrade,
  Jukebox Upgrade, Magnet Upgrade, Void Upgrade, Feeding Upgrade, Refill Upgrade, Lantern Upgrade,
  Mise à niveau vide `blank_upgrade` (reset) [j].
- Tuyau `hose` + Buse `hose_nozzle`, Réservoir de sac à dos `backpack_tank` [j].

## Mécaniques
- Équipement : clic droit en main = ouvrir, bouton « Equip » dans le GUI = porter sur le dos ; touche B par
  défaut pour ouvrir le sac équipé [m].
- Montée en tier : Cuir (gabarit) + sac du tier visé + item de mise à niveau, sur Table de Forge [m,j].
- Void Upgrade + Pickup Upgrade combinés = filtre d'objets à jeter automatiquement à la récup [m].
- Magnet Upgrade attire les items au sol dans un rayon de 5 blocs, vérifié toutes les 10 ticks [c].
- Sac de couchage utilisable sans le déséquiper (`quickSleepingBag: true`), mais ne change pas le point de
  spawn chez nous (`enableSleepingBagSpawnPoint: false`) [c].
- Reset complet d'un sac posé au sol : Maj-clic avec la Mise à niveau vide (retombe en tier Cuir, vide items
  et upgrades autour) [j].

## Config serveur
- Sac increvable et ne disparaît jamais au sol (`invulnerableBackpack: true`) [c].
- Protection vide : pas de perte dans le vide, réapparaît flottant au-dessus du monde
  (`voidProtection: true`) [c].
- Sac déposé automatiquement à l'endroit de la mort du joueur (`backpackDeathPlace: true`, sans remplacer
  les blocs solides : `backpackForceDeathPlace: false`) [c].
- Coffres shulker interdits dans le sac (`allowShulkerBoxes: false`) [c].
- Équipement Trinkets/Accessories actif si mod présent (`backSlotIntegration: true`) [c].
- Loot naturel : les sacs peuvent apparaître dans des coffres de butin (`enableLoot: true`) et sur certains
  mobs équipés — zombie/squelette/enderman (overworld), wither squelette/piglin (nether), 0.5% de chance
  par mob (`chance: 0.005`) [c].
- Vente possible chez le Bibliothécaire villageois (`enableVillagerTrade: true`) [c].
