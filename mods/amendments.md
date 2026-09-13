---
slug: amendments
nom: Amendments
namespaces: [amendments]
version: 1.21-2.1.10
cote: S+C
resume: Tweaks de blocs vanilla (chaudrons, lanternes, bougies, tapis, gâteaux...), sans nouveau contenu
sources:
  m: https://modrinth.com/mod/amendments
  g: https://github.com/MehVahdJukaar/amendments
  j: jar amendments-1.21-2.1.10-fabric.jar
  c: config serveur amendments-common.json
verifie: 2026-09-13
---

## Ajoute
- Chaudron liquide `amendments:liquid_cauldron` et Chaudron à teinture `amendments:dye_cauldron` :
  variantes du chaudron vanilla, stockent d'autres liquides / teinture [j,m].
- Tapis d'Escalier `amendments:carpet_stairs` et Tapis de Dalle `amendments:carpet_slab` : tapis posé
  sur forme d'escalier/dalle [j].
- Lanterne Murale `amendments:wall_lantern` : lanterne accrochable au mur [j].
- Crochet à Outil `amendments:tool_hook` : posé sur un crochet à fil-piège (tripwire hook) [j].
- Gâteau Double `amendments:double_cake` et Gâteau Directionnel `amendments:directional_cake` [j].
- Empilement de Crânes `amendments:skull_pile` et Crâne à Bougie `amendments:candle_skull` [j].
- Pot Suspendu `amendments:hanging_pot`, Pot de Fleur Suspendu `amendments:hanging_flower_pot` [j].
- Bannière de Plafond `amendments:ceiling_banner` [j].
- Item Charge de Dragon `amendments:dragon_charge`, Bouteille de Teinture `amendments:dye_bottle` [j].

## Mécaniques
- Chaudron amélioré : peut mélanger des potions (dans le chaudron) et teindre de l'eau ; potions
  "inversées" définies par config (ex. Force ↔ Faiblesse, Vitesse ↔ Lenteur) ; craft à la main et
  craft en monde ("in_world_crafting") activés [c].
- Lutrin (lectern) : interface améliorée pour lire les livres [c].
- Cloche : peut être actionnée en chaîne sur plusieurs cloches reliées, portée de chaîne 16 blocs [c].
- Bougies sur crânes/empilements : plusieurs bougies possibles sur un même support (`multiple_candles`) [c].
- Boule de feu / charge de dragon : subit la gravité, cooldown de lancer 10 ticks, non déviable
  (`deflectable: false`) [c].
- Torche : peut mettre le feu si portée/utilisée (`torch_fire`), durée 2s, désactivé en main secondaire [c].
- Nénuphars améliorés (`better_lilypads`) et tapis posables sur escaliers/dalles [c].

## Config serveur
- `potions_mixing: ON`, limite 8 mélanges par chaudron, 4 recettes de teinture et 2 de potion par couche [c].
- `falling_lanterns: ON` — les lanternes peuvent tomber si non supportées [c].
- `misc.dye_blocks: false` — teindre des blocs directement désactivé sur ce serveur [c].
- `consistent_lava_layers: false` [c].

## Compat
- Fusion d'anciens mods de l'auteur (Carpeted Stairs, Better Lilypads, Better Jukeboxes, features
  Supplementaries) : plus besoin de les installer séparément [m].
- Dépend de `moonlight` (>=1.21-3.1.0c) comme Supplementaries ; nécessite Supplementaries à jour côté
  compat croisée (assets `supplementaries` référencés dans le jar) [j].
