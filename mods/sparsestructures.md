---
slug: sparsestructures
nom: Sparse Structures
namespaces: []
version: "3.0"
cote: S
resume: "Espace toutes les structures (vanilla + modées + datapacks) selon un facteur configurable, aucun ajout de contenu"
sources:
  m: https://modrinth.com/mod/sparsestructures
  g: https://github.com/MaxenceDC/sparsestructures
  j: jar sparsestructures-fabric-1.21.1-3.0.jar
  c: config serveur sparsestructures.json5
verifie: 2026-09-13
---

Mod technique pur : pas de bloc/item/structure/biome ajouté (aucun `data/<ns>/` dans le jar). `client_side: unsupported`, `server_side: required` — rien à installer côté joueur. [j,m]
Nécessite un redémarrage complet du serveur pour appliquer un changement de config. [c]

## Mécaniques
- `spreadFactor` = facteur d'espacement global appliqué à toutes les structures (vanilla, mods, datapacks) : >1 = plus rares/espacées, <1 = plus communes, 1 = inchangé, 0 = désactive toutes les structures. [c]
- `customSpreadFactors` : liste de surcharges par structure ou par structure_set (`namespace:id`), remplace le facteur global pour cette entrée. [c]
- `idBasedSalt: true` : donne un sel unique par structure_set (hashé depuis son id) pour éviter les chevauchements quand plusieurs mods/datapacks de structures utilisent le même sel. [c]
- Commande `/dumpstructuresets` : liste tous les structure sets actifs sur le serveur (pratique pour trouver l'id à cibler dans `customSpreadFactors`). [c]

## Config serveur
- `spreadFactor: 2` — toutes les structures du pack sont ~2x plus espacées/rares que leur défaut. [c]
- `idBasedSalt: true` — actif (recommandé quand plusieurs mods de structures cohabitent, ex. Terralith/Structory/When Dungeons Arise). [c]
- `customSpreadFactors` : seule entrée = `minecraft:mansion` avec `factor: 2`, exemple activé par défaut dans le template du mod (double la rareté du manoir en plus du `spreadFactor` global). [c]
