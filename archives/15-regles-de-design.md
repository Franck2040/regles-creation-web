# Les regles de design du portfolio

Dites par Calixte le 31/10/2026. Elles valent pour toutes les pages.

## La palette : quatre couleurs, pas une de plus

> « les couleurs sont le vert, le blanc, le noir et le doré, pas d'autres couleurs, si des dégradés doivent être faits alors ça devra être des nuances de l'une de ces 4 couleurs »

> « après tout sur ce portfolio nous ne sommes pas dans un arc-en-ciel »

| | Valeur | Role |
|---|---|---|
| Vert | `#bce23a` `#a6d61f` `#4d7c0f` | l'accent, partout |
| Noir | `#141a12` | le texte, les boutons pleins |
| Blanc | `#ffffff` `#fdfdfb` | le fond, les cartes |
| Doré | `#efc01f` `#dfa50a` | **occasionnel** : le cube, le trace |

**Interdits repérés et corriges le 31/10** : le degrade bleu vers orange du
panneau « Ce que je fais », et le fond orange du visuel « Infrastructure
multisite ». Tout degrade est desormais une nuance de vert, de blanc ou de noir.

## Pas de pastille « point vert + texte »

> « il y a souvent des petits blocs de texte que tu utilises, généralement un point vert suivi du texte et dans un rectangle avec des bords très arrondis, enlève cela sur l'ensemble du site, ces choses sont typiques de l'IA, présente-les d'une autre façon »

Ce qui les remplace :
- **Titre de section** : un filet horizontal court, puis le mot en capitales espacees. Pas de point, pas de galet.
- **Etiquette flottante** : une micro-legende en capitales au-dessus d'une ligne forte, dans une carte a rayon modere. C'est le motif « OBJECTIF / Mastère en alternance », qu'il a lui-meme choisi.
- **Sous-titre de carte** : du texte, rien d'autre.

## Les marges

> « j'aime bien quand on laisse les marges gauche et droite libres, pour que le design se voie au centre entre ces marges-là »

Colonne centrale de 1180 px au maximum. Sur un ecran de 1440, il reste donc
130 px libres de chaque cote. Le contenu ne touche jamais le bord.

## Le respir entre les sections

> « la partie "Ce que j'ai construit" et le footer se collent, esthétiquement c'est horrible »

Entre deux sections, au moins 110 px sur grand ecran. Un pied de page ne
demarre jamais a moins de 120 px du bloc precedent.

## Le trace dore

> « les tracés dorés sont beaux, mais à toi-même de voir que c'est dispersé partout, de la mauvaise façon »

Un seul geste continu, pas deux morceaux poses au hasard. Il part au-dessus de
la tete, contourne le cube, boucle, passe **derriere** la statue et ressort en
bas a gauche. Il ne touche jamais la statue.

## La barre de navigation

> « à la place de ma photo directement sur la navbar tu peux mettre un cube doré ou vert, et quand la souris vient dessus, le cube s'anime et affiche mon profil, d'ailleurs je trouve cela mieux ainsi »

Un cube dore en 3D au centre de la barre, qui tourne lentement. Au survol il
accelere, s'ouvre, et la fiche de profil descend : photo, nom, formation,
LinkedIn et GitHub.

## Et la regle qui les commande toutes

> « avant de t'arrêter regarde bien toi-même, je ne veux plus avoir à te montrer des fautes de design de ce genre »

Avant de rendre une page : ouvrir le rendu, verifier les couleurs hors palette,
les chevauchements, les espaces entre sections, et la tenue aux largeurs
courantes. Ne pas lui faire relever ce qui se voit a l'oeil nu.

## Precisions du 31/10, deuxieme passe

**Les verts.** Lime et pomme, jamais d'olive.

| | Valeur | Role |
|---|---|---|
| Lime | `#c9f63f` | la clarte : pastille du titre, fleches, cube |
| Lime clair | `#d8fa6a` | la face eclairee du cube |
| Pomme | `#9ad02e` | la profondeur, les faces d'ombre |
| Feuille | `#3f6b0e` | le texte vert sur fond clair |

> « je veux un vert qui est semblable à la nature, la croissance »
> « le vert lime et le vert pomme sont pour moi les verts idéaux, le lime pour sa clarté »

Une pastille lime est **plate**. Pas de degrade du lime vers l'olive, pas
d'ombre interne qui l'assombrit. L'ombre, s'il en faut une, est portee et verte.

**Les petits blocs sont noirs ou verts, jamais blancs.**

> « les blocs comme "Terrain d'abord" ou "Ouvert aux échanges" doivent être soit vert soit noirs, mais pas blanc, j'ai dit le blanc est une couleur secondaire »

Le filet + capitales de la premiere passe ne convenait pas non plus : il lisait
comme un tiret. Un sur-titre, une etiquette, un compteur, un ruban, un bouton
rond sont des **blocs noirs** a texte blanc, avec le mot important en lime.
Le blanc reste le fond des grandes cartes de contenu, rien d'autre.

**Les deux boutons de l'accueil ont la meme couleur**, noirs tous les deux. Le
principal porte la pastille lime a fleche, comme « Voir le projet ».

**Le trace dore est devenu un anneau.** Une ellipse en perspective autour de la
statue : la moitie haute passe derriere, la moitie basse devant. Le cube de la
barre en est la pierre. Il ne croise aucun texte.

**Le cube de la barre est vert et enorme** : 92 px contre une barre de 56, il
deborde de 23 px en haut et en bas.

> « il doit être comme la perle sur la bague de mariage, donc bien plus grand que la nav bar »

**Le prenom ferme la page.** « Calixte » en tres grand sous le pied de page,
coupe par le bas.

**Piege technique a retenir** : un `filter` sur un element en
`transform-style: preserve-3d` l'aplatit. Le cube ne montrait qu'une face. Son
ombre portee doit vivre sur le conteneur, pas sur le cube.

## Troisieme passe, 31/10 : les blocs sombres et le sens des couleurs

**Ce que les couleurs veulent dire.** Il l'a explique, il ne faut plus le lui
redemander :

> « j'ai exigé le vert parce que ça symbolise la croissance, la croissance parce que je me cherche encore, je suis encore en quête d'opportunité, mais dans 5 ans la couleur changera parce que j'aurai déjà trouvé les opportunités »

> « j'ai ensuite ajouté le noir parce que le noir passe bien avec le vert, mais il y a aussi le vert foncé qui donne bien avec le vert clair »

Le systeme complet est donc : **vert, vert fonce, noir, blanc, et un peu de
dore**. Il avait restreint a trois couleurs pour simplifier, pas par gout.
Le vert fonce est pleinement admis, et c'est lui qui remplace le noir plat.

**Un aplat noir n'est pas un design.**

> « tout les boutons sont maintenant noirs, mais moi je veux que ces boutons soient beaux »

Releve dans Minux : ses surfaces sombres ne sont **jamais** `#000`. Elles vont
de `#1c1c1c` a `#404040`, et le noir pur ne sert qu'aux voiles. Son bouton
« Golden Hour » tient sur trois choses : un degrade diagonal qui se rechauffe
d'un cote, un **liseré interieur plus clair que le fond**, et une ombre portee
douce. Sans le liseré, la surface est plate.

Les trois fonds retenus :

```
--bloc        linear-gradient(118deg,#1e2a1b,#26331f 54%,#2d3a24)
--bloc-clair  linear-gradient(118deg,#2a3626,#323f2a)
--bloc-or     linear-gradient(118deg,#1e2a1b,#2c3422 46%,#473c21)
--rim         inset 0 0 0 1px rgba(255,255,255,.11), inset 0 1px 0 rgba(255,255,255,.10)
```

Le dore ne sert que sur **un seul bouton par page**, le principal, en echo au
cube que la statue tend.

## Ce qu'il attend de moi, et qu'il a fallu qu'il dise

> « j'me attends souvent aussi à tes propositions »
> « apprends à comprendre l'idée et ensuite équilibre les choses et fais un beau design, bien équilibré »
> « tu dois faire de vraies recherches sur les couleurs, les dégradés, moi je mets juste des références et des idées, toi tu dois les comparer, faire des tests et trouver ce qui sera le mieux »

Il donne des references et une direction. Le travail est de **chercher,
comparer, batir plusieurs variantes, puis recommander**, pas d'appliquer sa
derniere phrase au pied de la lettre. Une consigne prise litteralement donne
un resultat rigide, et c'est exactement ce qu'il reproche.

Methode retenue : quand une decision esthetique se pose, on construit une
planche de variantes cote a cote dans son univers, on explique ce que chacune
coute et apporte, et on recommande une. Il choisit.

## Quatrieme passe : la hierarchie des blocs

> « en fonction du bloc, certains doivent être des dégradés de noir, et d'autres des dégradés de vert foncé »
> « tous les boutons ne peuvent pas avoir la même couleur »
> « il faut bien hiérarchiser les choses et ne pas appliquer bêtement la même chose partout, chaque section doit se comprendre et montrer son design »

**Cinq familles, chacune avec un emploi.** Ce n'est pas une palette, c'est un
rang : on choisit la famille d'apres ce que l'element fait, pas d'apres son
aspect.

| Famille | Valeur | Emploi |
|---|---|---|
| **Encre** | `118deg, #151815 → #1e221d → #292e27` | les actions fortes : second bouton, « Voir le projet », le ruban, le compteur, la barre |
| **Forêt** | `118deg, #0d2114 → #153020 → #1c3d27` | ce qui touche a la croissance : bouton principal, adresse du pied |
| **Blanc travaille** | `152deg, #fff → #fbfcf8 → #f3f6ec` | ce qui se pose sur une image : cartes sur la statue, ronds, « Terrain d'abord » |
| **Gris** | `136deg, #f5f6f2 → #e6e9e0` | ce qui vit **a l'interieur** d'un bloc : « web », « automatisation », « sécurité », « design » |
| **Lime** | aplat `#c9f63f` | **une seule chose par ecran** : la pastille du titre, ou « Ouvert aux échanges » |

**Les liserés changent avec la famille**, c'est ce qui les distingue :
blanc a 12 % sur l'encre, lime a 22 % sur la foret, encre a 7 % plus une
lumiere blanche en haut sur le blanc travaille.

**Un titre de section n'est pas un galet.** « Ce que je fais », « Les
projets », « Me joindre » sont des **mots en degrade**, de l'encre vers le
vert, sans fond. Le galet noir de la passe precedente etait aussi rigide que
la pastille a point vert qu'il remplacait.

**Un noir de ce systeme ne tire jamais sur le bleu.** Les premiers que j'avais
poses etaient a 200 deg de teinte : un gris-bleu. Ils sont neutres ou penchent
vers le vert.

**Le prenom fait exactement la largeur de la carte du pied**, mesure au pixel.
Piege rencontre : un `display:block` donne toujours la largeur du conteneur,
donc le calcul de mise a l'echelle valait 1 et ne corrigeait rien. Il faut un
`inline-block` pour que la boite epouse le texte.

## Cinquieme passe : le noir est sans teinte

> « je vois une sorte de vert sur la nav bar dans le bouton "me contacter" ainsi que sur l'affichage de mon profil quand on hover sur le cube, ces choses doivent être en noir »

Mes « noirs » etaient `#151815 → #292e27` : une teinte verte a tres faible
saturation. Invisible sur une petite pastille, mais sur un bouton de barre ou
une fiche de profil entiere, ce soupcon de vert se voit.

**Un noir de ce systeme n'a aucune teinte** : `#161616 → #202020 → #2b2b2b`.
Le vert fonce reste une famille a part, pour le bouton principal et l'adresse
du pied, jamais pour une surface neutre.

**Le fond est blanc**, pas creme : `#fefefe`. Le quadrillage descend a 2,2 %
et les nuages a 10-27 % d'opacite, pour ne pas grisailler la page.

> « le background doit être plus blanc, au moins blanc à 97 % »

**Le prenom va d'un bord de l'ecran a l'autre**, pas de la largeur de la carte :
`width:100vw` avec `margin-left:-50vw`, et le script le cale sur
`documentElement.clientWidth`. Mesure : 0 px a gauche, 0 px a droite.

**Le cube s'ouvre.** Au survol, les six faces s'ecartent de leur centre, la
face du dessus devient translucide, et la fiche de profil sort par la breche
en grandissant depuis le cube.

> « pour l'animation du cube, on doit avoir l'impression que le cube tourne et s'ouvre pour laisser sortir mon profil »

## Le pied de page : une grille, pas un flex

Le pied etait en `flex` avec retour a la ligne. Des que le titre s'allongeait,
les trois colonnes de liens basculaient **sous** le bloc de gauche et tout se
tassait a gauche, avec la moitie droite vide.

Un pied de page se construit en **grille a deux colonnes**, dont les parts ne
dependent pas de la longueur du contenu :

```
.pied-haut { display:grid; grid-template-columns: minmax(0,.9fr) minmax(0,1.1fr) }
.colonnes  { display:grid; grid-template-columns: repeat(3, minmax(0,1fr)) }
```

Sous 860 px, une seule colonne et les liens sur deux.

**Typographie francaise** : une espace fine insecable (`&#8239;`) avant `?`,
`!`, `;` et `:`. Elle est correcte en francais **et** elle empeche le signe de
tomber seul en debut de ligne, ce qui arrivait sur « Un problème à poser ? ».

## Sixieme passe : le mouvement qui informe

**Le pied dit ce que je cherche, sans le dire deux fois.** Sous les chiffres du
rythme, une ligne « Recherche d'alternance en cours » dont la lumiere balaie le
texte, un rail avec un curseur lime qui va de « nov. 2026 » a « 2028 », et les
deux bornes en petites capitales. En deux secondes on sait quoi et pour quand.

**Le cube ne s'arrete jamais.** Rotation en 9 s au lieu de 19, flottement
vertical en 4,4 s, et une lueur lime qui pulse sous lui. C'est ce mouvement
continu qui dit qu'on peut cliquer, avant meme le survol.

> « quant au cube, il doit constamment être animé, pour que les visiteurs sachent qu'ils peuvent cliquer dessus »

Sous `prefers-reduced-motion`, rien ne s'arrete mais tout ralentit beaucoup
(rotation en 46 s, le reste en 12 s). Couper entierement supprimerait le signal
de clic ; ralentir le garde sans agresser.

**Du verre sur « automatisation »** : la pastille n'est plus un aplat lime mais
un verre teinte, `backdrop-filter: blur(16px) saturate(1.6)`, avec une lumiere
blanche en haut et un liseré interieur. On voit le quadrillage au travers.

**Ordre des projets** : n8n-veille-emploi-fr, puis TechFind, puis
Infrastructure multisite. Le pied suit le meme ordre.

## Reste a faire, decide le 31/10

Quand la page projets existera, les quatre etiquettes du panneau
« Ce que je fais » deviennent des declencheurs :

| Etiquette | Ce qu'elle montre |
|---|---|
| web | un apercu de TechFind, avec un bouton pour ouvrir le projet |
| automatisation | le projet n8n |
| securite | le chapitre 01, infrastructure |
| design | les trois premiers projets graphiques |

Il faudra aussi un signe visible que ces etiquettes sont cliquables.

**Piege a ne pas refaire** : un script qui annonce son succes sans verifier.
Le reordonnancement des projets avait « reussi » a l'ecran alors que le
remplacement n'avait rien trouve, parce que je joignais les blocs sans leurs
separateurs. Un script de patch relit le fichier ecrit et affiche le resultat
reel, jamais son intention.

## La page projets, 31/10

Trois familles, filtrables : **Infrastructure** (les six chapitres),
**Developpement** (n8n, TechFind, Health Tracker, EduSphere), **Design**
(les supports clients). Le compteur de chaque filtre se calcule tout seul.

**L'anatomie d'une fiche** reprend la hierarchie des blocs :

| Element | Famille | Pourquoi |
|---|---|---|
| la famille, sur l'image | gris | elle vit DANS la fiche |
| le numero de chapitre | encre | c'est une marque, elle doit tenir |
| les outils | lime pale | ce sont des faits techniques |
| l'etat (lab, client, en ligne) | texte seul | une mention, pas un bloc |
| la fleche | encre, devient lime au survol | c'est l'action |

**L'etat de chaque projet est dit.** « Réalisé en lab », « Projet de groupe »,
« Vérifié en débranchant », « En ligne », « Client ». On ne laisse pas croire
qu'une maquette a tourne en production.

**Piege rencontre, le meme qu'au pied de page** : un raccourci `padding` sur
une classe qui porte aussi `.lim` **efface le padding lateral de `.lim`**, et
le contenu vient coller le bord de l'ecran. On n'ecrit que les cotes qu'on veut
changer : `padding-top`, `padding-bottom`.

## Le fond kaki

> « je constate que le blanc est trop prononcé, du coup on va mettre un fond légèrement kaki, on diminue le blanc de 4 % »

`--page: #f7f6ee`. Teinte 53 deg, saturation 36 %, clarte **95,1 %**. Le kaki
est un dore tres desaturé : il reste dans la palette. Les cartes restent en
blanc pur, et c'est ce qui les fait ressortir du fond au lieu de s'y fondre.

Deux valeurs suivent : `--coquille: #f0efe4` et le blanc travaille, dont la
fin de degrade passe a `#f5f3e7`. Le gris des etiquettes se rechauffe aussi
(`#f4f3ea → #e4e2d4`), sinon il tirait au bleu sur un fond chaud.

## Les familles sur la page projets

> « lorsque tous les projets s'affichent ils doivent s'afficher clairement par sections, pour que ça ne se mélange pas »

Sur « Tous », les trois sections restent la, chacune avec son titre, sa phrase
et son compte. Rien ne se melange. Sur un filtre, les deux autres sections
disparaissent entierement, titre compris.

## Les adresses

Chaque famille a la sienne, et elle marche depuis l'exterieur :

| | Adresse |
|---|---|
| Infrastructure | `projets.html#infrastructure` |
| Developpement | `projets.html#developpement` |
| Design | `projets.html#design` |

Au chargement, la page lit l'adresse et ouvre la bonne famille. Un clic sur un
filtre met l'adresse a jour sans recharger, donc le lien se copie et se partage.

**Chaque fiche pointe vers la vraie page du projet**, prise dans les donnees du
site et non inventee : les six chapitres par leur slug
(`/projets/batir-une-infrastructure/` et les cinq autres), les projets par leur
id (`/projets/techfind/`, `/projets/biosense/`...).

Un cas particulier : **n8n-veille-emploi-fr n'a pas de page a lui**, il est
rattache au chapitre 05 dans les donnees. Sa fiche mene donc a
`/projets/deployer-et-automatiser/`. A trancher : soit il garde ce
rattachement, soit on lui fait sa propre page.

## Le confort de l'oeil : ce que disent les guides

> « l'arriere-plan ne donne pas tres bien avec les textes, avec les blocs verts et texte vert partout ça donne l'impression de faire mal aux yeux »

Il avait raison, et c'est documente :

- **Une couleur tres saturee sur une grande surface fatigue la retine.** Pour
  un ecran qu'on regarde longtemps, on reste en saturation faible a moyenne.
- **Le jaune est tres haut sur l'echelle de luminance**, donc difficile a
  marier avec du texte.
- **Le jaune sur vert** est une paire connue comme penible, en particulier pour
  les troubles de la vision des couleurs.
- Un blanc casse est plus confortable qu'un blanc pur : ca, on le gardait.

**Ce qui a change.** Le fond avait 9 points d'ecart entre le rouge et le bleu,
franchement jaune. Il passe a 5 : `#f7f6ee` devient **`#f6f5f1`**. Toujours un
blanc casse, mais sans le kaki.

Les pastilles vertes a texte vert deviennent neutres. Il ne reste qu'un seul
grand aplat colore, la carte du rythme dans le pied, et son texte tient le
contraste.

**Tous les couples verifies passent le niveau AA** (4,5:1 minimum) :

| | Rapport |
|---|---|
| texte sur fond | 15,2:1 |
| gris sur fond | 4,7:1 |
| vert feuille sur carte verte | 5,7:1 |
| etiquette grise | 12,1:1 |
| blanc sur encre | 16,3:1 |
| encre sur lime | 14,5:1 |

## Une icone seule ne dit rien

Les trois boutons ronds etaient en blanc travaille sur un fond presque blanc :
invisibles. Ils passent en **encre**, et **le nom apparait au survol** :
GitHub, LinkedIn, E-mail. Une icone que le visiteur ne connait pas n'est pas
un lien, c'est une devinette.

L'icone GitHub etait fausse, c'est maintenant la vraie marque.

**Les trois metiers** portent des icones larges plutot que des photos :
`ph-hard-drives`, `ph-brackets-curly`, `ph-pen-nib`. Celle du metier survole
passe en vert.

## Le rapport s'inverse : fond blanc, blocs kaki

> « le meilleur arriere-plan sera le blanc, donc remets l'arriere-plan en blanc »
> « peut-etre les blocs qui sont blancs maintenant deviendront legerement kaki, juste pour que le blanc d'un bloc ne cree pas la confusion avec le blanc de l'arriere-plan »

C'est exactement ce qu'il fallait faire, et il l'avait vu avant moi : si on
blanchit le fond sans toucher aux cartes, les cartes disparaissent.

| | Avant | Apres |
|---|---|---|
| Fond | `#f6f5f1` kaki | **`#ffffff`** |
| Cartes | `#ffffff` | **`#faf9f5`**, legerement chaud |
| Bord | 9 % | **12 %**, parce qu'un bord trop fin ne pose plus une carte sur du blanc |

La plus grande surface de l'ecran redevient neutre, ce qui est le plus
reposant, et la carte se detache par trois choses a la fois : 5,3 points de
clarte en moins, un bord a 12 %, et l'ombre douce. Aucune des trois ne suffit
seule.

Contrastes apres le changement, tous au niveau AA : texte sur carte 15,8:1,
gris sur carte 4,9:1, texte sur fond 16,6:1, gris sur fond 5,1:1.

## Une seule famille d'icones

Le bureau utilisait des SVG dessines a la main, le mobile des icones Phosphor.
Deux familles pour les memes liens. **Phosphor partout**, puisque le site la
charge deja : `ph-house`, `ph-briefcase`, `ph-user`.

Le bouton « Mon CV » rejoint la famille de la barre : fond transparent, un
bord a 12 %, comme le bouton de langue. Il etait en encre, donc il criait plus
fort que la navigation elle-meme.

## Le respir avant le pied de page

144 px de blanc entre la carte des competences et celle du pied : un trou, pas
un respir. Il passe a **82 px au maximum**. Un pied de page enchaine, il ne
ferme pas un chapitre.

## Le fond gris, et le verre vert

Troisieme essai de fond, et c'est le bon : **`#ededed`**, un gris neutre. Les
cartes redeviennent **blanc pur** et se posent dessus sans aucune aide. Le bord
peut meme redescendre de 12 a 10 %, puisque l'ecart de clarte fait le travail
tout seul.

Les trois essais, pour memoire : kaki avec cartes blanches (trop jaune), blanc
avec cartes kaki (les cartes se fondaient), gris avec cartes blanches.

**« Ce que j'ai construit » vit dans un panneau de verre vert**, la variante D
du comparatif, teintee :

```
background: linear-gradient(134deg, rgba(201,246,63,.30), rgba(154,208,46,.16) 54%, rgba(201,246,63,.22));
backdrop-filter: blur(20px) saturate(1.5);
box-shadow: inset 0 0 0 1px rgba(255,255,255,.55), inset 0 2px 0 rgba(255,255,255,.7);
```

Le verre a besoin de quelque chose derriere pour exister : sur un fond uni il
ne sert a rien. Ici le gris et les nuages passent au travers, et c'est ce qui
le fait tenir.

**Un seul style pour les trois metiers.** Avant, le premier etait vert et les
deux autres neutres : trois cartes de meme rang ne peuvent pas avoir deux
aspects. Elles sont identiques, et le vert arrive au survol.

**La pilule verte est un degrade**, du lime clair au pomme, avec une lumiere
blanche en haut. Un aplat vert ne tient pas face au reste.

**Les icones de la barre.** Elles n'avaient jamais ete posees sur les liens du
bureau : seules les versions mobiles en avaient. Accueil, Projets, A propos et
Contact portent maintenant les memes traits, a 45 % d'opacite pour accompagner
le mot sans le concurrencer.

## La lumiere n'est pas la meme partout

> « la meme lumiere et la meme intensite ne peuvent pas s'appliquer a tous les elements concernes »
> « je prefere qu'on ait l'impression que les lumieres sont bien positionnees, bien reglees, sans exagerer »

**La regle : plus la surface est grande, plus la lumiere est diffuse et
discrete.** Une pastille de deux mots peut porter un halo ; un panneau de
1100 px de large deviendrait une tache.

| Surface | Taille | Son traitement |
|---|---|---|
| pastille « automatisation » | petite, forte | liseré lumineux qui dessine la forme, halo exterieur, et une lueur sur le texte lui-meme |
| panneau de verre des projets | tres grande | **une seule** source, large et rasante, en haut a gauche. Aucun halo |
| carte du rythme, dans le pied | moyenne, calme | un filet de lumiere en haut, rien d'autre. Elle informe, elle n'appelle pas |
| pilule « Pret a saisir » | petite, active | liseré et halo moderes |
| fleche de remontee | minuscule, flottante | degrade clair, liseré, halo court |

**Les verts ont ete eclaircis**, pas assombris. Les fonds partaient de
`rgba(201,246,63,.30)` et montent a `rgba(219,250,124,.46)` : la couleur reste
la meme, c'est la quantite de lumiere qui change.

Les sur-titres (« Les projets », « Me joindre ») passent de 11,5 a 13,5 px :
ils annoncent une section, ils ne peuvent pas etre plus discrets qu'une
legende.


## Un element qui se repete ne porte pas de halo

Quatre jalons de parcours, trois cartes de poste, trois fiches : si chacun
porte son halo, la page compte dix lampes et on ne regarde plus rien.

**Un element unique peut appeler. Un element qui se repete se contente d'un
liseré.** Les pastilles du parcours gardent le degrade lime et le liseré
interieur, et s'arretent la. C'est le prolongement direct de la regle de la
taille : la repetition compte comme de la surface.

## Un grand bloc vert n'est pas un bouton vert

Le foret (`#0d2114 -> #1c3d27`) tient sur un bouton de 200 px. Sur un bloc de
500 px de large il devient une tache noire, et la paire encre + foret se lit
comme deux noirs.

Pour les grandes surfaces, le foret s'eclaircit : `#16331f -> #285736`. Les
deux faces de la page A propos recoivent alors chacune **une seule** source
rasante en haut a gauche, blanche sur l'encre, lime sur le foret. Meme regle
que le panneau de verre : une source, pas de halo.

## La mesure du texte

Une ligne de 110 signes ne se lit pas. Les blocs d'un seul tenant prennent une
largeur de lecture (900 px pour le parcours, 980 px pour les postes et la
recherche d'alternance) ; les grilles de cartes gardent les 1200 px de la
page. Deux largeurs differentes ne sont pas une erreur quand l'une porte de la
prose et l'autre des cartes.


## Le liseré de mise au point doit se voir

Tout le site utilisait `outline: 2px solid var(--accent2)` au clavier. Du
pomme sur du blanc fait **1,84:1** : la norme en demande 3. Qui navigue au
clavier ne savait pas ou il se trouvait.

Le liseré passe partout a `3px solid var(--feuille)` : 6,3:1 sur une carte
blanche, 5,4:1 sur le fond gris, 5,1:1 sur une pastille lime. Seul le bouton
fantome, qui vit sur de l'encre, garde le lime, qui y fait 13:1.

**Une couleur d'accent n'est pas une couleur de liseré.** Le lime sert a
attirer l'oeil sur une grande forme ; un trait de 3 px a besoin d'une couleur
qui porte, donc d'une couleur sombre.

## Une teinte chaude, une seule fois

Le message d'erreur du formulaire est le seul endroit du site ou une teinte
chaude est admise (`#76300f` sur `#fbefe9`, 8,5:1). Un echec annonce en vert
ne se comprend pas. Partout ailleurs la regle tient : vert, dore, neutre.


# La lumiere, apres mesure

Calixte : « jai a chaque fois limpression davoir des problemes de yeux, il y a
tellement de trucs sombres ». Au lieu de deviner, on a mesure sa capture et
celle du site de reference, pixel par pixel.

## Ce que la mesure a dit

| | reference | nous, avant |
|---|---|---|
| fond | #eeeeee, clarte 94,1 | #ededed, clarte 93,7 |
| noir franc | 3,5 % de l'ecran | 4,7 % |
| **gris sale** (sous la clarte du fond, sans etre noir) | **9,7 %** | **14,3 %** |

Le fond n'etait donc pas le probleme : il est le meme chez eux. Le noir non
plus. Le probleme etait une large zone grisee, un point ou deux sous la clarte
du fond, sur presque toute la page. Trois causes, trouvees en traversant
l'image :

1. **Les nuages du haut** descendaient a `#bababa`, dix-huit points de clarte
   sous le ciel, sur toute la largeur. Un nuage plus sombre que le ciel est un
   nuage de pluie.
2. **Le halo lime** de la pastille : de 89 a 93 de clarte sur soixante pixels,
   alors que le fond est a 93,7. En face, le halo de la reference va de 87 a
   94,1 en deux pas, et il est chaud.
3. **Le ciel lui-meme** : trois degrades lime a 8-12 % par-dessus le fond.
   Lime pose sur gris clair donne 93,3 contre 94,4. La page entiere etait
   grisee d'un point.

## La regle

**Une lumiere monte la clarte. Si elle la baisse, ce n'est pas une lumiere,
c'est une tache.**

Le lime pur est a 77 de clarte, le fond a 94. Un halo lime sur fond clair
salit, forcement. Sur le fond noir de la page 404, le meme lime a 77 eclaire :
c'est la clarte de ce qu'il y a dessous qui decide, pas la couleur du halo.

Les lueurs sont donc devenues blanches, a peine citronnees :

    --lueur:   0 0 48px -8px rgba(250,255,232,.95), 0 0 92px 6px rgba(255,255,255,.6)
    --lueur-c: 0 0 34px -10px rgba(250,255,232,.9), 0 0 62px 4px rgba(255,255,255,.5)

Et le ciel eclaire au lieu de teinter : trois sources blanches qui montent la
clarte vers 97 au lieu de trois teintes lime qui la descendaient a 93,3.

## Les autres regles de la meme serie

**Jamais d'ombre sur du texte.** Une ombre sous une lettre la rend floue, elle
ne la detache pas. Les quatre `text-shadow` du site sont parties.

**Les ombres restent sous les blocs blancs**, parce que c'est ce qui les pose
sur le fond, mais elles perdent la moitie de leur noir : `--pose` passe de
45 % a 22 %, `--pose-c` de 22 % a 12 %.

**Un bloc n'est pas un bouton.** Une encre de bouton (`#161616`) tient sur
40 px de haut. Sur un bloc de 500 px de large elle fait un trou : l'ecran des
deux faces de la page A propos comptait **29 % de noir franc**, contre 4 % sur
l'accueil. Les deux faces sont passees au graphite (`#35352f -> #4e4e47`) et
au vert de feuillage (`#235033 -> #336b48`) : 15 % de noir, clarte moyenne de
71,8 a 76,0.

**Un seul element vraiment sombre par ecran.** Le second bouton de l'accueil
etait une deuxieme encre a cote de la premiere. Il est blanc.

**Un blanc transparent n'est pas une couleur.** `rgba(255,255,255,.74)` tenait
4,5:1 sur l'ancien vert tres sombre et tombait a 3,6:1 sur le vert eclairci.
Le texte des blocs colores est passe en teinte pleine, `#eef7f0`, qui garde
son contraste quel que soit le fond.

## Le resultat, mesure au meme cadrage

| | avant | apres | reference |
|---|---|---|---|
| gris sale | 14,3 % | **10,9 %** | 9,7 % |
| noir franc | 5,2 % | **4,0 %** | 3,9 % |
| plus clair que le fond | 8,3 % | **33,3 %** | 14,9 % |

Le fond est passe de `#ededed` a `#f0efec` : un demi-point de clarte et trois
points de chaleur. Peu de chose, et ce n'etait pas la le probleme. C'est la
derniere colonne qui a change la page : il y a maintenant deux fois plus de
surface **plus claire que le fond** que sur le site de reference. C'est ca,
l'eclat.

Consequence a surveiller : le fond ayant monte, `--muted` est passe de
`#6b6f66` a `#676b62`, sinon le texte courant tombait a 4,46:1.


# La couleur d'accent remplit des formes, elle n'ecrit pas de mots

Calixte : « le noir se voit bien sur l'arriere plan actuel mais le vert se voit
tres mal, ca derange les yeux », « des textes de couleur gris ne se voient pas
tres bien, ca donne le genre de couleur qui donne envie de dormir ».

Mesure du vert tel qu'il ecrivait, sur une carte blanche :

| ou | couleur | contraste |
|---|---|---|
| contexte des projets, resume des chapitres, coches des listes | `--accent2` `#9ad02e` | **1,84:1** |
| fin du degrade des sur-titres | `#79ad16` | **3,0:1** |
| liens, annees, employeurs, icones | `--feuille` `#3f6b0e` | 5,7:1 |
| texte courant | `--muted` `#676b62` | 4,9:1 |

Le `#9ad02e` etait sur les cartes de projet, les cartes de chapitre, les
listes de la page projets, les modales. A 1,84:1 ce n'est pas un texte pale,
c'est un texte absent.

**La regle : le lime remplit, il n'ecrit pas.** Il garde les pastilles, les
panneaux de verre, les boutons et les icones posees sur de l'encre, ou il fait
11 a 13:1. Partout ou il ecrivait sur du clair, il passe au vert sombre.

    --feuille : #3f6b0e -> #2f5a0a    5,7:1 -> 7,3:1
    --muted   : #676b62 -> #50564c    4,9:1 -> 6,8:1
    sur-titre : finissait a #79ad16, finit a #44760f    3,0:1 -> 4,9:1
    toutes les ecritures en --accent2 passent a --feuille

Le fond monte en meme temps, de `#f0efec` a `#f4f3f0`, soit 94,4 a 95,8 de
clarte. La carte blanche se tient a +4,2 au-dessus, la ou la reference est a
+4,9 : elle se detache toujours, avec son bord et son ombre.

# La lumiere sur un chiffre

Releve sur le « 80+ » de la reference, en ne lisant que le trace et jamais les
contre-formes :

- dans le zero, la clarte passe de **0,8 en haut** a **80,6 en bas** ;
- la source est a **56 % en largeur**, posee **sous la ligne de base** ;
- horizontalement, le trace remonte de 1 a 43 puis redescend a 2 : c'est un
  foyer, pas une pente.

Donc : un `radial-gradient` pose sous le texte, clair au centre, eteint en
montant, et `background-clip: text`.

Chez eux le zero peut disparaitre a moitie : le « 8 » et le « + » suffisent a
lire. Notre nombre n'a que deux chiffres, et il porte une information. La
lumiere s'arrete donc a `#80837d`, soit **3,47:1** sur le fond, le minimum
d'un grand texte. Le chiffre reste lisible sur toute sa hauteur, et il
attrape quand meme la lumiere.

    .ck-compte b {
      background: radial-gradient(64% 94% at 58% 104%, #80837d 0%, #63665f 15%,
                  #3d403a 36%, #191c17 60%, #000000 80%);
      -webkit-background-clip: text; background-clip: text; color: transparent; }

L'effet grandit avec la taille. Leur « 80+ » fait 150 px, notre « 12 » en fait
44 a 62 : a cette echelle la lumiere se voit, elle ne spectacularise pas.


# Un seul vert

Calixte : « le bloc "les projets" n'est pas vraiment vert, en comparaison avec
le vert de la fleche, les verts sur la page sont trop differents », « ca fait
mal aux yeux ».

J'ai compte. **Cinquante-trois verts differents** dans la feuille de style, et
surtout **deux familles de teinte** qui n'ont rien a voir :

| famille | teinte | ou |
|---|---|---|
| lime | 73 a 92 | la pastille, les panneaux, les boutons, la fleche |
| emeraude | 133 a 144 | le bouton « Decouvrir », le pied de page, les deux faces |

Deux verts separes de soixante points de teinte, poses cote a cote, vibrent.
C'est optique, pas une question de gout : l'oeil cherche a les accorder et
n'y arrive pas. La mesure sur sa capture le disait : le panneau des projets a
**teinte 72**, la fleche juste a cote **teinte 75,6**.

## La regle

**Toutes les surfaces vertes du site sont douze pas d'une seule couleur.**

    #16240a  #1c2d0b  #243a0d  #2d4610  #355210  #406015
    #4b7116  #598217  #7eaf1d  #a3d926  #b5e634  #c6f641
    #cdf85a  #d3f96c  #dffb93  #e5fca6  #eafcba  #eefdc9
    #f2fbda  #f5fce4  #f8fbee  #fafcf3

La teinte glisse de 76 en haut de l'echelle a 90 en bas. Ce n'est pas une
entorse : un jaune-vert tres sombre vire a l'olive, et quatorze points de
teinte suffisent a le ramener a un vert franc. Au-dessus de 40 de clarte, la
teinte ne bouge plus.

Resultat mesure, apres : panneau **teinte 75,7**, fleche **teinte 75,5**. La
meme couleur, a deux clartes.

## Ce qui va avec

**Le texte pose directement sur le fond est noir**, pas gris. « je pars d'un
probleme », « Depuis 2022, Nemours » : ces lignes etaient en `--muted`. Elles
passent en `--text`, 15:1. Le gris ne sert plus qu'a l'interieur des cartes,
et il descend encore, de `#50564c` a `#474c42`.

**Le titre respire** : l'interligne passe de 1 a 1,1, et la note inclinee
s'ecarte de 20 a 34 px avec 18 px de moins vers le haut. Elle collait a
« reseaux, ».

**La barre de navigation se resserre** : 880 px au lieu de 1080 pour 762 px de
contenu. Il y avait 185 px de vide a chaque bout, il en reste 50. Et le cube a
maintenant **48 px de chaque cote** au lieu de 14 a gauche : il s'ouvre au
survol et mordait sur « A propos ».

**Les trois metiers** : au survol, le rond de la fleche verdit comme l'icone.
Un seul des deux changeait.


# Un survol global efface les boutons

Calixte : « quand on survole certains textes et qu'ils deviennent vert, ce
n'est pas tres visible ».

Le coupable tenait en trois lignes, tout en haut de la feuille de style :

    a:hover { color: var(--feuille); }

Elle s'applique a **tous** les liens. Or un bouton est souvent un lien :
« Decouvrir mes projets » est un `<a>` pose sur un vert tres sombre, « Voir le
projet » un `<a>` pose sur de l'encre, le courriel du pied de page un `<a>`
pose sur du vert sombre. Au survol, leur texte blanc devenait vert fonce sur
fond fonce. Invisible.

**La regle : un survol global ne doit toucher que les liens de texte.**

    a:not([class]):hover { color: var(--feuille); }

Un lien qui porte une classe est un composant : il a deja sa couleur, et cette
couleur tient compte de son fond. Un lien nu est du texte dans un paragraphe :
lui seul verdit.

# La barre de navigation, une seule structure

Elle en avait deux : une version bureau et une version telephone qui
repliait tout dans un menu burger, avec des liens en double et le cube
masque. Deux structures pour la meme barre, c'est deux fois les reglages et
deux fois les oublis.

Il n'y en a plus qu'une : trois destinations a gauche du cube, trois outils a
droite. **Sous 950 px, seuls les mots disparaissent.** Les icones restent, le
cube reste au milieu, rien ne se replie. A 375 px la barre mesure 351 px pour
214 px de boutons : elle tient sans deborder.

**La page ouverte porte le lime de « automatisation ».** C'etait un gris a
6 % qui ne disait rien. C'est maintenant la seule chose verte de la barre,
avec le meme degrade et le meme liseré que la pastille du titre : on sait ou
on est sans lire.
