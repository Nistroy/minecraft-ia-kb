---
slug: farmers-delight-refabricated
nom: Farmer's Delight (Refabricated)
namespaces: [farmersdelight]
version: 1.21.1-3.3.6+refabricated
cote: S+C
resume: Expansion cuisine/agriculture — nouvelles cultures, marmite/four/planche à découper, ~90 plats
sources:
  m: https://modrinth.com/mod/farmers-delight-refabricated
  w: https://github.com/vectorwing/FarmersDelight/wiki
  g: https://github.com/MehVahdJukaar/FarmersDelightRefabricated
  j: jar FarmersDelight-1.21.1-3.3.6+refabricated.jar
  c: config serveur farmersdelight-common.json
verifie: 2026-09-13
---

## Ajoute
- Nouvelles cultures : Tomate `tomatoes` (grimpe sur corde), Chou `cabbages`, Oignon `onions`,
  Riz `rice` (pousse en eau peu profonde) + variantes sauvages (`wild_<culture>`) [j].
- Blocs de cuisine : Four `stove`, Marmite `cooking_pot`, Poêle à frire `skillet`, Planche à découper
  `cutting_board`, Terre fertile `rich_soil` (+ labourée) [j].
- Rangement/déco : Caisses de légumes (`<legume>_crate`), Panier `wooden_basket`/`bamboo_basket`,
  Armoires par essence `<bois>_cabinet`, Corde `rope` + clôture/portillon, Botte de paille `straw_bale`,
  Tatami (`tatami`/`half_tatami_mat`/`full_tatami_mat`), panneaux en toile (couleurs) [j].
- Couteaux : silex, fer, or, diamant, netherite `<materiau>_knife` — outil de découpe rapide [j].
- ~90 plats/ingrédients transformés : ragoûts (bœuf, poulet, poisson, morue), sandwiches (bacon, poulet,
  œuf), soupes (oignon, citrouille, légumes, nouilles), pâtes (bolognaise, agneau, encre de seiche),
  tartes (pomme, chocolat, citrouille), cheesecake, riz (cuit/sauté/aux champignons/rouleaux), pâté
  chinois, ratatouille, hamburger, jambon (fumé/glacé au miel), bacon, brochette, cidre, chocolat chaud,
  jus de melon, glace à la pastèque [j].

## Mécaniques
- Marmite `cooking_pot` : cuisine les plats du mod (ragoûts, soupes, pâtes…) [j].
- Planche à découper `cutting_board` : découpe rapide (viandes en tranches, légumes) avec un couteau ;
  message si outil incorrect ou item non découpable [j].
- Poêle à frire `skillet` : cuisson à la poêle, impossible sous l'eau [j].
- Tomates grimpantes : ont besoin d'une corde (bloc du tag configuré, par défaut `farmersdelight:rope`) [c].
- Terre fertile `rich_soil` : chance de boost de croissance des cultures (20% par défaut) [c].

## Config serveur
- `enableFarmerFDTrades` / `enableWanderingTraderFDTrades: true` — villageois fermiers et marchands
  ambulants proposent des échanges Farmer's Delight [c].
- `richSoilBoostChance: 0.2` (défaut) [c].
- `cuttingBoardFortuneBonus: 0.1` (défaut) [c].
- `generateFDChestLoot`, `generateVillageCompostHeaps`, `generateFDCropsOnVillageFarms: true` — loot et
  cultures du mod apparaissent dans les villages/coffres générés [c].
- `enableVanillaSoupExtraEffects` et `enableRabbitStewBuff: true` — les soupes vanilla ont aussi les
  effets bonus du mod [c].
- `enablePumpkinPieSneakToPlace: false` — pas besoin de s'accroupir pour poser la tarte à la citrouille [c].
