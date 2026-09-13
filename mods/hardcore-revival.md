---
slug: hardcore-revival
nom: Hardcore Revival
namespaces: [hardcorerevival]
version: 21.1.22+fabric-1.21.1
cote: S+C
resume: À la mort, le joueur passe K.O. au lieu de mourir tout de suite ; un autre joueur peut le réanimer à temps
sources:
  m: https://modrinth.com/mod/hardcore-revival
  w: https://mods.twelveiterations.com/minecraft/hardcore-revival
  g: https://github.com/TwelveIterations/HardcoreRevival
  j: jar hardcorerevival-fabric-1.21.1-21.1.22.jar
  c: config serveur hardcorerevival-common.toml
verifie: 2026-09-13
---

## Mécaniques
- À ce qui serait la mort, le joueur entre en état K.O. : peut regarder autour et chatter, ne peut plus
  bouger, attaquer ni utiliser d'objets [m].
- Un autre joueur maintient clic droit à proximité pour le réanimer avant la fin du minuteur [m].
- Si réanimé : léger débuff + faim, le joueur repart ; si le minuteur expire (ou le sauveteur échoue), mort
  définitive classique [m].
- Fonctionne en mode Hardcore ET en mode normal (`disableInNonHardcore: false` chez nous) [c].
- Le bouton « Accept your Fate » permet de mourir volontairement sans attendre la fin du minuteur
  (`allowAcceptingFate: true`) [c].

## Config serveur
- Minuteur avant mort définitive : 120 secondes (`secondsUntilDeath = 120`) [c].
- Distance max pour réanimer : 3 blocs (`rescueDistance = 3.0`) [c].
- Temps de maintien du clic pour réanimer : 40 ticks = 2 secondes (`rescueActionTicks = 40`) [c].
- À la réanimation : 1 cœur de vie, 5 points de faim, effets Faim (30s) + Faiblesse (60s) appliqués
  (`rescueRespawnHealth = 1`, `rescueRespawnFoodLevel = 5`, `rescueRespawnEffects`) [c].
- Joueur K.O. qui se déconnecte : minuteur suspendu jusqu'à son retour (`continueTimerWhileOffline = false`) [c].
- Chute dans la lave = mort instantanée, pas de phase K.O. (`instantDeathSources = ["minecraft:lava"]`) [c].
- Joueur K.O. reste visible à travers les blocs (`glowOnKnockout = true`) [c].
- Joueur K.O. : commandes autorisées (`allowCommands = true`), téléportation autorisée
  (`allowTeleports = true`), mais pas de combat mains nues ni d'arc (`allowUnarmedMelee = false`,
  `allowBows = false`) [c].
- Ses ender pearls jetées disparaissent à son K.O. (`enderPearlsVanishOnKnockout = true`) [c].
- K.O. répétés en moins de 40s comptent comme "consécutifs" mais le minuteur ne reprend pas où il en
  était (`consecutiveKnockoutThresholdSeconds = 40`, `resumeTimerOnConsecutiveKnockout = false`) [c].

## Pièges
- Solo (aucun autre joueur en ligne) : le mod reste actif par défaut chez nous
  (`disableInLonelyMultiplayer = false`) — mourir seul veut dire personne pour réanimer avant les 120s [c].
- Nécessite le mod Balm en dépendance (déjà présent, lib) [j].
