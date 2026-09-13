---
slug: do-a-barrel-roll
nom: Do a Barrel Roll
namespaces: [do_a_barrel_roll]
version: 3.7.3+1.21-fabric
cote: S+C
resume: vol elytre façon simulateur de vol (roulis/tangage/lacet, poussée, dégâts de choc réglables)
sources:
  m: https://modrinth.com/mod/do-a-barrel-roll
  g: https://codeberg.org/enjarai/do-a-barrel-roll
  j: jar do_a_barrel_roll-fabric-3.7.3+1.21.jar
  c: config serveur do_a_barrel_roll-server.json
verifie: 2026-09-13
---

- Côté C : client_side required sur Modrinth, server_side optional [m]. Jouable en solo/client seul ; les
  réglages serveur (forcer actif/installé, autoriser la poussée) n'existent que si le mod est aussi côté
  serveur [j].

## Mécaniques
- Ajoute un axe de roulis en plus du tangage/lacet vanilla pendant le vol à l'élytre [j].
- Mode d'activation configurable : Vanilla (1 saut), Triple Jump (2 sauts), Hybrid, Hybrid Toggle [j].
- Poussée (thrust) : touches dédiées pour accélérer/décélérer en continu en vol ; le texte du mod précise
  qu'elle est "désactivée sur tout serveur qui ne l'autorise pas explicitement" [j].
- Dégâts cinétiques réglables par le serveur : Vanilla / Haute vitesse seulement / Aucun / Insta-kill au choc [j].
- Bascule (banking) optionnelle : incline la caméra selon le roulis pour un ressenti "avion" sans loopings
  complets [j].
- Options avancées : formules personnalisables (variables pitch/yaw/roll/vitesse) pour le banking et
  l'efficacité des gouvernes [j].
- Si le serveur force le mod actif (`force_enabled`), le joueur ne peut plus le désactiver côté client [j].
- Si le serveur force le mod installé (`force_installed`), les joueurs sans le mod sont expulsés [j].

## Config serveur
- Fichier vide (`{}`) chez nous → tous les réglages serveur restent à leur valeur par défaut du mod (état
  réel de la poussée/activation forcée non déterminable sans lire le code par défaut, non vérifié) [c].

## Pièges
- Pas de traduction française dans le jar (uniquement en_us) [j].
