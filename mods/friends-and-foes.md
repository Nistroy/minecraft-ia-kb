---
slug: friends-and-foes
nom: Friends&Foes
namespaces: [friendsandfoes]
version: fabric-4.0.27+mc1.21.1
cote: S+C
resume: Mobs recalés du mob vote (crabe, moobloom, golems cuivre/tuf, wildfire...) + structures dédiées
sources:
  m: https://modrinth.com/mod/friends-and-foes
  w: https://github.com/Faboslav/friends-and-foes/wiki
  g: https://github.com/Faboslav/friends-and-foes
  j: jar friendsandfoes-fabric-4.0.27+mc1.21.1.jar
  c: config serveur friendsandfoes.json
verifie: 2026-09-13
---

## Ajoute
- Mobs : Golem de cuivre `friendsandfoes:copper_golem`, Crabe `friendsandfoes:crab`, Glare `friendsandfoes:glare`,
  Cryologiste `friendsandfoes:iceologer`, Lumimeuh `friendsandfoes:moobloom`, Fripouille `friendsandfoes:rascal`,
  Mordeur `friendsandfoes:mauler`, Golem de Tuf `friendsandfoes:tuff_golem`, Wildfire `friendsandfoes:wildfire`,
  Illusion de Joueur `friendsandfoes:player_illusion` [j].
- Remplace/complète le vanilla Illusionneur `friendsandfoes:illusioner`, config peut le désactiver (voir Config) [j,c].
- Blocs : ruches par essence (`friendsandfoes:<bois>_beehive`), boutons de cuivre + variantes oxydation
  (`friendsandfoes:copper_button` etc.), paratonnerres oxydables (`friendsandfoes:*_lightning_rod`),
  Bouton d'Or `friendsandfoes:buttercup` + pot [j].
- Items : Pince de crabe `friendsandfoes:crab_claw`, Totem de Gel `friendsandfoes:totem_of_freezing`,
  Totem d'Illusion `friendsandfoes:totem_of_illusion`, Couronne du Wildfire `friendsandfoes:wildfire_crown`
  + fragment `friendsandfoes:wildfire_crown_fragment` [j].
- Structures : Citadelle (Nether) `friendsandfoes:citadel`, Cabane du cryologiste (biomes enneigés)
  `friendsandfoes:iceologer_cabin`, Cabane + terrain d'entraînement de l'illusionneur (taïgas)
  `friendsandfoes:illusioner_shack` / `illusioner_training_grounds` [j].

## Mécaniques
- Golems de cuivre : peuvent apparaître en village (structure dédiée), en cité antique, en chambre d'épreuves ;
  s'oxydent comme le cuivre, se cirent [j,c].
- Crabe : donne pince de crabe (loot), potion de portée liée (durée configurée serveur 3600 ticks) [c].
- Fripouille : peut donner une récompense en bundle (`rascalGiveRewardInBundle`) [c].
- Golem de tuf : peut apparaître en stronghold [j,c].
- Wildfire : lié à la structure Citadelle dans le Nether [j].

## Où trouver
- Citadelle : biomes Nether (`#minecraft:is_nether`) [j].
- Cabane du cryologiste : biomes de la collection "snowy" du mod [j].
- Cabane/terrain de l'illusionneur : biomes de la collection "taigas" du mod [j].

## Config serveur
- `enableIllusioner: false` — l'illusionneur custom du mod est désactivé sur notre serveur, mais
  `replaceVanillaIllusioner: true` et `enableIllusionerSpawn/InRaids: true` restent actifs [c].
- Spawns activés par défaut pour crabe, glare (griefing activé), cryologiste, mordeur (désert/badlands/savane),
  lumimeuh, fripouille, golem de tuf, wildfire, golem de cuivre [c].
- Structures dédiées toutes activées (village apiculteur, workstation golem cuivre, cabane cryologiste,
  cabane+terrain illusionneur, citadelle) [c].
