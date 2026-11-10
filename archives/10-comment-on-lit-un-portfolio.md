# 10 — Comment les gens lisent vraiment un portfolio

> Écrit le 29/10, à partir de ce que Calixte a décrit en détail. Ses mots exacts sont dans
> [`docs/00-paroles-de-calixte.md`](00-paroles-de-calixte.md), section « Sur la façon dont les gens lisent réellement un portfolio ».
>
> **Ce document prime sur tout le reste en cas de désaccord de mise en page.** Les règles d'écriture
> de `docs/08` restent valables, mais elles s'appliquent à un texte que personne ne lira en entier.

---


> ## ⚠ La règle qui prime sur toutes les autres
>
> **On ne se justifie pas, et on n'explique pas un livre.** Sujet, verbe, complément.
> Un fait, un chiffre, un résultat. Puis on s'arrête.
>
> « *2 Go de RAM pour les pare-feu, 4 Go pour le serveur de fichiers* » se suffit.
> Expliquer pourquoi on a choisi ces chiffres, ce que ça apprend, ce que ça prouve :
> personne ne l'a demandé. Calixte a dû le redire quatre fois entre le 28 et le 29 octobre.
>
> **Le test, avant d'écrire une phrase :** est-ce qu'elle dit un fait, ou est-ce qu'elle
> défend une décision devant quelqu'un qui n'a rien demandé ? Si c'est la seconde, elle
> disparaît. Et même quand une phrase dit un fait, si elle peut être plus courte, elle
> l'est.
>
> **Les tournures interdites**, parce qu'elles annoncent toujours une justification :
> « c'est une méthode, pas… », « ce qu'on obtient en échange », « la contrainte apprend
> quelque chose », « ce qui est précisément la question qu'on pose à… », « et c'est une
> réponse qu'il vaut mieux avoir préparée », « ce n'est pas X, c'est Y ».
>
> Le visiteur vient voir **ce qui a été fait et le résultat**. Celui que ça intéresse
> cherchera ensuite comment. Les autres, s'ils lisent un paragraphe de défense, se
> demandent devant qui on se défend.


## 1. Le fait de départ

**Personne ne lit un portfolio.** Pas par mépris : parce qu'il y a quatre pages à visiter, que le visiteur est pressé, et que la plupart du temps ce n'est pas son métier.

Il faut écrire en sachant cela, et non en espérant le contraire.

---

## 2. Les deux visiteurs, et ce qu'ils font réellement

### Le visiteur d'un autre domaine (le cas le plus fréquent)

Une personne du marketing, une personne des ressources humaines. Elle ne code pas, elle ne connaît pas GitHub, elle ne saura pas ce qu'est un VLAN.

Son parcours, dans l'ordre :

1. L'accueil, parcouru en diagonale pour comprendre le domaine, pas pour le lire.
2. Un jugement immédiat : **la présentation, la vitesse, la beauté.**
3. La page projets, par curiosité. Elle scrolle d'abord **jusqu'en bas** pour voir s'il y a des animations cachées.
4. Elle remonte, et clique sur un projet **au hasard**. Pas pour comprendre : pour voir ce qui se passe quand on clique.
5. Un deuxième projet, pareil.
6. Dans le projet, elle ne lit pas le début. Elle scrolle jusqu'à la fin pour voir s'il y a quelque chose d'intéressant. Si elle ne voit **que du texte**, elle ne lira rien.

Ce qu'elle lira, au mieux : **le début du premier paragraphe, un paragraphe du milieu, le début de la conclusion.**

Ce qu'elle retiendra : **rien du projet, et tout de l'impression.**

### Le visiteur du même domaine

Lui peut décider de lire un projet. Mais :

- **Trois pages de texte sans image, il ne lit pas.** Il part.
- **Deux pages avec des images, il lit vite pour arriver à l'image.**
- Les schémas sont ce qui le convainc qu'il ne perd pas son temps.
- Devant un schéma, il vérifie trois choses : **est-ce qu'un texte déborde, est-ce que les blocs se voient, est-ce que ça a du sens.**
- Et la phrase qu'on vise : *« c'est tellement propre et bien fait, comment ce monsieur a-t-il fait ces schémas ? »*

**Le long texte chasse. L'image retient.**

---

## 3. Les règles qui en découlent

### Règle A — la lecture peut commencer n'importe où

Un visiteur n'entre pas par le début. Chaque bloc doit donc se tenir seul, sans dépendre du paragraphe précédent. Un titre qui ne se comprend que si on a lu ce qui précède est un titre raté.

### Règle B — un titre est une question qu'on se pose, pas une étiquette

C'est l'exemple que Calixte a donné, et il est parfait :

| Titre raté | Titre qui accroche |
|---|---|
| « Ce que j'aurais pu utiliser à la place » | **« GLPI est-il le seul outil pour inventorier un parc ? »** |

Le premier ne dit rien à qui n'a pas lu. Le second attrape immédiatement quelqu'un du métier, qui voudra savoir ce qu'on a à répondre.

**Donc : les titres de section portent une question ou une promesse concrète.** Jamais une abstraction.

### Règle C — une conclusion tient en une phrase simple

Si personne ne lit, une conclusion de quatre lignes ne sert à rien. Une phrase courte et compréhensible, oui.

| Avant | Après |
|---|---|
| « Que la valeur d'une supervision ne se joue pas à l'installation mais au réglage, et que l'ordre des opérations compte autant que les opérations : je commencerais par l'inventaire… » | **« C'est le réglage des seuils qui fait la valeur d'une alerte, pas l'outil. »** |

### Règle D — tout doit se lire en deux minutes

Un projet entier, schémas compris, se parcourt en deux minutes. Ce qui dépasse va dans un pop-up de détail.

### Règle E — un bouton doit se voir comme un bouton

Certains visiteurs ne comprennent même pas qu'un élément est cliquable. Donc : fond plein et foncé, texte blanc, **un verbe à l'infinitif** (« Voir le plan d'adressage ») plutôt qu'un nom (« Plan d'adressage »), et une flèche.

### Règle F — un bloc blanc sur fond blanc n'existe pas

Ce qui doit être vu vite doit être **coloré**. Le vert du site est la couleur qui attire l'œil : on l'utilise pour l'information que le visiteur doit percevoir en une seconde.

### Règle G — une vraie bordure, pas une ombre

Un cadre de schéma se traite **comme un cadre de photo** : une bordure nette, visible, d'un gris franc. Pas une ombre interne, qui ne se voit pas.

### Règle H — le schéma est l'argument, pas le texte

Le texte accompagne le schéma, jamais l'inverse. Si un passage peut devenir un schéma, il devient un schéma.
Et un schéma dont un texte déborde détruit l'effet recherché : **vérifier le débordement à chaque fois, sur petit écran compris.**

### Règle I — une étiquette doit se lire sans effort

Une étiquette de 10 px en majuscules espacées fatigue les yeux avant d'être lue. Un mot qui nomme un bloc important se met en 14 px, en gras, dans une couleur franche, avec un repère coloré devant.

> « cela a empeu stréssé mes yeux quand jessaiyais de les lire »

### Règle J — un bloc de schéma doit se détacher de son fond

La bordure du thème clair du site est à 12 % d'opacité. Sur le fond gris d'un cadre de schéma, elle disparaît. Les schémas redéfinissent donc leurs propres couleurs, plus franches, dans `DiagramFrame.tsx`. Avant de livrer un schéma, vérifier que **chaque** bloc se voit en un coup d'œil, les en-têtes de VLAN et les cartes d'étape compris.

### Règle K — on nomme ce dont on parle

Jamais « trois outils tiennent les trois rôles de la chaîne ». On écrit lequel fait quoi : *GLPI inventorie le parc. Zabbix mesure l'état des serveurs. Wazuh lit les journaux de sécurité.*

Et on dit aussi ce que les autres entreprises utilisent, parce qu'un visiteur du métier reconnaît d'abord ce qu'il connaît déjà.

### Règle L — on informe, on ne se justifie pas

« C'est ce qui prouve qu'un choix a été fait, et non subi » est une phrase de plaidoirie. Sur un portfolio, dire une chose suffit à l'assumer.

> « par defaut si nous disons quelque chose sur le portfolio cela est deja notre avis »

### Règle M — une phrase ne parle jamais du portfolio lui-même

« Les deux outils qu'on confond le plus souvent **sur cette page** » n'a aucun sens pour le lecteur : la page, c'est le portfolio. On écrit *« Zabbix et Wazuh sont souvent confondus »*, qui parle du métier et non du site.

### Règle N — les logos avant les mots

Les gens cliquent sur ce qu'ils reconnaissent. Les outils du chapitre sont donc montrés **en haut**, avec leur logo, avant le moindre paragraphe. Au survol de l'un d'eux : pourquoi lui, les alternatives connues, et un bouton qui descend à la comparaison complète.

### Règle O — on doit pouvoir sauter

Une barre fine à droite du pop-up numérote les sections, suit le défilement, donne le titre au survol et y amène au clic. Elle disparaît sous 900 px.

---

## 4. Ce qu'il faut corriger dans ce qui existe

| Ce qui existe | Pourquoi ça ne va pas | Ce qu'on fait |
|---|---|---|
| Bloc « en bref » blanc cassé | invisible sur fond blanc | fond vert, comme le bloc résultat |
| Cadres de schéma à ombre interne | l'ombre ne se voit pas | vraie bordure, nette |
| « Ce que j'aurais pu utiliser à la place » | ne dit rien à qui n'a pas lu | une question : « *GLPI est-il le seul outil pour inventorier un parc ?* » |
| « Ce que j'en retiens » (4 lignes) | trop long pour une conclusion | une phrase |
| « Ce que ça a ouvert » (4 lignes) | idem | une phrase, plus le lien vers le chapitre suivant |
| Boutons au nom abstrait | on ne voit pas que c'est cliquable | un verbe : « Voir… », « Ouvrir… » |
| Titres du type « Le contexte », « L'objectif » | étiquettes neutres | des questions concrètes |

## P — un logo se pose nu

Les fichiers officiels sont déjà détourés : la forme seule est visible, sans fond.
On ne les enferme donc **ni dans un cadre, ni dans une pastille de couleur**.

Et un outil dont le logo n'est pas encore posé ne reçoit **rien du tout** : son nom se lit seul.
Deux lettres dans un carré coloré ne sont pas un logo, elles en ont seulement la forme,
et c'est exactement ce qui fait hésiter l'œil une demi-seconde de trop.

## Q — on décrit avant de juger

Un outil se décrit avant qu'on dise quoi que ce soit sur lui : qui l'édite, sous quelle
forme il arrive, ce qu'il fait, comment on s'en sert. Sans ce paragraphe, « pourquoi lui »
ne veut rien dire, et la phrase tiendrait aussi bien pour trois autres outils.

Le détail compte : « inclus dans le système » ne veut rien dire, « livré avec Windows »
veut dire quelque chose. Le mode d'emploi complet est dans
[docs/12-comment-on-decrit-un-outil.md](12-comment-on-decrit-un-outil.md).

## R — un titre est une promesse, le texte la tient

Un titre qui pose une question reçoit sa réponse dès la première phrase, et cette
réponse porte sur **ce que le titre a demandé**, pas sur ce qu'on avait envie de
raconter. « GLPI est-il le seul outil pour inventorier un parc ? » appelle les noms
des autres outils d'inventaire, pas la liste de ce que j'ai utilisé.

La vérification se fait à l'œil : si l'image posée sous le titre montre autre chose
que ce que le titre annonce, c'est l'image qui ment, et le lecteur la croit elle.

## S — une conclusion oppose deux choses réelles

« C'est le réglage qui compte, pas l'outil » est une fausse opposition : sans l'outil
on ne règle rien, et chaque outil se règle à sa façon. Une conclusion nomme ce qui a
changé, avec le chiffre ou le paramètre qui l'a fait changer, et elle reste vraie si
on la relit à voix haute devant quelqu'un du métier.

## T — un laboratoire ne découvre pas une vraie entreprise

Le travail a eu lieu sur une machine, seul ou avec des camarades. On n'écrit donc
jamais « j'ai trouvé des comptes oubliés » comme si une entreprise réelle avait été
auditee. On écrit la situation telle qu'elle se présente : « le jour où l'inventaire
fait remonter des comptes qui… ». Le scénario reste entier, la compétence aussi, et
rien n'est inventé.

## U — un sigle s'explique sur place

Tout outil est présenté par son **type de service** : un ITSM, un NMS, un SIEM, un EDR,
un IGA. Et chaque sigle est reconnu à l'affichage, souligné, et ouvre au survol — au
premier appui sur téléphone — une fiche en trois temps : ce que c'est, à quoi ça sert,
qui en fait, avec les éditeurs européens nommés en premier.

Le glossaire est dans [`site/src/data/glossary.ts`](../site/src/data/glossary.ts) :
une entrée suffit, le texte des chapitres n'a rien à déclarer.

## V — un paragraphe long se replie

Au-delà de deux ou trois lignes, un paragraphe se coupe à la fin d'une phrase et se
termine par un « voir plus ». Le lecteur choisit d'entrer ou non : un mur de texte
fait fuir avant d'être lu.

## W — les ressources se disent en chiffres

« Un gigaoctet par pare-feu, deux par serveur, des disques de 25 à 40 gigaoctets. »
C'est tout. On n'explique pas pourquoi, on ne dit pas ce que ça apprend, on n'annonce
pas que c'est une méthode.

## X — on prend la version mûre, pas la dernière

Windows Server 2022 et non 2025, Ubuntu 22.04 et non la dernière sortie, ESXi 7.0 Update 3.
La règle vaut pour tous les chapitres, et quand une version apparaît dans un tableau, c'est
celle-là. Le dire une fois dans le chapitre concerné suffit : ça se lit comme une décision,
pas comme du retard.
