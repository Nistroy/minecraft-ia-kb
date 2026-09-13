---
slug: waystones
nom: Waystones
namespaces: [waystones]
version: 21.1.44+fabric-1.21.1
cote: S+C
resume: Blocs de téléportation (waystones) + parchemins/pierres de warp, alternative à /home et /warp
sources:
  m: https://modrinth.com/mod/waystones
  w: https://mods.twelveiterations.com/minecraft/waystones
  g: https://github.com/TwelveIterations/Waystones
  j: jar waystones-fabric-1.21.1-21.1.44.jar
  c: config serveur waystones-common.toml
verifie: 2026-09-13
---

## Ajoute
- Bloc Waystone `waystones:waystone` + variantes moussue/grès/blackstone/deepslate/end stone/nether/purpur/
  prismarine/boue (`mossy_`, `sandy_`, `blackstone_`, `deepslate_`, `end_stone_`, `red_nether_bricks_`,
  `purpur_`, `prismarine_`, `mud_bricks_waystone`) [j].
- Plaque de téléportation `waystones:warp_plate`, Sharestones et Portstones (1 jeu par couleur de laine,
  `waystones:<couleur>_sharestone` / `_portstone`) [j].
- Objets : Parchemin de téléportation `warp_scroll` (+ version liée `warp_scroll_bound`), Parchemin de retour
  `return_scroll`, Pierre de téléportation `warp_stone`, Parchemin lié `bound_scroll`, Poudre de téléportation
  `warp_dust`, Parchemin vierge `blank_scroll` [j].
- Objets sans traduction FR dans le jar (nom EN) : Portal Scroll `portal_scroll`, Dormant Shard `dormant_shard`,
  Attuned Shard `attuned_shard`, Crumbling Attuned Shard `crumbling_attuned_shard`, Deepslate Shard
  `deepslate_shard`, Twinbound Feather `twinbound_feather`, Epitaph `epitaph`, bloc Warp Portal `warp_portal`,
  bloc Fleeting Memorial `fleeting_memorial` — tous craftables (recette dans le jar) [j].

## Mécaniques
- Waystone une fois activée = destination réutilisable via Warp Scroll, Warp Stone rechargeable ou saut
  d'une waystone à l'autre [m].
- `warp_dust` : ender pearl + éclat d'améthyste ; `dormant_shard` : 2x warp_dust + silex ; `portal_scroll` :
  ender pearl + encre + papier + éclat d'améthyste ; `epitaph` : éclat d'améthyste + deepslate + pépite d'or ;
  `twinbound_feather` : plume + éclat d'améthyste + pépite d'or + encre [j].
- Waystone globale = accessible à tous les joueurs (activation en creatif ou si autorisé en config) [m,c].
- Bouton téléportation dans l'inventaire configurable (off par défaut chez nous, `inventoryButton = ""`) [c].

## Où trouver
- Génération naturelle dans le monde : tous les 25 chunks environ (`chunksBetweenWildWaystones = 25`), style
  visuel selon biome (`wildWaystoneStyle = "BIOME"`), autorisée overworld/nether/end [c].
- Apparition dans les villages en mode régulier (`spawnInVillages = "REGULAR"`, pas garanti sur chaque village) [c].

## Config serveur
- Coût XP (`warpRequirements`) : même dimension = 0,01 × distance ; changement de dimension = +27 ; gratuit
  depuis une plaque de téléportation, vers une waystone globale ou un Fleeting Memorial ; min 0, max 27 [c].
- Recharge bouton d'inventaire : 300 ticks (15s) si utilisé [c].
- Mobs en laisse : téléportés avec le joueur (`transportLeashed = "ENABLED"`), sauf le Wither (deny-list) ;
  animaux proches (non laissés) NON téléportés (`transportPets = "DISABLED"`) [c].
- Durabilité des pierres de téléportation activée, coûts XP activés, cooldowns activés (défauts du mod) [c].

## Pièges
- Message « touch waystone, nothing happens » (clic droit waystone-à-waystone si désactivé) reste en
  anglais dans le fichier de traduction FR du jar [j].
- Nécessite le mod Balm en dépendance (déjà présent, lib) [j].
