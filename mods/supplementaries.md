---
slug: supplementaries
nom: Supplementaries
namespaces: [supplementaries]
version: 1.21.1-3.9.9
cote: S+C
resume: Blocs déco/utilitaires vanilla+ à mécaniques (redstone, rangement, gadgets) — des centaines de variantes
sources:
  m: https://modrinth.com/mod/supplementaries
  w: https://github.com/MehVahdJukaar/Supplementaries/wiki
  g: https://github.com/MehVahdJukaar/Supplementaries
  j: jar supplementaries-1.21.1-3.9.9-fabric.jar
  c: config serveur supplementaries-common.json
verifie: 2026-09-13
---

## Ajoute
- Familles déco à teintes/variantes : Awning `supplementaries:awning*` (16 couleurs), Present `present*`/
  `trapped_present*` (16 couleurs), Bunting `bunting*`, Flag `flag*`, Candle Holder `candle_holder*`,
  Sconce `sconce*` (glow/soul/ender/cupric/nether_brass) [j].
- Familles pierre taillée : Ash Bricks, Brittlestone Bricks, Lapis Bricks, Stone/Blackstone/Deepslate/
  End Stone Lamp, Stone/Blackstone Tile (+ dalles/escaliers/murs) `supplementaries:<nom>` [j].
- Objets à mécanique redstone : Bellows (soufflet, attise feux/fournaises) `bellows`, Crank (manivelle,
  génère redstone via clic) `crank`, Faucet (robinet, transvase fluides) `faucet`, Turn Table (plaque
  tournante, tourne entités/loot des conteneurs) `turn_table`, Pulley Block (poulie, tracte plateformes)
  `pulley_block`, Speaker Block (haut-parleur, joue son/texte narré) `speaker_block`, Relayer `relayer`,
  Redstone Illuminator `redstone_illuminator`, Lock Block (verrouille porte par redstone) `lock_block`,
  Spring Launcher (lanceur à ressort) `spring_launcher`, Cog Block `cog_block` [j].
- Rangement/déco fonctionnelle : Item Shelf (étagère à items) `item_shelf`, Notice Board (tableau
  d'affichage, dépose un item en grand format) `notice_board`, Pedestal (piédestal, expose 1 item)
  `pedestal`, Safe (coffre-fort verrouillable) `safe`, Sack (sac, inventaire portable posable) `sack`,
  Blackboard (tableau noir, écrit dessus) `blackboard`, Globe `globe`/`globe_sepia` (affiche coordonnées),
  Way Sign (panneau directionnel vers structures) `way_sign` [j,c].
- Items : Flute (appelle animaux à distance) `flute`, Wrench (tourne blocs orientables) `wrench`,
  Slingshot (fronde) `slingshot`, Bubble Blower `bubble_blower`, Key (ouvre coffres/portes liées) `key`,
  Quiver (carquois porté, slots flèches) `quiver`, Lunch Basket (panier repas posable) `lunch_basket`,
  Rope Arrow (flèche-corde, pose une Rope grimpable) `rope_arrow`, Altimeter, Speedometer, Cartographer's
  Quill, Slice Map (carte zoomée) `slice_map`, Bomb / Blue Bomb `bomb`(+projectile) [j].
- Mobs : Red Merchant (marchand ambulant) `red_merchant`, Plunderer (pillard naval sur navire-canon)
  `plunderer` [j].

## Mécaniques
- Sack : inventaire portable posable, 9 slots par défaut, pénalité de vitesse si porté (`sack_penalty`) [c].
- Quiver : porté (slot armure/curio), 6 slots de flèches par défaut, utilisable sans effet de lenteur
  (`use_without_slow`) [c].
- Cannon/Cannonball/navire-canon : tire des boulets qui font exploser du TNT à l'impact (`explode_tnt:
  IGNITE`), fuse 40 ticks, cooldown 60 ticks ; pillards utilisent les canons sur bateau en raid naval [c].
- Urn (urne) : peut faire apparaître une créature (« critter ») à la casse, chance 1% par défaut ;
  urnes de grotte activées (génération naturelle) [c].
- Faucet : transvase fluides (ex. vide un tonneau/chaudron) ; peut aussi faire tomber des items [c,j].
- Turn Table : sous un conteneur, mélange son contenu (`shuffle_containers`) et fait tourner les entités
  posées dessus [c].
- Pulley Block : tracte un bloc/plateforme relié par corde, tirage coopératif possible (plusieurs poulies
  synchronisées), utilisable comme ascenseur de mineshaft [c].
- Way Sign : pointe vers la structure la plus proche dans un rayon (200 blocs par défaut), affiche la
  distance [c].
- Bellows : actionné manuellement ou par redstone, attise les feux/fournaises dans un rayon (5 blocs
  par défaut) [c].
- Timber Frame/Daub (pans de bois) : hache décorative en frappant (`axes_strip`), remplace le Daub par
  variante avancée (`replace_daub`) [c].

## Config serveur
- `general.creative_tab: false` — pas d'onglet créatif dédié Supplementaries sur ce serveur (items
  répartis dans les onglets vanilla) [c].
- Slots par défaut gardés : Sack 9, Quiver 6, Lunch Basket 6 [c].
- Bomb : rayon 2.0 (Blue Bomb 3.0, se scinde en 5 mini-bombes) [c].
- Cannon : puissance de tir 0.6, mèche 40 ticks, cooldown 60 ticks [c].
- Speaker Block : narrateur activé, texte max 32 caractères, portée 64 blocs [c].
- Wrench : contourne l'action normale seulement en main principale (`bypass_when_on: MAIN_HAND`) [c].

## Pièges
- Bloqué avec `sodium <0.8.12-beta.1` et `farmersdelight <1.21.1-2.2.0` (dépendances `breaks` du jar) [j].
- Casse compat avec `amendments <1.21-2.0.0` (voir fiche amendments) [j].

## Compat
- Détecte/interagit avec Farmer's Delight, Create, Curios/Trinkets, Quark, Serene Seasons si présents
  (données de compat dans le jar) ; sur ce pack, vérifier présence effective de ces mods avant de
  compter sur l'intégration [j].
