# 01 — L'univers

## Le monde

Un jeune ingénieur vit dans les nuages.

Il est élégant — chemise blanche, cravate noire, veste en cuir noire, jean loose marron, mocassins. Ce n'est pas un costume de scène, c'est sa tenue de travail : il s'habille comme quelqu'un qui porte une responsabilité. Il n'est pas perdu là-haut, il y est **chez lui** : il y a installé ses affaires, il y a construit quelque chose. Et il y cherche des opportunités — le cube doré.

Le cloud n'est pas une métaphore décorative. C'est le métier. C'est le seul cas où le monde du portfolio et la fiche de poste disent exactement la même chose.

Le visiteur ne regarde pas ce monde : **il y entre**. Il doit s'y sentir bien. Il doit avoir envie d'y rester, et en repartir avec le sentiment d'avoir rencontré quelqu'un, pas d'avoir lu un CV.

## Les lieux

Chaque page est un endroit de ce monde, pas une rubrique de menu.

| Lieu | Page | Ce qu'on y trouve | Sensation visée |
|---|---|---|---|
| **L'arrivée** | Accueil | Lui, debout sur son nuage, la main tendue vers le cube doré | On arrive. On lève les yeux. |
| **La bibliothèque** | Projets | Son savoir rangé, classé, consultable. Les chapitres sont des rayonnages. | De l'ordre. Beaucoup de travail accumulé. |
| **L'atelier** | À propos | D'où il vient, ce qui l'a construit, les gens qui l'ont formé | De l'intime. On comprend qui il est. |
| **Le poste de pilotage** | Compétences | Les instruments. Ce qu'il sait faire, lisible d'un coup d'œil. | De la maîtrise. |
| **La terrasse** | Contact | L'endroit d'où on parle au sol. Le message part d'ici. | De l'ouverture. Une main tendue. |

> La bibliothèque et l'atelier sont les deux lieux de Calixte. Le poste de pilotage et la terrasse sont des extensions proposées — à valider.

## L'altitude comme navigation

On **monte**. Le scroll n'est pas un défilement, c'est une ascension.

- Le sol (le passé, Yaoundé, les débuts) est tout en bas et apparaît dans la brume.
- La couche nuageuse, c'est le présent : le travail, les projets.
- Au-dessus, le ciel dégagé : le cloud, le Mastère, ce qui vient.

Chaque page a une altitude. Changer de page, c'est changer de niveau — et la transition doit le faire sentir. Plus on monte, plus l'air est clair, plus les contrastes s'adoucissent, plus la lumière est haute.

Conséquence concrète : **la perspective atmosphérique gouverne toute la mise en page.** Ce qui est loin est plus clair, moins contrasté, plus flou. Ce qui est proche est net et dense. C'est ce qui fait qu'un ciel paraît vrai, et c'est exactement ce qu'une IA ne fait pas quand elle empile des blocs.

## Le niveau d'exigence — à lire avant d'écrire la moindre ligne

Ce que Calixte reproche aux IA, et qui est mérité : on demande un univers, elles livrent des rectangles avec des images dedans et appellent ça un design.

Le repère qu'il a donné, en substance : *un portfolio de pilote où les nuages sont dessinés détail par détail, l'herbe, les oiseaux, l'avion qui passe ; on scrolle, ça zoome sur le pilote ; on continue, il dézoome et prend de la vitesse ; un globe affiche ses trajets ; il atterrit sur une nouvelle carte ; et la page contact, c'est lui qui reçoit l'appel de la base.* Ce n'est pas le sujet qu'il veut — c'est le **niveau de fabrication** qu'il veut.

Ce que ça implique, noir sur blanc :

1. **Ce qui n'existe pas, on l'écrit.** Il n'y a pas de composant npm pour « une couche de nuages en perspective atmosphérique qui se sépare quand on monte ». Ça se code au pixel. Pas de librairie trouvée sur internet pour tenir lieu de création.
2. **Pas de placeholder.** Pas de bloc gris « image ici ». Si un nuage doit être là, il est dessiné.
3. **La matière compte.** Grain, lumière, dégradés dirigés, ombres portées cohérentes avec une source lumineuse unique. Un ciel plat est un ciel raté.
4. **Le mouvement raconte.** Si ça bouge sans raison, on l'enlève. Si ça monte, ça doit vouloir dire quelque chose.
5. **Le code reste maintenable.** C'est un portfolio d'admin sys : un site qui rame prouve le contraire de ce qu'il affirme.

## Les garde-fous — là où l'univers peut se retourner contre lui

Un monde de nuages peut basculer en deux secondes du côté naïf. Trois règles non négociables :

1. **Le nuage est une profondeur, pas un sticker.** Des couches, de la brume, de l'air entre les éléments. Jamais un nuage de dessin animé répété.
2. **Le cube doré est rare.** C'est la seule touche chaude d'une palette blanche et lime. S'il apparaît partout il ne vaut plus rien. Une fois, au bon endroit, il devient un symbole.
3. **Un seul personnage, peu d'apparitions.** Sa silhouette est l'unique élément figuratif du site. Omniprésente, elle devient une mascotte.

Et la règle qui prime sur les trois : **ça doit rester navigable.** La v1 a réussi ça, c'est son acquis le plus précieux. Un recruteur pressé doit pouvoir atteindre un projet en deux clics, sans attendre une animation ni comprendre une métaphore.

## Contraintes techniques héritées

- Export **statique** (`output: 'export'`) sur LWS : pas de serveur, pas d'API. Tout est HTML/CSS/JS.
- Les couleurs et le style actuels sont **conservés** : fond clair, accent lime, cartes blanches, rayons doux.
- Budget de poids à tenir : le site doit rester rapide sur mobile 4G.
- `prefers-reduced-motion` respecté : l'univers doit rester lisible sans animation.

## Pistes de fabrication (à explorer, non arrêtées)

- Nuages procéduraux en SVG (`feTurbulence` + `feDisplacementMap`) plutôt qu'images : légers, nets à toute résolution, animables.
- Couches de parallaxe pilotées par `scroll-driven animations` en CSS natif — pas de librairie JS d'animation.
- Transitions de page via l'API `View Transitions` : le changement de lieu devient un déplacement, pas un rechargement.
- Le cube doré en CSS 3D, facettes et reflets peints à la main. Pas de WebGL : trop lourd pour ce qu'il apporte ici.
- Grain et lumière en overlay léger, pour casser le « plat » du dégradé.

> À vérifier au moment de coder : support navigateur réel des scroll-driven animations et de View Transitions, avec repli propre. Les articles de tendance 2026 les annoncent généralisés ; ça se vérifie sur caniuse, pas sur un blog.
