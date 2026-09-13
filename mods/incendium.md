---
slug: incendium
nom: Incendium
namespaces: [incendium]
version: 5.4.4
cote: S
resume: Refonte du Nether (8 biomes, structures, boss Hovering Inferno, armes uniques)
sources:
  m: https://modrinth.com/mod/incendium
  w: https://stardustlabs.miraheze.org/wiki/Incendium
  g: https://github.com/Stardust-Labs-MC/Incendium
  j: jar Incendium_1.21.x_v5.4.4.jar
verifie: 2026-09-13
---

## Ajoute
- Datapack de refonte du Nether : aucun bloc/item propre au sens vanilla, tout passe par recettes/loot/fonctions (pas de traductions dans le jar, les noms viennent de `fallback` intégré aux loot tables). [j]
- Noms FR ci-dessous = traductions descriptives, pas des noms en jeu (datapack sans fichier de langue) ; chercher par id : `/locate biome incendium:<id>`, `/locate structure incendium:<id>`. [j]
- 8 biomes Nether : Landes de cendres (`ash_barrens`), Dunes infernales (`infernal_dunes`), Forêt inversée (`inverted_forest`), Plaines de quartz (`quartz_flats`), Tas toxique (`toxic_heap`), Deltas volcaniques (`volcanic_deltas`), Vallée pleureuse (`weeping_valley`), Forêt flétrie (`withered_forest`). [j]
- Structures : Tour abandonnée, Château interdit (`forbidden_castle`), Autel infernal (`infernal_altar`), Réacteur du Nether (`nether_reactor`), Village Piglin (`piglin_village`), Pipeline, Cuisine de quartz, Labo en ruine, Sanctuaire (`sanctum`). [j]
- Boss : Hovering Inferno - combat scripté à phases (fonctions `incendium:hovering_inferno/*`), invoqué via un autel rituel, bouclier tournant, invoque blazes/vex, plusieurs types de sorts (lasers, boules de feu, feux d'artifice). [j]
- Armes/objets uniques ("artefacts", base vanilla + nom/lore custom) : Ragnarok (arc, foudre en tirant), Trailblazer (arc, flèches spectrales laissent une traînée de flammes), Firestorm (arbalète, flèches spectrales → attaque foudre), Scarlet Dagger (épée en netherite, draine la vie), Infernal Wings (élytres forgées des débris du Hovering Inferno), boucliers Necrotic/Prismatic/Radiation, Elixir of Undying (potion), Hazmat Suit (armure cuir custom). [j]

## Compat
- `client_side: optional` côté Modrinth : le monde généré différera visuellement sans le mod côté client. [m]
