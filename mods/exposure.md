---
slug: exposure
nom: Exposure
namespaces: [exposure]
version: 1.9.18
cote: S+C
resume: appareil photo survie, pellicules à développer en chambre claire, photos encadrées/projetées
sources:
  m: https://modrinth.com/mod/exposure
  w: https://moddedmc.wiki/en/project/exposure/latest/docs
  g: https://github.com/mortuusars/Exposure
  j: jar exposure-fabric-1.21.1-1.9.18.jar
  c: config serveur exposure-server.toml
verifie: 2026-09-13
---

## Ajoute
- Items : Appareil photo `exposure:camera`, Film noir et blanc `exposure:black_and_white_film`, Film couleur
  `exposure:color_film`, "High-Sensitivity Black and White Film" `exposure:high_sensitivity_black_and_white_film`
  (pas de trad fr), "High-Sensitivity Color Film" `exposure:high_sensitivity_color_film` (pas de trad fr),
  Album photo `exposure:album`, "Signed Photo Album" `exposure:signed_album` (pas de trad fr),
  Photographie `exposure:photograph`, "Interplanar Projector" `exposure:interplanar_projector` (pas de trad fr) [j].
- Blocs/entités : Chambre claire `exposure:lightroom`, "Camera Stand" `exposure:camera_stand` (pas de trad fr),
  "Photograph Frame" `exposure:photograph_frame`, "Glass Photograph Frame" `exposure:glass_photograph_frame`,
  "Glow Photograph Frame" `exposure:glow_photograph_frame` (pas de trad fr) [j].

## Mécaniques
- Appareil photo : plage focale par défaut 18-55mm sans objectif ; clic droit en inventaire ouvre l'écran
  fixations/accessoires [c].
- Pellicule : plusieurs poses par film (compteur affiché), tooltip donne sensibilité, balance des couleurs,
  contraste, bruit, palette [j].
- Développement/impression via la Chambre claire : nécessite lumière ≥13, consomme des teintures (noir pour
  N&B, cyan+magenta+jaune+noir pour couleur) [c].
- Camera Stand : rayon de fonctionnement 100 blocs autour du propriétaire ; hors zone = appareil "en panne"
  (réparable en le réutilisant) ; si le propriétaire est absent, un autre joueur proche peut servir de secours [c].
- Interplanar Projector : renommé avec une URL ou un chemin de fichier puis utilisé comme filtre = projette une
  image d'un autre plan ; se consomme à l'usage ; mode "Clean" ou "Dithered" au clic droit [j].
- Cadre à photo : 3 tailles (1x1, 2x2, 3x3), pose comme un tableau mais aussi au sol/plafond ; sac d'encre
  luminescent = version lumineuse [j].
- Album photo : peut être signé, devient alors non modifiable [j].

## Config serveur
- `lightroom_light_requirement = 13` [c].
- `dyes_black_and_white = ["black"]`, `dyes_color = ["cyan","magenta","yellow","black"]` [c].
- `print_time_black_and_white = 80` ticks [c].
- `working_range` (Camera Stand) = 100, `out_of_working_range_malfunction = true` [c].
- `default_frame_size = 320` (résolution capture par défaut) [c].
- `projecting_enabled = true`, `projecting_timeout_ticks = 100` (5s) [c].
- `film_roll_easy_renaming = true` — pellicules renommables sans coût XP [c].
- `fallback_to_other_players_projector = false` chez nous : le projecteur ne va PAS chercher une image sur le
  PC d'un autre joueur si le propriétaire est absent [c].
