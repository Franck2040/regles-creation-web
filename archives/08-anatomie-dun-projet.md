# 08 — L'anatomie d'un projet

> Écrit le 28/10 après la remarque de Calixte :
> « *pour chaque projet il faut que la personne puisse savoir qu'est-ce que tu voulais faire, quel est le problème que tu voulais résoudre, comment tu as fait pour résoudre le problème, quelles sont les petites difficultés que tu as rencontrées […] le temps que ça a pris, les captures, comment on a configuré* »
> « *mon portfolio doit parler à des admins système, à d'autres étudiants intéressés par mes labs et aussi à de simples RH qui ne connaissent même pas trop manipuler les outils du web* »

Ce document remplace toute improvisation de structure. **Chaque chapitre et chaque projet suit ce plan.**

---

## 1. Correction d'une règle que j'avais mal posée

Le 28/10 au matin j'avais écrit : *« pas d'adresses IP, pas de VLAN sur le site »*. **C'était faux, et trop large.**

Ce que Calixte a demandé, c'est de retirer **les noms de machines codés** — `PAR-DC-01`, `PAR-FS-01` — parce qu'ils n'apprennent rien à personne. Pas de retirer la matière réseau, qui est au contraire le cœur du métier qu'il apprend.

**La règle corrigée :**

| Interdit sur le site | Attendu sur le site |
|---|---|
| `PAR-DC-01`, `PAR-FS-01`, `PAR-ITSM-01` | **contrôleur de domaine**, **serveur de fichiers**, **serveur d'inventaire** |
| un nom de code en guise d'étiquette | le **rôle** en étiquette, **et l'adresse IP en dessous** |
| — | les **VLAN**, le **plan d'adressage**, les **ports**, les **flux**, les **versions** |

Un schéma réseau sans adressage n'est pas un schéma réseau, c'est un dessin. Un administrateur système qui regarde une architecture cherche d'abord le découpage, l'adressage et les flux — c'est exactement ce qu'il faut lui montrer.

**Dans le référentiel interne** (`docs/03`), les noms de machines restent : ils servent à ce que les schémas, les extraits et les captures concordent entre eux. Ils ne s'affichent simplement jamais en étiquette.

---

## 2. Les trois lecteurs, et comment un seul texte les sert tous

> « *admins système · étudiants intéressés par mes labs · RH qui ne connaissent même pas trop manipuler les outils du web* »

Ces trois personnes ne lisent pas la même chose. La réponse n'est pas d'écrire trois pages, c'est **d'empiler trois profondeurs dans une seule**, et de laisser chacun s'arrêter où il veut.

| | Ce qu'il cherche | Où il s'arrête | Il doit comprendre en… |
|---|---|---|---|
| **RH / recruteur** | « Est-ce qu'il sait faire le métier ? » | la carte : image, titre, résumé vert, durée, statut | **15 secondes, sans cliquer** |
| **Admin système** | « Est-ce qu'il a vraiment fait ça ? » | les schémas, le plan d'adressage, les flux, les extraits de configuration | 2 minutes |
| **Étudiant** | « Comment je refais ça chez moi ? » | les étapes, les ressources, les versions, le module outils et ses liens | il lit tout |

**Le mécanisme :** la profondeur se déplie, elle ne s'impose pas.
La carte parle au recruteur. « Voir les détails » ouvre le projet : contexte, objectif, rôle, schémas, résultat — niveau administrateur. Et à l'intérieur, les blocs **« Voir plus »** ouvrent la couche technique : plan d'adressage, flux, extraits de configuration, ressources, module outils.

Personne ne scrolle dans ce qui ne le concerne pas. C'est aussi ce qui tient la règle du *jamais de scroll trop long*.

**Conséquence d'écriture :** le résumé vert et le premier paragraphe ne contiennent **aucun nom d'outil**. Un recruteur RH ne sait pas ce qu'est Zabbix. Il sait ce que veut dire *« être prévenu d'une panne avant que l'utilisateur appelle »*. Les outils arrivent juste après, dans les logos de la carte — là où ils font leur effet sans bloquer la lecture.

---

## 3. Les questions d'entretien auxquelles chaque projet doit répondre

Calixte en a cité trois et m'a demandé de compléter. Voici la liste complète, et **la section de la page qui répond à chacune**. Si une case est vide, le projet est incomplet.

| # | La question posée en entretien | La section qui y répond |
|---|---|---|
| 1 | Qu'est-ce que vous avez fait ? | Titre + résumé vert |
| 2 | Quel problème vous cherchiez à résoudre ? | Le contexte |
| 3 | Pourquoi ce projet existait ? qui l'a demandé ? | Le contexte |
| 4 | Quel était le périmètre ? combien de machines, d'utilisateurs, de sites ? | Le contexte (chiffré) |
| 5 | Quel était **votre** rôle exactement ? seul ou en équipe ? | Mon rôle |
| 6 | Combien de temps ça a pris ? | Métadonnées (durée + période) |
| 7 | Comment vous avez planifié ? | Plan de gestion du projet |
| 8 | Quelle architecture, et pourquoi celle-là ? | L'architecture + schémas |
| 9 | Quelles solutions vous avez écartées, et pourquoi ? | Module outils (*pourquoi lui* / *sa limite*) |
| 10 | Avec quoi vous avez travaillé ? quelles ressources ? | Ressources matérielles et logicielles |
| 11 | Comment ça marche concrètement ? montrez-moi. | La mise en œuvre + extraits de configuration |
| 12 | Qui parle à qui, sur quels ports ? | Schéma de flux |
| 13 | Quel découpage réseau, quel adressage ? | Schéma réseau + plan d'adressage |
| 14 | Quelle difficulté vous avez rencontrée, et comment vous l'avez levée ? | Les défis |
| 15 | Comment vous avez vérifié que ça marchait ? | La recette — dans « La mise en œuvre » |
| 16 | Qu'est-ce qui reste à la fin ? c'est documenté ? | Le résultat |
| 17 | Et si le parc double ? si ça tombe ? | Les limites — dans « Le résultat » |
| 18 | Combien ça coûte ? licences ? | Ressources (colonne licence) |
| 19 | Qu'est-ce que vous en avez appris ? | Ce que j'en retiens |
| 20 | Et après ? | Ce que ça a ouvert → chapitre suivant |

**Les quatre questions que j'ajoute et qu'on oublie toujours :** la 12 (les flux et les ports — c'est la question qui sépare celui qui a monté le lab de celui qui a lu le tutoriel), la 15 (la recette : *comment vous savez que ça marche* — presque personne ne la prépare), la 17 (la montée en charge et la panne) et la 18 (le coût, que tout responsable finit par poser).

---

## 4. Le plan de page, dans l'ordre

> Révisé le 28/10 au soir. La première version empilait les blocs les uns sous les autres, puis une barre d'onglets à défilement horizontal. Les deux obligeaient à chercher. Voici ce qui les remplace.

**On arrive toujours par la bibliothèque.** Carte, clic, pop-up. Jamais de page de projet autonome.

**Le pop-up montre un résumé qui se suffit à lui-même.** Un visiteur pressé le lit en entier et comprend le projet : le besoin, ce qui a été fait, le résultat, ce que ça a ouvert. Il contient **trois schémas au maximum**, posés dans la lecture à l'endroit où ils expliquent quelque chose, chacun avec une légende.

**Les détails sont proposés au fil du texte.** Juste sous le paragraphe qui vient d'aborder un sujet, une ligne discrète annonce ce qu'on peut approfondir, avec un ou deux boutons. Jamais plus de deux à la fois, jamais de boutons là où rien n'a été abordé.

**Chaque bouton ouvre un second pop-up**, sur un seul sujet, avec une croix bien visible. On le referme et on reprend la lecture exactement où on l'avait laissée, puisque le premier pop-up n'a pas bougé.

```
┌─ LA CARTE ────────────────────────────────── niveau RH
│  image · numéro de chapitre · titre · résumé en vert
│  description · outils (logos) · « Voir les détails »
└─────────────────────────────────────────────
                    ↓ clic
┌─ LE POP-UP : LE RÉSUMÉ ───────────────────── niveau administrateur
│  couverture · chapitre · statut · titre · résumé vert
│  période · format · environnement
│
│  Le contexte          le besoin, le périmètre chiffré
│  L'objectif           le problème à résoudre
│  ▣ SCHÉMA 1           la chaîne fonctionnelle
│  L'architecture       le découpage et sa raison
│  ▣ SCHÉMA 2           le réseau, avec les adresses
│    → Plan d'adressage et flux
│  Mon rôle             ce que j'ai fait, et ce qu'ont fait les autres
│  ▣ SCHÉMA 3           le travail en trois étapes
│    → Étapes, recette et configurations
│    → Machines et logiciels
│  Le résultat          ce qui reste, et les limites assumées
│    → Voir les captures
│  Les outils           les logos, et pourquoi le chapitre n'en porte pas le nom
│    → Les outils comparés
│  Ce que j'en retiens
│  Ce que ça a ouvert   → le chapitre suivant
│  Ce qui venait avant  ← le chapitre précédent
└─────────────────────────────────────────────
                    ↓ clic sur une flèche
┌─ LE SECOND POP-UP ────────────────────────── niveau étudiant
│  un seul sujet · un bouton « Fermer » · Échap
└─────────────────────────────────────────────
```

**Les cinq rubriques de détail**, et pas une de plus :

| Rubrique | Ce qu'elle contient |
|---|---|
| Plan d'adressage et flux | le tableau d'adressage, le schéma de flux, les ports |
| Étapes, recette et configurations | les étapes dans l'ordre, les tests qui prouvent, ce qui a résisté, les extraits |
| Machines et logiciels | les machines et leur taille, les versions, les licences, le coût |
| Les outils comparés | un onglet par tâche, chaque outil avec sa raison et sa limite |
| Les captures | trois au maximum, légendées |

## 6 bis. L'écriture

**Aucun tiret quadratin dans le texte visible.** Une incise se construit avec des virgules, un deux-points, ou deux phrases. Le tiret est une facilité d'écriture qui finit par donner un texte haché.

| À ne pas écrire | À écrire |
|---|---|
| « une durée — le seuil tient cinq minutes — et une condition de reprise » | « deux paramètres. D'abord une durée : le seuil tient cinq minutes. Ensuite une condition de reprise. » |
| « sa collecte s'arrête — acceptable à quatre-vingts postes » | « sa collecte s'arrête. C'est acceptable à quatre-vingts postes. » |
| « libre — GPL » | « libre (GPL) » |

Pour séparer deux libellés dans une étiquette de schéma ou une ligne de méta-données, on utilise le point médian : *annuaire · DNS · attribution des adresses*.

## 5. Le jeu de schémas

> « *pour chaque projet on peut avoir plusieurs schémas : le schéma réseau, le schéma physique, le schéma de flux, le plan d'adressage, le plan de gestion, les ressources que j'ai utilisées* »

| Schéma | Ce qu'il montre | Obligatoire ? |
|---|---|---|
| **Schéma réseau** | le découpage logique : VLAN, adressage, routage, pare-feu | **oui** |
| **Plan d'adressage** | tableau rôle / VLAN / adresse / passerelle | **oui** |
| **Ressources** | matériel et logiciel, avec versions et licences | **oui** |
| **Schéma de flux** | qui parle à qui, dans quel sens, sur quel port | oui dès qu'il y a des agents, des serveurs ou de la sécurité |
| **Schéma physique** | où tournent réellement les machines — hyperviseur, hôtes, liens | quand le virtuel et le physique ne se ressemblent pas |
| **Plan de gestion** | le projet découpé en jalons, avec les durées | oui pour le chapitre 05, utile partout ailleurs |
| **Schéma fonctionnel** | la chaîne métier, lisible par un non-technicien | quand il explique mieux que le schéma réseau |

**Trois règles de forme :**
1. Tous en **SVG écrit à la main**, variables CSS du site, aucune image — net à tout zoom, modifiable au mot près, et ça pèse deux kilo-octets.
2. **Une étiquette = un rôle**, l'adresse en dessous en plus petit. Jamais un nom de code seul.
3. **Toujours une légende.** Un schéma sans légende suppose que le lecteur devine.

---

## 6. Les défis — comment en parler sans se rabaisser

> « *le but n'est pas de dire sur le portfolio que j'ai galéré, le but n'est pas de se rabaisser* »

C'est juste, et ma version précédente tombait dedans : j'avais écrit *« j'ai commencé à les ignorer »*. Ça raconte une lassitude, pas une compétence.

**La règle : on raconte l'obstacle technique et la décision qui l'a levé. Jamais l'état d'âme.**

| Ce qu'on n'écrit pas | Ce qu'on écrit |
|---|---|
| « j'ai galéré avec les seuils » | « un seuil instantané déclenche sur un pic normal — il fallait une condition de durée » |
| « au début je ne comprenais rien aux agents » | « trois systèmes, trois méthodes de déploiement : dépôt, paquet, stratégie de groupe » |
| « j'ai fini par abandonner et tout refaire » | « j'ai repris le nommage avant de continuer : un tableau de bord n'est lisible que si les machines portent leur rôle » |

La formule qui marche en trois temps : **le symptôme** → **la cause** → **la décision**. C'est exactement ce qu'un recruteur cherche à entendre, et ça ne dit jamais « j'étais perdu ».

Même chose pour « ce que je referais autrement » : ce n'est pas un regret, c'est un **ordre d'opérations corrigé**. *« Je commencerais par l'inventaire, puis la supervision »* est une phrase d'architecte.

---

## 7. Ce qui fait qu'un projet de lab se lit comme un vrai projet

Sans jamais prétendre que c'était en production :

- **un périmètre chiffré** — 80 utilisateurs, 3 sites, 2 systèmes d'exploitation ;
- **une durée** — trois semaines, pas « quelques temps » ;
- **une contrainte qui n'était pas négociable** — l'authentification doit survivre à la coupure du lien entre sites ;
- **des valeurs précises** — un seuil, une durée, un port, une version ;
- **une décision justifiée** — pourquoi celui-là et pas l'autre ;
- **un livrable** — ce qui reste quand on éteint : une documentation, des scripts, des tableaux de bord, une procédure.

Et le statut est écrit en clair dans le bandeau : *Réalisé en lab*. On ne s'en excuse pas, on le dit.
