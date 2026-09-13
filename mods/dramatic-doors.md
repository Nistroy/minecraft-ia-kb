---
slug: dramatic-doors
nom: Dramatic Doors
namespaces: [dramaticdoors]
version: 1.21.1-3.3.2
cote: S+C
resume: Portes 1 bloc plus courtes (short) ou 3 blocs de haut (tall), toutes essences + fer/cuivre
sources:
  m: https://modrinth.com/mod/dramatic-doors
  g: https://github.com/Kitteh6660/DramaticDoors
  j: jar DramaticDoors-NeoQuiFab-1.21.1-3.3.2.jar
  c: config serveur dramaticdoors-startup.toml
verifie: 2026-09-13
---

## Ajoute
- Short Door (porte courte, 1 bloc de haut) par essence vanilla (oak, spruce, birch, jungle, acacia,
  dark_oak, mangrove, bamboo, cherry, pale_oak, crimson, warped) : `dramaticdoors:short_<essence>_door` [j,m].
- Tall Door (porte haute, 3 blocs) mêmes essences : `dramaticdoors:tall_<essence>_door` [j,m].
- Fer et cuivre (+ tous états d'oxydation et versions cirées) en short/tall :
  `dramaticdoors:short_iron_door`, `tall_iron_door`, `short_copper_door` ... `tall_waxed_oxidized_copper_door` [j].
- Compat Aether (mod présent sur ce serveur) : Skyroot Door en short/tall
  `dramaticdoors:short_aether_skyroot_door` / `tall_aether_skyroot_door` [j].
- Autres compats (Biomes O'Plenty, Twilight Forest, Create, Caupona, Locksmith...) enregistrées
  seulement si le mod correspondant est installé (`dev_mode: false`) ; sur ce pack seul Aether est
  concerné parmi ceux listés dans le jar (à confirmer selon mods réellement chargés) [j,c].

## Mécaniques
- Fonctionnent comme des portes vanilla ; waterlogging activé par config (`waterloggable_doors: true`,
  `waterloggable_fence_gates: true`) [c].
- Porte courte = 1 bloc de haut (passe sous un plafond bas) ; porte haute = 3 blocs (laisse passer à
  cheval sans suffocation, argument annoncé par le mod) [j,m].

## Config serveur
- `waterloggable_doors` et `waterloggable_fence_gates` : true (défaut) — désactiver seulement en cas
  de conflit avec un autre mod [c].
