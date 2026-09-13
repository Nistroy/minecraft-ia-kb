---
slug: leaves-be-gone
nom: Leaves Be Gone
namespaces: [leavesbegone]
version: v21.1.1-1.21.1-Fabric
cote: S
resume: Accélère la disparition naturelle des feuilles non reliées à un tronc après avoir coupé l'arbre
sources:
  m: https://modrinth.com/mod/leaves-be-gone
  g: https://github.com/Fuzss/leavesbegone
  j: jar LeavesBeGone-v21.1.1-1.21.1-Fabric.jar
  c: config serveur leavesbegone-server.toml
verifie: 2026-09-13
---

## Mécaniques
- Fait pourrir plus vite les feuilles non reliées à leur tronc (comportement vanilla accéléré, pas de nouvelle
  mécanique) [m].
- Délai de disparition chez nous : entre 5 et 20 ticks (`minimum_decay_ticks` / `maximum_decay_ticks`, valeurs par
  défaut) [c].
- Ne fait pas pourrir les feuilles d'une essence différente de celle du tronc coupé par défaut chez nous
  (`ignore_other_leave_types = false`) ; la doc précise que ça marche mal avec des arbres à feuilles mixtes (ex.
  azalea) [c].
- Conçu pour la performance et la compatibilité avec d'autres mods de bûcheronnage [m].
- Mod purement mécanique : pas de nouvel item/bloc, pas de fichier de langue dans le jar [j].
