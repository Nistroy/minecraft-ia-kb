---
slug: rightclickharvest
nom: Right Click Harvest
namespaces: [rightclickharvest]
version: 4.6.1+1.21.1
cote: S
resume: Récolter les cultures (vanilla + quasi tout mod) au clic droit, replante auto
sources:
  m: https://modrinth.com/mod/rightclickharvest
  g: https://github.com/JamCoreModding/RightClickHarvest
  j: jar rightclickharvest-fabric-4.6.1+1.21.1.jar
  c: config serveur rightclickharvest.json5
verifie: 2026-09-13
---

## Mécaniques
- Clic droit sur une culture mûre = récolte + replantation auto des graines, marche sur blé, carottes,
  cacao, canne à sucre, cactus et la plupart des cultures moddées sans config spécifique [m].
- Houe enchantée Fortune = meilleur rendement à la récolte [m].
- `harvestInRadius` (actif par défaut chez nous et par défaut du mod) : une houe de tier supérieur
  récolte plusieurs blocs dans un rayon autour du point visé [j,c].
- `requireHoe` (désactivé par défaut chez nous, = défaut du mod) : si activé, certaines cultures
  (ex. blé, carottes) ne seraient récoltables au clic droit qu'avec une houe en main [c].
- Pas de gestion faim/XP par défaut (`hungerLevel: NONE`, `experienceType: NONE`) [c].

## Config serveur
- Config alignée sur les valeurs par défaut du mod : `requireHoe: false`, `harvestInRadius: true`,
  `hungerLevel: NONE`, `experienceType: NONE` [c].
