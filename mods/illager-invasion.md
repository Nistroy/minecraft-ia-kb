---
slug: illager-invasion
nom: Illager Invasion
namespaces: [illagerinvasion]
version: 21.1.6
cote: S+C
resume: ~11 nouveaux illagers avec capacités uniques, 5 structures dédiées, table d'imprégnation pour enchants
sources:
  m: https://modrinth.com/mod/illager-invasion
  g: https://github.com/Fuzss/illagerinvasion
  j: jar IllagerInvasion-v21.1.6-1.21.1-Fabric.jar
  c: config serveur illagerinvasion-server.toml
verifie: 2026-09-13
---

## Ajoute
- Illagers (`illagerinvasion:<id>`, pas de trad FR dans le jar) : Alchemist (archer, potions à effet
  différé), Archivist (buff les illagers proches, fuit et lance des sorts si effrayé), Basher (bouclier,
  charge le joueur), Marauder (lance des hachettes, peut faire tomber la Hachette Platine Imprégnée),
  Provoker (arc + sorts de buff basiques), Sorcerer (invoque du feu violet dangereux, drop Unusual Dust),
  Necromancer (invoque des morts-vivants), Inquisitor (guerrier au bouclier puissant, casser le bouclier
  avant de le vaincre), Firecaller (mage discret, magie dévastatrice), Invoker (le plus puissant, drop
  Hallowed Gem pour la table d'imprégnation), Surrendered (illager qui s'est rendu) [m,j].
- Illusioner remis en jeu en survie avec nouvelle apparence, drop Illusionary Dust [m].
- Structures : Cabane du Firecaller (badlands), Fort des illagers (taïgas), Tour de l'Illusionneur
  (taïgas + forêts sombres), Labyrinthe souterrain (entrée = temple en pierre, forêts), Cabane du
  Sorcerer (forêts sombres) [m,j].
- Bloc Table d'imprégnation `illagerinvasion:imbuing_table` — dépasse les limites d'enchant normales,
  consomme un Hallowed Gem à chaque utilisation [m,j].
- Items : Hachette Platine Imprégnée (lancée, rare chez Marauder), Lost Candle (révèle les minerais
  proches), Horn of Sight (fait briller les monstres proches), Hallowed Gem, Illusionary Dust,
  Unusual Dust, Primal Essence, chunk/sheet de platine [m,j].

## Mécaniques
- Trims d'armure en platine : effets spéciaux si `platinum_trim_effects` actif (défaut) — casque = plus
  d'XP en tuant, plateau = minage plus rapide sans outil adapté, jambières = faim réduite à l'effort,
  bottes = plus de dégâts au sol cultivé (pas de piétinement) [c].

## Où trouver
- Cabane Firecaller : badlands [m].
- Fort des illagers : taïgas [m].
- Tour de l'Illusionneur : taïgas et forêts sombres [m].
- Labyrinthe : biomes forestiers (majorité) [m].
- Cabane du Sorcerer : forêts sombres [m].

## Config serveur
- Tous les illagers participent aux raids de village par défaut (`participate_in_raids = true`), sauf
  Invoker (`false` par défaut chez l'auteur du mod, boss bar jaune activée) [c].
- `platinum_trim_effects = true` (défaut, voir Mécaniques) [c].
