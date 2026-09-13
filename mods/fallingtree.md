---
slug: fallingtree
nom: FallingTree
namespaces: [fallingtree]
version: 1.21.1-1.21.1.11
cote: S
resume: Coupe un seul bloc de tronc pour abattre tout l'arbre d'un coup, feuilles cassées avec
sources:
  m: https://modrinth.com/mod/fallingtree
  w: https://github.com/RakambdaOrg/FallingTree/wiki
  g: https://github.com/RakambdaOrg/FallingTree
  j: jar FallingTree-1.21.1-1.21.1.11.jar
  c: config serveur fallingtree.json
verifie: 2026-09-13
---

## Mécaniques
- Couper un bloc de tronc casse tout l'arbre détecté d'un coup (`detectionMode = "WHOLE_TREE"`), de façon
  instantanée chez nous (`breakMode = "INSTANTANEOUS"`, pas de chute progressive) [c].
- Feuilles cassées avec l'arbre (`leavesBreaking = true`), troncs mélangés (essences différentes) interdits par
  défaut (`allowMixedLogs = false`) [c].
- Taille max d'arbre traitée : 100 blocs de tronc (`maxSize`), au-delà l'action est annulée
  (`maxSizeAction = "ABORT"`, message en jeu "Cet arbre est trop grand et ne peut être coupé en un coup") [c,j].
- Sneak désactive l'effet par défaut chez nous (`sneakMode = "SNEAK_DISABLE"`) : il faut ne PAS être accroupi pour
  déclencher l'abattage groupé [c].
- Aucune restriction d'outil (`tools.allowed` vide = tous les outils marchent), aucun enchantement requis
  (`enchantment.requireEnchantment = false`) [c].
- Ne fonctionne pas en créatif chez nous (`breakInCreative = false`) [c].
- Si l'outil est sur le point de casser (durabilité), l'abattage groupé est empêché : message en jeu "Ton outil est
  sur le point de casser, va le réparer ou fais en un nouveau" [j].
- Notification du nombre de blocs cassés affichée dans la barre d'action (`notificationMode = "ACTION_BAR"`) [c].
- Casse aussi les warts d'arbre du Nether et les racines de mangrove [c].
