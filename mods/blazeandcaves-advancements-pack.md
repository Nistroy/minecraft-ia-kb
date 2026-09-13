---
slug: blazeandcaves-advancements-pack
nom: BlazeandCave's Advancements Pack
namespaces: [blazeandcave, bc_rewards]
version: 1.17.2
cote: S
resume: datapack, environ 1200 advancements custom en 16 catégories, récompenses via fonctions
sources:
  m: https://modrinth.com/mod/blazeandcaves-advancements-pack
  w: https://bit.ly/bacap_1_20_doc
  j: datapack "BlazeandCave's Advancements Pack 1.17.2.zip"
verifie: 2026-09-13
---

- Distribué chez nous comme datapack world (`server/world/datapacks/`), pas comme mod jar : fonctionne avec
  un client vanilla, aucune installation côté joueur pour voir/valider les advancements [j].
- Côté S : Modrinth liste server_side required / client_side optional (il existe une version mod-jar avec
  extras client), mais notre installation en datapack pur ne demande rien côté client [m,j].
- Nom de fichier indique "1.17.2" (absent de `versions-testees.tsv`) mais `pack_format` interne = 48,
  compatible avec notre MC 1.21.1 [j].

## Ajoute
- 1219 fichiers advancement répartis en 16 catégories : adventure, animal, biomes, building, challenges,
  enchanting, end, farming, mining, monsters, nether, potion, redstone, statistics, technical, weaponry,
  plus la catégorie `bacap` (jalons/milestones de suivi) [j].
- Namespace advancements : `blazeandcave:<categorie>/<nom>`, ex. `blazeandcave:adventure/beethoven`
  ("Beethoven" — fabriquer un jukebox avec des planches et un diamant) [j].
- Chaque advancement peut déclencher une fonction de récompense `bc_rewards:<categorie>/<nom>` [j].

## Mécaniques
- Les advancements normales s'annoncent dans le chat par défaut (`announce_to_chat: true`) ; le nœud racine
  `blazeandcave:bacap/root` ne s'annonce pas [j].
- Chaque catégorie a une advancement "milestone" qui compte le nombre d'advancements obtenues dedans [m].
- Contenu inspiré d'achievements pré-1.12 et d'exclusivités Bedrock/Console, plus des idées originales de
  l'auteur [m].

## Pièges
- Se trouve dans `server/world/datapacks/`, pas dans `server/mods/` — ne pas chercher un jar Fabric pour
  ce "mod" [j].
