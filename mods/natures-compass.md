---
slug: natures-compass
nom: Boussole de la nature
namespaces: [naturescompass]
version: 1.21.1-2.6.0-fabric
cote: S+C
resume: Objet pour localiser un biome et voir ses infos (température, hauteur, blocs de surface...)
sources:
  m: https://modrinth.com/mod/natures-compass
  g: https://github.com/MattCzyr/NaturesCompass
  j: jar NaturesCompass-1.21.1-2.6.0-fabric.jar
  c: config serveur naturescompass.json
verifie: 2026-09-13
---

## Ajoute
- Objet Boussole de la nature `naturescompass:naturescompass`, recette débloquée avec boussole vanilla +
  rondin ou gland (tag bois/saplings) [j].

## Mécaniques
- Clic droit : ouvre le GUI de sélection de biome, avec recherche et fiche d'infos (climat, température,
  pluviosité, hauteur de base, variation de hauteur, bloc de surface/profondeur) [m,j].
- Maj-clic droit : réinitialise l'état de la boussole [m].
- Pas de biome ciblé = pointe vers le spawn du monde [m].
- Supporte tous les biomes enregistrés, vanilla et moddés [m].

## Config serveur
- Téléportation vers le biome trouvé activée, réservée créatif/op/mode triche
  (`allowTeleport: true`) [c].
- Jusqu'à 25 recherches de l'instance suivante par biome (`maxNextSearches: 25`) [c].
- Coordonnées précises affichées en HUD (`displayCoordinates: true`) [c].
- Précision de recherche : rayon = taille du biome × 2500, espace d'échantillon = taille × 16
  (`radiusModifier`, `sampleSpaceModifier`) [c].
- Durabilité désactivée : la boussole ne se casse jamais (`compassDurability: 0`) [c].
- Coût XP par recherche : 0 par défaut, pas de biome surtaxé (`defaultXpLevels: 0`,
  `perBiomeXpLevels: {}`) [c].
- Aucun biome black-listé chez nous (`biomeBlacklist: []`) [c].

## Compat
- Complémentaire d'Explorer's Compass (même auteur/API) : celle-ci cherche les biomes, celle-là les
  structures [m].
