---
slug: easy-magic
nom: Easy Magic
namespaces: [easymagic]
version: v21.1.4-1.21.1-Fabric
cote: S+C
resume: Refonte table d'enchantement - items restent à la fermeture, reroll des enchants possible
sources:
  m: https://modrinth.com/mod/easy-magic
  g: https://github.com/Fuzss/easymagic
  j: jar EasyMagic-v21.1.4-1.21.1-Fabric.jar
  c: config serveur easymagic-server.toml, easymagic-common.toml
verifie: 2026-09-13
---

## Mécaniques
- Tables d'enchantement vanilla remplacées : les vanilla restantes deviennent inutilisables après install
  (`disable_vanilla_enchanting_table`), celles générées par le monde après sont automatiquement converties
  (`convert_vanilla_enchanting_table_during_world_gen`, pas les chunks déjà générés) [c].
- Item et livres/lapis dans l'interface restent en place à la fermeture, plus de perte [m].
- Bouton "Reroll enchantments" dans l'interface pour relancer les enchantements proposés
  (`reroll_enchantments = true`) [j,c].
- Coût du reroll par défaut : 1 lapis-lazuli (`easymagic:enchanting_catalysts`) + 5 points d'expérience
  (`reroll_catalyst_cost` / `reroll_experience_points_cost`) [j,c]. Peut être basculé pour coûter des niveaux
  d'enchant complets à la place (`rerolling_takes_enchantment_levels`, désactivé chez nous) [c].
- Slot dédié au catalyseur de reroll possible via tag `easymagic:reroll_catalysts` séparé de `enchanting_catalysts`
  (désactivé chez nous, `dedicated_reroll_catalyst = false`) [c].
- Puissance d'enchantement max (équivalent 15 bibliothèques) : `max_enchanting_power = 15` (valeur vanilla) [c].
- Blocs sans forme de collision pleine (torche, tapis) ne bloquent plus une bibliothèque placée derrière de compter
  (`lenient_bookshelves`) [c].
- Étagères ciselées (chiseled bookshelves) donnent de la puissance d'enchantement si elles font face à la table,
  1 pour 3 livres contenus (`chiseled_bookshelf_enchanting_power = "FACING"`) [c].
- Tooltip d'enchantement dans l'interface : affiche 1 seul enchantement possible par ligne (`enchantment_hint =
  "SINGLE"`) [c].
