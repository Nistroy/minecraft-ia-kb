---
slug: visual-workbench
nom: Visual Workbench
namespaces: [visualworkbench]
version: 21.1.2
cote: S+C
resume: Tweak visuel — les items posés dans un établi restent visibles/rendus par-dessus, pas de nouveau contenu
sources:
  m: https://modrinth.com/mod/visual-workbench
  g: https://github.com/Fuzss/visualworkbench
  j: jar VisualWorkbench-v21.1.2-1.21.1-Fabric.jar
  c: config serveur visualworkbench-server.toml
verifie: 2026-09-13
---

## Ajoute
- Aucun bloc/item nouveau : remplace juste le rendu de l'établi vanilla pour afficher les items posés
  dessus (mixin sur le crafting table) [j,m].
- Tag `visualworkbench:unaltered_workbenches` (établis exclus de la transformation) [j].

## Mécaniques
- Les établis vanilla existants se transforment en version « visuelle » dès qu'un joueur interagit
  avec (comportement contrôlé par la config serveur) [c].

## Config serveur
- `convert_vanilla_workbench_when_interacting = true` (défaut) — établis vanilla restants convertis
  automatiquement à l'usage [c].
