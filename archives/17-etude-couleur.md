# Etude de couleur, 1er novembre 2026

Calixte : « j'ai toujours l'impression que ca fait un peu mal aux yeux [...] je
choisissais juste le vert parce que je voulais signifier la croissance, mais
maintenant j'en ai marre, je veux juste que ce soit beau, bien pense, bien
designe, sans faire mal aux yeux ».

Trois passes de reglage n'ont pas suffi. Ce n'etait donc pas un reglage.

## Le diagnostic

Une couleur d'accent sert a **decouper une forme sur un fond**. Pour qu'une
forme existe, il faut un bord, donc un ecart de clarte.

| accent | clarte | ecart au fond | contraste | peut porter du texte |
|---|---|---|---|---|
| notre lime `#c6f641` | 90,9 | **4,9 points** | **1,14:1** | non, jamais |
| relab, l'orange `#f67426` | 63,5 | 30,6 points | 2,43:1 | en gros seulement |
| A, cuivre `#b4531a` | 46,9 | 49,3 points | 4,56:1 | oui |
| D, sarcelle `#0f5a5e` | 34,4 | 61,7 points | 7,21:1 | oui |
| C, vert profond `#1f5131` | 30,4 | 66,0 points | 8,41:1 | oui |
| B, bleu d'encre `#1e447e` | 29,2 | 67,3 points | 8,82:1 | oui |

**Le lime est a 4,9 points du fond.** Il brille et ne decoupe rien. L'oeil
recoit de la lumiere sans recevoir d'information, alors il insiste. C'est la
sensation decrite.

Deuxieme fait : le jaune-vert est la region du spectre que l'oeil percoit
comme la plus lumineuse. A saturation egale, c'est celle qui fatigue le plus
vite. Tous les guides de design sur la chartreuse disent la meme chose :
jamais en grande surface, jamais avec du texte clair, 10 % de la page au
maximum.

Troisieme fait, qui decoule des deux premiers : **le lime ne peut etre ni du
texte, ni un fond de bouton avec du texte dessus, ni un lien.** C'est
pourquoi il a fallu inventer un vert sombre a cote de lui, et c'est de la
que venaient les deux familles de vert qui se cognaient.

Un controle automatique l'a confirme. Sur dix verifications de contraste par
piste, les quatre nouvelles passent les dix. La palette actuelle en rate
trois, et ce sont exactement celles-la : accent sur le papier, accent sur la
carte, blanc sur l'accent.

## Ce qui ne change pas

Les quatre pistes gardent **un fond clair et des cartes blanches**. La clarte
qu'il aime ne bouge pas. Ce qui change, c'est que l'accent **descend** au
lieu de monter : il devient une couleur qui ecrit, qui souligne, qui porte un
bouton, au lieu d'une couleur qu'on ne peut poser nulle part.

## Les quatre directions

**A, Cuivre `#b4531a`.** La couleur de l'atelier : le metal chaud, l'outil, la
main. Elle rechauffe un fond clair sans l'eclairer. La plus vivante des
quatre, et la plus proche de la reference, mais posee plus bas pour qu'elle
decoupe.

**B, Bleu d'encre `#1e447e`.** La couleur du plan et du schema. Elle dit le
metier sans le crier. Le bleu est bas sur la courbe de sensibilite de l'oeil :
meme sature, il ne fatigue pas. Risque : c'est la couleur de tout le monde
dans l'informatique.

**C, Vert profond `#1f5131`.** Son idee de depart, posee au bon endroit. La
croissance reste, mais le vert descend de 91 a 30 de clarte : il passe de
lumiere a couleur.

**D, Sarcelle `#0f5a5e`.** Un vert qui a vu la mer. Il garde l'idee de
croissance en perdant le jaune, qui est la part du lime qui fait mal. Le plus
calme des quatre.

## La recommandation

**D, la sarcelle.** Elle repond a la plainte a la racine, puisqu'elle retire
le jaune, et elle garde le sens que Calixte voulait, puisqu'elle reste un
vert. Elle est plus rare que le bleu dans ce metier, donc elle distingue. Et a
7,2:1 elle ecrit partout, ce qui supprime d'un coup le besoin d'une deuxieme
couleur d'appoint.

**C en second**, s'il veut que la croissance se lise au premier coup d'oeil.

Le comparateur est dans `croquis/palettes.html` : la meme page, les cinq
palettes, un clic pour passer de l'une a l'autre. Rien n'a ete touche dans le
site tant que le choix n'est pas fait.
