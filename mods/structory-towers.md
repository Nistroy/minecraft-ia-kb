---
slug: structory-towers
nom: "Structory: Towers"
namespaces: [structory_towers]
version: 1.0.17
cote: S+C
resume: "Add-on Structory : 21 tours/avant-postes thématiques par biome, overworld + nether + end, pas de lang FR dans le jar"
sources:
  m: https://modrinth.com/mod/structory-towers
  w: "https://stardustlabs.miraheze.org/wiki/Structory:_Towers"
  g: https://github.com/Stardust-Labs-MC/Structory-Towers
  j: jar Structory_Towers_26.2_v1.0.17.jar
verifie: 2026-09-13
---

Add-on de Structory, fonctionne aussi seul. Pas de traduction FR ni EN dans le jar : ids bruts, descriptif seulement. `/locate structure structory_towers:<id>`. [j,m]

## Ajoute
- 21 structures (`data/structory_towers/worldgen/structure/`) réparties overworld/nether/end. [j]
- Overworld : `ocean_pillar`, `ancient_temple`, `farmer_outpost`, `engineer_tower`, `nomad_outpost`, `mirage_outpost`, `quarter_outpost`, `great_toadstool`, `taiga_outpost`, `foraging_outpost`, `wizard_tower`, `warped_greatsword`, `overgrown_mangrove`, `pillager_lookout`, `lighthouse`, `small_firetower`, `sacred_relic_temple`. [j]
- Nether : `nether/fortress_tower`, `nether/warped_outpost`, `nether/strange_outpost`. [j]
- End : `end/end_tower`. [j]
- Tag `structory_towers:any_tower` regroupe toutes les tours (utile pour cibler tout le mod, ex. dans `sparsestructures.customSpreadFactors`). [j]

## Où trouver
- Structure sets par rareté : `towers` (commun), `rare_towers`, `ultra_rare_towers`, `nether_towers`, `end_towers`. [j]
- `structory_towers:end/end_tower` génère dans l'End (seule structure du mod hors overworld/nether). [j]
