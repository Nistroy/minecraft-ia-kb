# minecraft-ia-kb — connaissances du modpack BahBeuh

Base de connaissances de l'assistant IA en jeu (`Nistroy/minecraft-ia`) pour le serveur Fabric 1.21.1 de nistroy.
Lue par le cerveau (index FTS reconstruit), écrite par l'IA (notes, commits auto) et nistroy (édite/revert).
Docs écrites pour agents : notes denses, pas de prose.

## Arbo
- `mods/<slug>.md` — 1 fiche/mod. `<slug>` = slug Modrinth.
- `index.md` — généré (`minecraft-ia kb index`), 1 ligne/mod depuis frontmatter. Jamais édité à la main.
- `notes/<slug>/<YYYY-MM-DD>-<id>.md` — faits appris par l'IA. `<slug>` = `_general` si pas de mod.

## Fiche mod — format
Frontmatter YAML obligatoire :
```yaml
---
slug: aether                      # slug Modrinth
nom: The Aether                   # nom affiché
namespaces: [aether]              # namespaces du jar (data/<ns>/, assets/<ns>/) ; ids = <ns>:<id>
version: 1.21.1-1.5.11-fabric     # version installée (versions-testees.tsv du dépôt serveur)
cote: S+C                         # S / C / S+C (Modrinth server_side/client_side)
resume: Dimension du ciel, donjons + 3 boss, portail en glowstone   # 1 ligne, pour index.md
sources:
  m: https://modrinth.com/mod/aether
  w: https://aether-wiki.example/...    # wiki du mod si existe
  g: https://github.com/.../...         # source / README
  j: jar aether-1.21.1-1.5.11-fabric.jar
  c: config serveur aether-common.toml
verifie: 2026-09-12               # date de vérif des faits
---
```
Sections (omettre si vide) :
- `## Ajoute` — contenu : blocs, items, mobs, structures, biomes, enchants. Nom FR (lang `fr_fr` du jar si présent) + id `ns:id`.
- `## Mécaniques` — comment ça marche, comment faire (obtenir, activer, fabriquer non-trivial).
- `## Où trouver` — structures/biomes/dimensions, loot, marchands, profondeur.
- `## Config serveur` — réglages notables de NOTRE config (fichier `server/config/…`), seulement si ≠ défaut ou utile au joueur.
- `## Pièges` — bugs connus pour cette version, pertes d'items, danger, incompat.
- `## Compat` — interactions avec d'autres mods du pack, seulement si sourcée.

Règles :
- Frontmatter = YAML valide : valeur contenant `:` → entre guillemets. Fiche invalide = ignorée par le cerveau (log).
- Chaque puce finit par clé(s) de source définies dans `sources` : `[m]`, `[j]`, `[w,g]`… Fichiers de langue = `[j]`.
  Pas de source → pas de puce.
- Nom en jeu exact du jar (`fr_fr` si la clé existe, sinon `en_us` tel quel). Traduction perso seulement entre
  parenthèses. Mécanique ou chiffre = texte explicite (infobulle, lore, advancement, config, doc), jamais déduit d'un
  nom de fichier ou de classe.
- Jamais inventer (nom, id, recette, chiffre). Doute → omettre.
- Version : infos wiki/GitHub d'une autre version MC/mod → vérifier ou préciser `(v. X)`.
- Résumer, jamais copier le texte des pages (droits). Recettes détaillées inutiles : DB exacte + EMI en jeu.
- Caveman FR : fragments, puces, pas d'intro/outro. Viser 20-80 lignes.

## Note apprise — format
```yaml
---
mod: aether              # slug ou _general
version: 1.21.1-1.5.11-fabric
statut: non-vérifié      # non-vérifié / confirmé-joueur / validé-nistroy / contesté
source: https://...      # URL ou fichier
date: 2026-09-12
reponse: 42              # id réponse d'origine (DB cerveau), optionnel
---
Fait en 1-3 lignes caveman.
```
- Statut : IA crée `non-vérifié` ; vote ✔ → `confirmé-joueur` ; vote ✘ → `contesté` ; nistroy → `validé-nistroy`.
- Rien supprimé auto. Réorganisation par l'IA = commit (diff visible, revert).
