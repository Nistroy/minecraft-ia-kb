---
slug: universal-graves
nom: Universal Graves
namespaces: [universal_graves]
version: 3.4.4+1.21
cote: S
resume: Tombe/coffre de mort customisable, protection temporaire, boussole de mort, GUI /graves
sources:
  m: https://modrinth.com/mod/universal-graves
  g: https://github.com/Patbox/UniversalGraves
  j: jar graves-3.4.4+1.21.jar
  c: config serveur universal-graves/config.json
verifie: 2026-09-13
---

## Mécaniques
- À la mort, les items (et XP configurable) sont stockés dans une tombe posée au sol au lieu de se
  disperser [m].
- Boussole de mort donnée au joueur, pointe vers sa tombe (`give_death_compass: true`) [c].
- Ramassage rapide en sneak + clic droit à mains nues sur la tombe (`shift_and_use_quick_pickup`) [c].
- Clic sur la tombe ouvre un GUI listant son contenu (`enable_click_to_open_gui`) [c].
- Commande `/graves` : liste ses propres tombes ; `/graves player <joueur>` : voir les tombes d'un autre
  (perm `universal_graves.list_others`) ; `/graves modify <joueur>` : modifier les tombes d'un joueur
  (perm `universal_graves.modify`) ; `/graves reload` recharge la config (op) [m].
- Permission `universal_graves.teleport` : téléportation vers n'importe quelle tombe [m].
- Si la tombe ne peut pas se placer (zone protégée, monde interdit), les items tombent au sol normalement
  à la place [m,c].

## Où trouver
- Recherche d'un emplacement libre autour du point de mort dans un rayon de 8 blocs, avec décalages
  possibles (jusqu'à 5 tentatives, décalage max 40 blocs) si la position est bloquée [c].

## Config serveur
- Protection anti-vol : 900s (15 min) avant que d'autres joueurs puissent accéder à la tombe
  (`non_owner_protection_time`) [c].
- Auto-destruction désactivée chez nous : `self_destruction_time: -1` (la tombe ne disparaît jamais toute
  seule, contrairement au défaut usine de 1800s) [c].
- Récupération gratuite : `unlocking_cost.type: "free"` (pas de coût XP/item pour ouvrir sa tombe) [c].
- XP stocké à 100% (`experience_type: "percent_points"`, `100.0`) [c].
- Un joueur mort dans le vide ne génère pas de tombe (comportement du mod, message dédié dans les
  traductions) [j].
- Mort en PvP (tué par un autre joueur) : le mod a un message dédié « pas de tombe créée, items tombent
  au sol » (comportement distinct de la mort classique, cause exacte de la restriction non détaillée dans
  la doc dispo) [j].
- Pas de limite de tombes par joueur (`player_grave_limit: -1`) [c].

## Pièges
- Enchantements bloqués configurables pour empêcher qu'un objet enchanté spécifique finisse en tombe
  (`blocked_enchantments`, vide chez nous = aucun blocage) [c].
