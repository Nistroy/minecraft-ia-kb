---
slug: emotecraft
nom: Emotecraft
namespaces: [emotecraft]
version: 2.4.12+1.21.1-fabric
cote: S+C
resume: émotes/animations joueur avec roue de sélection rapide, émotes perso importables
sources:
  m: https://modrinth.com/mod/emotecraft
  g: https://github.com/KosmX/emotes
  j: jar emotecraft-for-MC1.21.1-2.4.12-fabric.jar
  c: config serveur emotecraft.json
verifie: 2026-09-13
---

- Côté C : client_side required sur Modrinth, server_side optional [m]. Sans le mod côté serveur, les autres
  joueurs ne voient pas les émotes jouées ; avec une version différente entre client et serveur, l'affichage
  aux autres peut être incorrect [j].

## Mécaniques
- Écran des émotes : liste complète, recherche, favoris ; menu-rapide (roue) personnalisable — clic gauche sur
  une émote pour l'ajouter à la roue, clic droit pour la retirer [j].
- Touche personnalisable par émote pour la jouer directement ; touches dédiées existantes : menu-rapide
  (`key.emotecraft.fastchoose`), arrêt d'animation (`key.emotecraft.stop`) — pas de touche par défaut précisée
  dans les textes du mod [j].
- Émotes perso possibles ; export en `.json` ou `.emotecraft` depuis le menu [j].
- Vue 3e personne activable pendant une émote (option "perspective") [j].
- Émotes NSFW activables/désactivables séparément (avertissement contenu inapproprié dans le texte) [j].

## Config serveur
- `loadbuiltin = true` (émotes intégrées chargées), `quark = false` (lecteur alternatif instable, désactivé),
  `validate = false` (pas de validation anti-triche PvP), `debug = true` [c].
- `emotesFolderOnLogicalServer = true` [c] — voir Pièges.

## Pièges
- Notre config a `emotesFolderOnLogicalServer: true`. Le texte du mod dit explicitement de GARDER cette option
  désactivée : si activée, les émotes personnalisées ne fonctionnent qu'en solo [j,c]. À vérifier/corriger.
