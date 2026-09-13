---
slug: critters-and-companions
nom: Critters and Companions
namespaces: [crittersandcompanions]
version: 2.7.0
cote: S+C
resume: Petites créatures vanilla-style (loutre, panda roux, poulpe Dumbo, insectes...) + grappin et laisse en soie
sources:
  m: https://modrinth.com/mod/critters-and-companions
  g: https://github.com/bonsaistudi0s/CrittersAndCompanions
  j: jar crittersandcompanions-fabric-1.21.1-2.7.0.jar
  c: config serveur crittersandcompanions-common.json5
verifie: 2026-09-13
---

## Ajoute
- Mobs (nom FR trouvé) : Loutre `otter`, Araignée sauteuse `jumping_spider`, Poisson koï `koi_fish`,
  Libellule `dragonfly`, Lapin de mer `sea_bunny`, Shima enaga `shima_enaga` (petit oiseau blanc),
  Furet `ferret`, Poulpe Dumbo `dumbo_octopus`, Panda roux `red_panda`, Phasme feuille `leaf_insect`,
  tous `crittersandcompanions:<id>` [j].
- Mobs sans nom FR dans le jar → nom anglais en jeu (traduction entre parenthèses) : Ladybug `ladybug`
  (coccinelle), Stag Beetle `stag_beetle` (lucane), Roly-Poly `roly_poly` (cloporte), Snail `snail` (escargot),
  Stick Bug `stick_bug` (phasme), Acorn Weevil `weevil` (charançon) [j].
- Items : Grappin `grappling_hook`, Laisse en soie `silk_lead`, Soie `silk`, Perle `pearl` + colliers de
  perles (3 niveaux), Aile de libellule `dragonfly_wing`, Palourde `clam`, armures de libellule
  (fer/or/diamant) `<tier>_dragonfly_armor`, Fiole de gélatine de lapin de mer `sea_bunny_slime_bottle`,
  seaux pour poulpe Dumbo / poisson koï / lapin de mer [j].
- Blocs : Cocon de soie `silk_cocoon`, Bloc de gélatine de lapin de mer `sea_bunny_slime_block` [j].

## Mécaniques
- Grappin `grappling_hook` : lance/tire le joueur (portée et vitesse réglables en config, durabilité
  activable) [j,c].
- Collier de perles : buff nage + réduit l'agressivité/portée de détection des noyés et gardiens
  (valeurs par défaut : +0.2 vitesse nage, -0.1 portée noyé/gardien) [c].
- Laisse en soie `silk_lead` : alternative à la laisse vanilla (dépend de la soie du mod) [j].

## Où trouver
- Otter, koi_fish : rivières (`#c:is_river`) [c].
- Dragonfly : rivières/marais/biomes luxuriants [c].
- Sea_bunny, dumbo_octopus : océans (chaud/tiède/normal/profond), plus fréquent en océan chaud [c].
- Ferret : forêts et plaines [c].
- Red_panda, jumping_spider, leaf_insect : jungles (+ forêts/luxuriants pour spider/leaf_insect) [c].
- Shima_enaga : biomes enneigés [c].
- Insectes (ladybug, stag_beetle, roly_poly, snail, stick_bug, weevil) : forêts, biomes luxuriants,
  marais selon l'espèce [c].

## Config serveur
- `prevent_monster_spawns_in_lush_caves: false` — grottes luxuriantes gardent leurs monstres normaux [c].
- Toutes les tables de spawn sont aux valeurs par défaut du mod (aucune désactivation constatée) [c].
