---
slug: naturalist
nom: Naturalist
namespaces: [naturalist]
version: 2.0.3+1.21.1-fabric
cote: S+C
resume: 50 mobs vanilla-style (mammifères, oiseaux, reptiles, poissons, insectes) + blocs déco shellstone/froglass
sources:
  m: https://modrinth.com/mod/naturalist
  j: jar naturalist-2.0.3-fabric-1.21.1.jar
  c: config serveur naturalist-server.properties
verifie: 2026-09-13
---

## Ajoute
- 50 entités dans `entity.naturalist.*` (liste en_us du jar, trad FR partielle/absente sur cette version) [j].
  Mammifères : alligator, ours (`bear`/`black_bear`), sanglier, capybara, chevreuil, éléphant, girafe,
  hérisson, hippopotame, lion, mammouth, taupe, rhinocéros, tigre, zèbre `naturalist:<id>` [j].
  Oiseaux : `naturalist:bird` (variantes teintables, remplace les anciens geai/cardinal/moineau/etc.),
  autruche, vautour, dinde `naturalist:turkey` [j].
  Reptiles/amphibiens : lézard (+queue détachable `lizard_tail`), serpent, serpent corail, serpent à
  sonnettes (via `snake` variants), tortue, dragon de Komodo, escargot [j].
  Poissons/aquatique : bar, poisson-chat, piranha, anglerfish, blobfish, raie, requin blanc, méduse,
  étoile de mer, palourde (`clam`), crabe [j].
  Insectes : papillon (+ chenille + chrysalide), libellule, luciole, fourmi, scorpion (désert/jungle),
  cloporte géant (`giant_isopod`) [j].
- Blocs déco : Shellstone (brut, taillé, lisse + dalles/escaliers/murets), Greverre/Grevitre (froglass,
  3 teintes azuré/cramoisi/verdoyant), Roseau à massette `cattail`, Lentilles d'eau `duckweed`,
  Chrysalide `chrysalis`, œufs de mob (alligator, autruche, escargot, tortue) [j].
- Items : Filet de capture `naturalist:capture_net` (bambou + ficelle, forme en L), viandes crues/cuites
  (gibier `bushmeat`, venaison, canard, poisson-chat, bar, queue de lézard), Bois de chevreuil `antler`,
  Quenouille `cattail_fluff` [j].

## Mécaniques
- Filet de capture `naturalist:capture_net` : se craft avec bambou + ficelle (forme en L) [j].
- Chrysalide `naturalist:chrysalis` : bloc lié au cycle de vie chenille → papillon [j].
- Chaque mob a sa propre loot table (`data/naturalist/loot_table/entities/`) [j].

## Config serveur
- `server/config/naturalist-server.properties` : tous les `<mob>_removed=false` par défaut chez nous,
  aucun mob désactivé [c].
- `parrot_flight=true`, `bird_head_slow_falling=true`, `snail_crushing=false`, `remove_all_bugs=false`
  (réglages par défaut, insectes/perroquets non touchés) [c].
