---
slug: grind-enchantments
nom: Grind Enchantments
namespaces: [grindenchantments]
version: 4.0.0+1.21.1
cote: S
resume: Ajoute au touret à meuler (grindstone) désenchanter vers un livre + déplacer un enchant entre 2 livres
sources:
  m: https://modrinth.com/mod/grind-enchantments
  w: https://docs.mschae23.de/Grind_enchantments
  g: https://code.mschae23.de/mschae23/grind-enchantments
  j: jar grind-enchantments-4.0.0+1.21.1.jar
  c: config serveur grindenchantments/server.json
verifie: 2026-09-13
---

## Mécaniques
- Désenchanter vers un livre : mettre un objet enchanté + un livre vierge dans la meule, récupère l'objet
  désenchanté et le livre porte l'enchantement [w]. Activé chez nous (`disenchant_to_book.enabled = true`), l'objet
  d'origine n'est pas consommé (`consume_enchanted_item = false`) [c].
- Déplacer un enchantement entre 2 livres : livre enchanté en haut + livre (vide ou déjà enchanté) en bas, le
  premier enchantement du livre du haut passe sur l'autre livre [w]. Activé chez nous
  (`move_enchantments.enabled = true`) [c].
- Réinitialiser le coût de réparation (prior work penalty) via la meule avec un catalyseur : fonctionnalité présente
  dans le mod mais désactivée chez nous (`reset_repair_cost.enabled = false`) [c].
- Coût des opérations calculé par formule configurable (niveaux d'enchant comptés, malédictions traitées à part) ;
  valeurs exactes non détaillées côté doc, voir fichier de config [w,c].
- Aucune restriction d'objet/enchantement filtrée par défaut chez nous (`filter.enabled = true` mais listes vides)
  [c].
- Mod Fabric uniquement, pas de portage Forge prévu [w].
