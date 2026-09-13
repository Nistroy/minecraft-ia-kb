---
slug: easy-anvils
nom: Easy Anvils
namespaces: [easyanvils]
version: v21.1.0-1.21.1-Fabric
cote: S+C
resume: Refonte de l'enclume - items ne se perdent plus, coûts plus justes, moins de pénalité de réparation
sources:
  m: https://modrinth.com/mod/easy-anvils
  g: https://github.com/Fuzss/easyanvils
  j: jar EasyAnvils-v21.1.0-1.21.1-Fabric.jar
  c: config serveur easyanvils-server.toml, easyanvils-common.toml
verifie: 2026-09-13
---

## Mécaniques
- Enclumes vanilla : plus utilisables après install (`disable_vanilla_anvil`), remplacées dans les structures générées après
  (pas les chunks déjà générés) [c].
- Items dans l'enclume restent en place à la fermeture de l'interface, plus de perte [m].
- Renommer un objet : gratuit, 0 niveau (`free_renames = ALL_ITEMS`), ne casse jamais l'enclume
  (`risk_free_anvil_renaming`), supporte les codes couleur/style dans le champ de texte [j,c].
- Éditer une étiquette (name tag) sans enclume : sneak + clic droit (`edit_name_tags_no_anvil`), texte affiché
  "Edit %s" en jeu [j,c].
- Réparer avec un matériau (ex. lingot) : +1 niveau par matériau utilisé, restaure 25% de durabilité par matériau
  (`repair_with_material_unit_cost` / `restored_durability`) [c].
- Combiner avec un item du même type non réparé : +2 niveaux, bonus de 12% de durabilité en plus
  (`repair_with_other_item_cost` / `bonus_durability`) [c].
- Coût des enchantements venant d'un livre enchanté divisé par 2 (`halved_book_costs`) [c].
- Pas de limite de coût max en niveaux par défaut sur notre serveur (`too_expensive_limit = -1`, "Too Expensive!"
  désactivé) [c].
- Pénalité de travail antérieur (prior work penalty) : mode `LIMITED`, +4 niveaux max par palier ; renommer/réparer
  n'augmente jamais la pénalité (`penalty_free_renames_and_repairs`) et coûte selon le mode `FIXED` (ignore la
  pénalité déjà accumulée) [c].
- Combiner deux livres enchantés n'augmente pas la pénalité (`penalty_free_enchants_for_books`) [c].
- Chance de casse de l'enclume par usage : 5% (`anvil_break_chance`, vanilla = 12%) [c].
- Réparer une enclume abîmée avec un bloc de fer (1 dégât réparé par bloc), automatisable au distributeur
  (`anvil_repairing`) [c].
- Mobs avec nom personnalisé : ne droppent pas d'étiquette à la mort sur notre config (`name_tags_drop_from_mobs
  = false`) [c].

## Pièges
- Une enclume vanilla restante dans le monde (posée avant install) devient inutilisable : casser + reposer pour
  avoir la version Easy Anvils [c].
