---
slug: immersive-melodies
nom: Immersive Melodies
namespaces: [immersive_melodies]
version: 0.7.1+1.21.1
cote: S+C
resume: instruments jouables (clavier libre ou mélodie MIDI/ABC importée), audibles par les autres joueurs
sources:
  m: https://modrinth.com/mod/immersive-melodies
  w: https://github.com/Luke100000/ImmersiveMelodies/wiki
  g: https://github.com/Luke100000/ImmersiveMelodies
  j: jar immersive_melodies-fabric-0.7.1+1.21.1.jar
  c: config serveur immersive_melodies.json
verifie: 2026-09-13
---

## Ajoute
- Items instruments : Cornemuse `immersive_melodies:bagpipe`, Didgeridoo `immersive_melodies:didgeridoo`,
  Flûte `immersive_melodies:flute`, Luth `immersive_melodies:lute`, Piano `immersive_melodies:piano`,
  Triangle `immersive_melodies:triangle`, Trompette `immersive_melodies:trumpet`,
  Tambour minuscule `immersive_melodies:tiny_drum`, Vielle `immersive_melodies:vielle`,
  Basses de l'Ender `immersive_melodies:ender_bass`, Poignée `immersive_melodies:handpan` [j].

## Mécaniques
- Utiliser un instrument ouvre un écran : jouer au clavier (notes libres) ou charger une mélodie perso
  (fichier `.abc` ou `.midi` déposé dans l'écran) [j].
- Fichiers ABC convertis via un service en ligne (connexion internet requise), MIDI lu directement [g].
- MIDI multi-pistes : le mod choisit automatiquement la meilleure piste, sélection manuelle possible via
  l'icône partition [g].
- Écran liste des pistes : favoris, recherche, pause/lecture [j].

## Config serveur
- `maxAudibleDistance = 48` blocs [c].
- `bufferDelay = 75`, `instrumentVolumeFactor = 1.0` [c].
- `mobInstrumentFactors` : mobs hostiles (zombie, piglin brute, pillager, skeleton, wither skeleton,
  zombified piglin, piglin, husk) jouent très faiblement (facteur 0.01) s'ils ramassent un instrument [c].
- `forceMobsToPickUp = true`, `mobInstrumentDropFactor = 0.085` [c].
- `showOtherPlayersMelodies = true`, `autoSynchronize = true` [c].
- `stopGameMusicForPlayers = true` (coupe la musique du jeu pendant qu'un instrument joue),
  `stopGameMusicForMobs = false` [c].
- `uploadPermissionLevel = 0` — tout le monde peut importer un fichier [c].
- `loadInbuiltMidis = true` — mélodies intégrées chargées [c].

## Pièges
- Import ABC passe par un serveur de conversion externe (pas de stockage annoncé du fichier) : inutilisable
  hors ligne [g].
