---
slug: lootr
nom: Lootr
namespaces: [lootr]
version: 1.21.1-1.11.38.125
cote: S+C
resume: Chaque joueur a son propre butin par conteneur (coffre/tonneau/shulker/wagonnet) — plus de course au loot
sources:
  m: https://modrinth.com/mod/lootr
  w: https://github.com/noobanidus/Lootr/wiki
  g: https://github.com/noobanidus/lootr
  j: jar lootr-fabric-1.21.1-1.11.38.125.jar
  c: config serveur lootr.json
verifie: 2026-09-13
---

## Ajoute
- Blocs remplaçant les conteneurs à loot table vanilla : Coffre de Butin `lootr:lootr_chest`, Tonneau de
  Butin `lootr:lootr_barrel`, Shulker de Butin `lootr:lootr_shulker`, wagonnet `lootr:lootr_minecart`,
  pot décoré à butin, gravier/sable suspects [j].
- Trophée du Centenaire `lootr:trophy` (récompense d'accomplissement) [j].
- Cadres d'objet contenant du butin (`entity.lootr.item_frame`) [j].

## Mécaniques
- Chaque conteneur à loot table (coffre, coffre piégé, tonneau, shulker, wagonnet) devient unique par
  joueur : chacun voit/pille son propre inventaire généré, personne ne trouve un coffre déjà vidé par un
  autre [m].
- Couleur du conteneur change (or → bleu) une fois ouvert par le joueur courant [m].
- Casser un conteneur Lootr sans sneak affiche un avertissement (rappel qu'il est par-joueur) ; possible en
  sneak sauf si désactivé côté config [m].
- Ajouter Lootr à un monde existant convertit les conteneurs non encore ouverts ; les coffres déjà ouverts
  ne sont jamais convertis [m].
- Retirer le mod supprime définitivement tous les conteneurs Lootr convertis (pas de retour arrière) [m].
- Commande `/lootr custom` (op) : transforme un coffre vanilla rempli en conteneur "custom" partagé,
  même apparence qu'un coffre classique [m].

## Config serveur
- Cassage libre désactivé (`breaking.disable_break: false`, `enable_break: false`, joueurs non-op cassent
  seulement en sneak par défaut du mod) [c].
- Pas de décroissance des conteneurs chez nous : `decay.decay_all: false` et aucune table listée dans
  `decay_loot_tables` → aucun conteneur ne se détruit après ouverture [c].
- Pas de régénération du contenu : `refresh.refresh_all: false` et `refresh_loot_tables` vide → le butin
  par joueur reste figé une fois généré [c].
- Seed de génération randomisée par joueur (`seed.randomize_seed: true`) [c].
- Aucune dimension ni mod exclu (`dimension_blacklist`, `loot_modid_blacklist` vides) [c].
- Textures neuves actives côté client (`client.new_textures: true`, `vanilla_textures: false`) [c].

## Pièges
- Le coffre "à hache" du Manoir des bois vanilla n'a pas de loot table associée : jamais converti par
  Lootr [m].
- Un conteneur modé vide (juste décoratif) ou dont le contenu est généré manuellement par un autre mod
  peut ne jamais se convertir [m].
