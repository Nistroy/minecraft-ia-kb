---
slug: naturalist
nom: Naturalist
namespaces: [naturalist]
version: 2.0.3+1.21.1-fabric
cote: S+C
resume: 48 animaux vanilla-style (mammifères, oiseaux, reptiles, poissons, insectes) + blocs déco shellstone/froglass
sources:
  m: https://modrinth.com/mod/naturalist
  j: jar naturalist-2.0.3-fabric-1.21.1.jar
  c: config serveur naturalist-server.properties
verifie: 2026-09-13
---

Traduction FR du jar incomplète (fichier ancien) : nom FR en jeu quand il existe, sinon nom anglais en jeu
(glose FR entre parenthèses). Ids : `naturalist:<id>`. [j]

## Ajoute
- Mammifères : Ours `bear`, Black Bear `black_bear`, Sanglier `boar`, Capybara `capybara`, Chevreuil `deer`,
  Éléphant `elephant`, Girafe `giraffe`, Hedgehog `hedgehog` (hérisson), Hippopotame `hippo`, Lion `lion`,
  Mammoth `mammoth` (mammouth), Mole `mole` (taupe), Rat `rat`, Rhinocéros `rhino`, Tiger `tiger` (tigre),
  Zèbre `zebra`, Whale `whale` (baleine). [j]
- Oiseaux : Bird `bird`, Canard `duck`, Autruche `ostrich`, Turkey `turkey` (dinde), Vautour `vulture`. [j]
- Reptiles : Alligator `alligator`, Komodo Dragon `komodo_dragon`, Lézard `lizard` (+ Queue de lézard
  `lizard_tail`), Serpent `snake`, Tortue terrestre `tortoise`. [j]
- Aquatiques : Bar `bass`, Poisson-chat `catfish`, Anglerfish `anglerfish` (baudroie), Blobfish `blobfish`,
  Clam `clam` (palourde), Crab `crab` (crabe), Great White Shark `great_white_shark` (grand requin blanc),
  Jellyfish `jellyfish` (méduse), Piranha `piranha`, Ray `ray` (raie), Starfish `starfish` (étoile de mer),
  Giant Isopod `giant_isopod` (isopode géant). [j]
- Petites bêtes : Papillon `butterfly`, Chenille `caterpillar`, Libellule `dragonfly`, Luciole `firefly`,
  Ant `ant` (fourmi), Escargot `snail`, Desert Scorpion `desert_scorpion`, Jungle Scorpion `jungle_scorpion`. [j]
- Blocs déco : Shellstone (brute, taillée, lisse + dalles/escaliers/murets), Greverre / Grevitre (froglass et
  vitre, teintes azuré/cramoisi/verdoyant), massette `cattail`, lentilles d'eau `duckweed`, chrysalide
  `chrysalis`, œufs de mob. [j]
- Items : filet de capture `naturalist:capture_net`, viandes crues/cuites (dont gibier `bushmeat`, venaison,
  canard, poisson-chat, bar, queue de lézard), bois de chevreuil `antler`. [j]

## Mécaniques
- Filet de capture `naturalist:capture_net` : recette bambou + ficelle. [j]
- Chrysalide `naturalist:chrysalis` : étape entre chenille et papillon. [j]
- Chaque mob a sa loot table (`data/naturalist/loot_table/entities/`). [j]

## Config serveur
- `naturalist-server.properties` : tous les `<mob>_removed=false`, aucun mob désactivé. [c]
- `parrot_flight=true`, `bird_head_slow_falling=true`, `snail_crushing=false`, `remove_all_bugs=false`. [c]
