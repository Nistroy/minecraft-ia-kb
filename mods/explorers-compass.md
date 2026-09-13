---
slug: explorers-compass
nom: Boussole de l'explorateur
namespaces: [explorerscompass]
version: 1.21.1-2.6.0-fabric
cote: S+C
resume: Objet pour localiser n'importe quelle structure (vanilla ou moddée) via un GUI
sources:
  m: https://modrinth.com/mod/explorers-compass
  g: https://github.com/MattCzyr/ExplorersCompass
  j: jar ExplorersCompass-1.21.1-2.6.0-fabric.jar
  c: config serveur explorerscompass.json
verifie: 2026-09-13
---

## Ajoute
- Objet Boussole de l'explorateur `explorerscompass:explorerscompass`, se craft avec toile d'araignée +
  pierre taillée fissurée + boussole vanilla [j].

## Mécaniques
- Clic droit : ouvre un GUI pour choisir une structure ou un groupe de structures à rechercher [m].
- Maj-clic droit : réinitialise l'état de la boussole [m].
- Infos affichées en HUD pendant la recherche (structure, distance, coordonnées, statut) [m].
- Pas de structure ciblée = pointe vers le spawn du monde [m].
- Supporte toutes les structures enregistrées, vanilla et moddées [m].

## Config serveur
- Téléportation directe vers la structure trouvée activée, mais réservée créatif/op/mode triche
  (`allowTeleport: true`) [c].
- Jusqu'à 100 recherches de l'instance suivante par structure avant de forcer la plus proche
  (`maxNextSearches: 100`) [c].
- Coordonnées précises affichées en HUD, pas juste la direction (`displayCoordinates: true`) [c].
- Rayon de recherche max 10 000 blocs, jusqu'à 100 000 échantillons (`maxRadius`, `maxSamples`) [c].
- Durabilité désactivée : la boussole ne se casse jamais (`compassDurability: 0`) [c].
- Coût XP par recherche : 0 par défaut, pas de structure surtaxée (`defaultXpLevel: 0`,
  `perStructureXpLevels: {}`) [c].
- Aucune structure black-listée chez nous (`structureBlacklist: []`) [c].

## Compat
- Complémentaire de Nature's Compass (même auteur/API) : celle-ci cherche les biomes, celle-là les
  structures [m].
