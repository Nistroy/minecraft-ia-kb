---
slug: bountiful
nom: Bountiful
namespaces: [bountiful]
version: 8.0.0-beta.2
cote: S+C
resume: Tableaux de primes générés en village, missions (rapporter un item / tuer des mobs) contre récompenses
sources:
  m: https://modrinth.com/mod/bountiful
  w: https://kambrik.ejekta.io/mods/bountiful/
  j: jar bountiful-fabric-8.0.0-beta.2.jar
  c: config serveur bountiful/bountiful.json
verifie: 2026-09-13
---

## Ajoute
- Bloc Tableau de primes `bountiful:bountyboard`, génère des primes (bounties) tout seul dans le temps [j,m].
- Décrets (Decrees), items qui orientent le type de primes générées sur un tableau : Forge d'armures
  (armorer), Boucherie (butcher), Fournitures du chef (chef), Fournitures de clerc (cleric), Agriculture
  (farmer), Pêche (fisherman), Archerie (fletcher), Chasse (hunting), Inventing (inventor), Travail du cuir
  (leatherer), Bibliothécaire (librarian), Cartographie (mapper), Maçonnerie (mason), Berger (shepherd),
  Bricoler (tinker), Forge d'outils (toolsmith) — id `bountiful:decree_<nom>` [j].

## Mécaniques
- Une prime demande de rapporter un item précis ou tuer des mobs, en échange d'une récompense ; on
  redonne la prime au tableau (clic droit) pour être payé [m].
- Jusqu'à 3 décrets combinables sur un même tableau, mélange les objectifs/récompenses des décrets
  posés (`allowDecreeMixing: true`) [m,c].
- Un décret placé sur le tableau au hasard (sans le fabriquer) peut aussi être obtenu comme récompense de
  prime [m].
- Rareté des primes façon vanilla : Commun / Peu commun / Rare / Épique, plus la rareté est haute plus les
  récompenses rares ont de chances d'apparaître [m].
- Réputation par tableau : augmente en complétant des primes, débloque des primes/récompenses plus rares
  au fil du temps [m].
- Nécessite le mod Kambrik en dépendance (même auteur, déjà présent, lib) [j].

## Où trouver
- Tableaux générés dans les villages ; fréquence de génération par village configurable
  (`villageGenFrequency: 2`) [m,c].

## Config serveur
- Les primes expirent avec un minuteur (`shouldHaveTimersAndExpire: true`) [c].
- Rafraîchissement du tableau toutes les 45s pour vérifier/générer de nouvelles primes
  (`updateFrequencySecs: 45`) [c].
- Le tableau peut être cassé par un joueur (`canBreak: true`) [c].
- 1 à 2 primes initiales générées, 1 à 2 primes "filler" en renfort (`initialCountPreference`,
  `fillerCountPreference`) [c].
- Toast de complétion affiché côté client (`showCompletionToast: true`) [c].

## Pièges
- Version installée `8.0.0-beta.2` = beta, pas une release stable [j].
