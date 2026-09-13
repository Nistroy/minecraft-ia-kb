---
slug: aether
nom: The Aether
namespaces: [aether]
version: 1.21.1-1.5.11-fabric
cote: S+C
resume: Dimension du ciel (îles flottantes), 3 donjons + boss, portail en pierre lumineuse
sources:
  m: https://modrinth.com/mod/aether
  w: https://aether.wiki.gg/
  g: https://github.com/The-Aether-Team/The-Aether
  j: jar aether-1.21.1-1.5.11-fabric.jar
  c: config serveur aether-common.toml, aether-server.toml
verifie: 2026-09-13
---

## Ajoute
- Dimension `aether:the_aether`, îles flottantes en ciel. [j,m]
- Bois skyroot (planches/bûches/portes/etc `aether:skyroot_*`), pierre sacrée `holystone`, pierre sculptée `carved_stone`, pierre angélique `angelic_stone`, pierre brûlante `hellfire_stone` - blocs de construction. [j]
- Minerais : ambrosium (`ambrosium_ore`, équivalent charbon, éclat mangeable = +½ cœur), zanite (`zanite_ore`, outils/armure niveau fer), gravitite (`gravitite_ore`, le plus rare, flotte vers le haut). [j]
- Mobs : Moa (`aether:moa`, monture, œuf à incuber), Phyg (`phyg`, cochon volant), Aérolapin (`aerbunny`), Cocatrice (`cockatrice`), Mimic (`mimic`, coffre piège), Sentinelle (`sentry`), Swets bleu/doré (`blue_swet`/`golden_swet`), Zéphyr (`zephyr`), Tourbillon/Tourbillon démoniaque (`whirlwind`/`evil_whirlwind`). [j]
- 3 donjons avec boss (confirmé via advancements) : donjon de bronze → Slider (`aether:slider`) ; donjon d'argent → Reine des Valkyries (`aether:valkyrie_queen`) ; donjon d'or → Esprit du Soleil (`aether:sun_spirit`). [j]
- Armures : zanite (≈ fer) ; gravitite (meilleur set, set complet = saut très haut, touche « Activer le saut de gravitite ») ; Neptune (donjons de bronze, nage plus rapide) ; phénix (donjon d'or). [j]
- Accessoires dédiés : gants, anneaux, pendentifs, cape, bouclier (slots `accessories.slot.aether.*`). [j]
- Altar (fabrique/répare/améliore objets, alimenté ambrosium) et Altar du Soleil (contrôle le temps de la dimension). [j]

## Mécaniques
- Portail : cadre de pierre lumineuse (glowstone) + eau à l'intérieur pour l'activer. [j]
- Gravitite : minerai → Altar → gravitite enchantée → outils/armure gravitite ; outils gravitite font léviter les blocs. [j]
- Outils skyroot : doublent les drops de minerai d'ambrosium. [j]
- Congélateur (`freezer`) : geler un accessoire avec de la pierre glaciale (`icestone`). [j]
- Incubateur (`incubator`) : faire éclore un œuf de Moa. [j]
- Jour éternel dans l'Aether tant que l'Esprit du Soleil n'est pas vaincu ; cycle jour/nuit de durée propre (≠ Overworld). [c]

## Config serveur
- "Debuff non-Aether tools" = true : outils non-Aether minent plus lentement les blocs de l'Aether. [c]
- "Only whitelisted users access Sun Altars" = false : n'importe quel joueur peut changer le temps via un Altar du Soleil. [c]
- "Golden Feather in loot" = false / "Valkyrie Cape in loot" = true : réglages du butin du donjon d'argent. [c]
- "Maximum consumable Life Shards" = 10 : limite de fragments de vie consommables par joueur. [c]
- "Disables falling into the Overworld" = false : tomber hors de l'Aether renvoie dans l'Overworld. [c]
