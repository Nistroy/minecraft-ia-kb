---
slug: trade-cycling
nom: Trade Cycling
namespaces: [trade_cycling]
version: fabric-1.21.1-1.0.20
cote: S+C
resume: Bouton/touche pour changer les trades d'un villageois n'ayant encore jamais été échangé avec
sources:
  m: https://modrinth.com/mod/trade-cycling
  g: https://github.com/henkelmax/trade-cycling
  j: jar trade-cycling-fabric-1.21.1-1.0.20.jar
verifie: 2026-09-13
---

## Mécaniques
- Reprend la fonctionnalité "cycle trades" du mod Easy Villagers, en mod indépendant [m].
- Change les trades proposés par un villageois "n'ayant pas encore été échangé avec" ("hasn't been traded before"),
  sans attendre les heures de travail ni casser/reposer le poste de travail [g].
- Activable par bouton dans l'interface de commerce (position configurable) ou par touche clavier, "Cycle Trades"
  en jeu (`key.trade_cycling.cycle_trades`) [j,g].
- Coût XP/ressources, nombre de cycles possibles, cooldown : non précisés dans la doc, à vérifier en jeu [g].
- Incompatible avec le mod Easy Villagers (`breaks: easy_villagers`), suggère le mod VisibleTraders (>=0.0.7.1) en
  complément [j].
- Pas de fichier `fr_fr` dans le jar, textes en anglais [j].
