# 18 — Dossier de reprise

> **À lire en premier.** Ce fichier existe pour qu'un assistant qui arrive sur
> ce projet, ou moi-même après une coupure, puisse reprendre sans faire
> recommencer à Calixte des explications qu'il a déjà données dix fois.
>
> Il ne remplace pas les autres documents : il dit ce qu'ils contiennent et
> où tout se trouve. En cas de désaccord entre deux documents,
> `00-paroles-de-calixte.md` tranche, parce qu'il contient ses mots exacts.

---

## 1. Dans quel ordre lire

| # | Fichier | Ce qu'on y trouve |
|---|---|---|
| 1 | `docs/00-paroles-de-calixte.md` | ses phrases exactes, non corrigées. **La source.** |
| 2 | `docs/18-dossier-de-reprise.md` | ce fichier : qui, quoi, où, comment |
| 3 | `docs/15-regles-de-design.md` | toutes les règles visuelles, avec les mesures qui les ont imposées |
| 4 | `docs/16-implementation-refonte.md` | ce qui a été fait page par page |
| 5 | `docs/01-univers.md` | l'univers des nuages, la vision |
| 6 | `docs/02-architecture-projets.md` | pourquoi les projets portent ces noms |
| 7 | le reste | au besoin, voir le tableau du §6 |

Avant d'écrire la moindre ligne de Next.js, lire `site/AGENTS.md` : cette
version de Next n'est pas celle des modèles de langage, la documentation
officielle est dans `site/node_modules/next/dist/docs/`.

---

## 2. Qui est Calixte

**Kenmeugne Calixte Franck.** Étudiant en Mastère Cybersécurité & Cloud à
l'IMIE Paris, promotion **2026–2028**. Il vit à **Nemours, Île-de-France**.

| | |
|---|---|
| e-mail | `[adresse e-mail retirée]` |
| GitHub | https://github.com/Franck2040 |
| LinkedIn | https://www.linkedin.com/in/kenmeugne-calixte/ |
| Behance | https://www.behance.net/franckkenmeugne |
| école | https://www.imie-paris.fr/mastere-cybersecurite-cloud-computing-reseaux/ |

**Son parcours**, dans l'ordre : GCE Advanced Level (très bons résultats en
mathématiques pures et approfondies) → Université de Yaoundé 1, 2022, trop
théorique pour lui → formations pratiques en parallèle (développement web avec
Evariste Fomena, maintenance informatique avec le club COMSAS et Hanga
Francois) → **Keyce Informatique, 2023–2025** (C++, C#, React avec Evarist
Fomekong ; CCNA avec Romuald Djam) → **IMIE Paris**, Bachelor Administration
Systèmes, Réseaux et Cybersécurité 2025–2026, puis le Mastère.

**Ce qu'il cherche :** une **alternance** en administration systèmes et
réseaux ou en cybersécurité, à partir de 2026. Un stage conventionné de trois
mois reste possible. Disponibilité annoncée sur le site : **novembre 2026**.

**Ses expériences :** tuteur en mathématiques et informatique (sept. 2023 –
juin 2024), chef de projet étudiant chez Keyce (2023–2025), **graphiste
indépendant depuis 2023** (identités visuelles, pitch decks, flyers, menus).
Ce dernier point compte : le design n'est pas un loisir, c'est un métier qu'il
exerce.

**Langues :** français maternel, anglais courant (scolarité primaire et
secondaire en anglais). Les deux versions du site sont donc deux écritures
réelles, pas une traduction.

**Certifications :** Google IT Support Fundamentals, Bits and Bytes of
Computer Networking, Cisco Hardware Basics.

**Sa machine :** Windows 11 Home, **16 Go de RAM**. Toute proposition qui
demande plus est hors sujet. Il cherche systématiquement les outils gratuits
ou très peu chers, et il le dit.

**Son CV :** à partir de maintenant il n'y en a plus qu'**un seul** sur le
site, celui d'administrateur systèmes et réseaux. Le PDF doit être remplacé
quand il le fournira.

---

## 3. Les règles absolues

Elles ne se discutent pas. Elles viennent de lui, souvent répétées.

[Référence à un emplacement local retirée de cette édition publique.]
d'origine, ailleurs sur la machine, ne se touche jamais. C'est sa phrase :
[Référence à un emplacement local retirée de cette édition publique.]
changer le code source ».

**Un projet porte le nom d'une compétence, jamais celui d'un outil.** « avoir
un seul projet où je parle de GLPI c'est ça qui est nul » : le recruteur doit
retenir *gérer un parc*, pas *GLPI*. GLPI n'est qu'un outil parmi d'autres.

**Les projets d'infrastructure sont des chapitres.** Ils s'ouvrent en pop-up
depuis leur carte, jamais sur une page à part.

**Pas de nom de machine codé.** On écrit *serveur de fichiers*, *serveur DNS*,
pas `PAR-DC-01`. En revanche les **adresses, les VLAN, les ports et les
versions doivent apparaître** : c'est ce qui prouve que le travail a eu lieu.

**Trois publics à la fois :** l'administrateur système qui vérifie, l'étudiant
qui apprend, et le recruteur qui ne connaît pas les outils du web. Chaque page
doit parler aux trois.

**Les versions sont celles qui ont fait leurs preuves,** pas les dernières :
Windows Server 2022 et non 2025, Ubuntu 22.04, ESXi 7.0 U3.

**La vérité du labo.** Il a travaillé seul, parfois avec les machines de
camarades. On n'écrit jamais comme si une entreprise avait été auditée. Et
« je ne veux pas jouer la pitié de l'étudiant lambda » : on ne s'excuse pas
d'être étudiant non plus.

---

## 4. Comment il veut qu'on écrive

**La règle qui prime sur toutes les autres :**

> « on ne se justifie pas bêtement sur un portfolio, encore moins avec autant
> de blabla, et encore moins en essayant de philosopher »

Sujet, verbe, complément. Un fait, un chiffre, un résultat, et on s'arrête.

- **Pas de tirets cadratins.** Jamais.
- **FR et EN sont deux écritures,** pas une traduction mot à mot.
- **Les accents sont obligatoires** dans tout texte affiché. Les commentaires
  de code peuvent s'en passer, l'interface non.
- Il note : « j'ai une passion pour les textes bien écrits ». Un texte
  approximatif sera vu.

**Et sur la façon de travailler avec lui :**

> « arrête de prendre mes mots de façon littéraire … tu ne comprendras jamais
> ce que je n'ai pas dit »

> « je m'attends souvent aussi à tes propositions … tu dois faire de vraies
> recherches sur les couleurs, les dégradés … toi tu dois les comparer, faire
> des tests »

> « avant de t'arrêter regarde bien toi-même, je ne veux plus avoir à te
> montrer des fautes de design de ce genre »

> « il faut bien hiérarchiser les choses et ne pas appliquer bêtement la même
> chose partout »

Autrement dit : **mesurer au lieu de supposer, proposer au lieu d'attendre,
et se relire avant de livrer.** Plusieurs allers-retours ont été perdus parce
que j'avais deviné une couleur au lieu de la mesurer.

---

## 5. Les règles de design, en bref

Le détail et les mesures sont dans `docs/15-regles-de-design.md`. L'essentiel :

1. **Une lumière monte la clarté.** Si elle la baisse, ce n'est pas une
   lumière, c'est une tache. Un halo lime sur un fond clair salit ; le même
   halo sur un fond noir éclaire.
2. **Plus la surface est grande, plus la lumière est diffuse.** Et un élément
   qui se répète ne porte qu'un liseré, jamais un halo.
3. **La couleur d'accent remplit des formes, elle n'écrit pas de mots.** Le
   lime sur du clair ne se lit pas.
4. **Un seul vert.** Douze pas d'une même échelle, teinte 76 en haut, 90 en
   bas. Deux familles de vert côte à côte vibrent et fatiguent l'œil.
5. **Jamais d'ombre sur du texte.**
6. **Les ombres restent sous les blocs blancs,** c'est ce qui les pose sur le
   fond, mais légères.
7. **Un bloc n'est pas un bouton.** Une encre de bouton devient un trou sur
   500 px de large.
8. **Le texte posé directement sur le fond est noir,** pas gris.
9. **Tout ce qui est cliquable doit se sentir.** Personne ne sera là pour le
   dire au visiteur.
10. **Tous les contrastes au niveau AA** (4,5:1 pour le texte, 3:1 pour les
    icônes et les indicateurs), vérifiés par calcul avant de livrer.

---

## 6. Où tout se trouve

[Référence à un emplacement local retirée de cette édition publique.]

### Le site

```
[Référence à un emplacement local retirée de cette édition publique.]
├── package.json              Next 16.2.10, React 19.2.4
├── next.config.ts            output:'export', trailingSlash, images non optimisées
├── AGENTS.md                 « ce n'est pas le Next.js que vous connaissez »
├── out\                      l'export statique, produit par `npm run build`
├── public\assets\            images, captures, logos, certificats, CV
└── src\
    ├── app\
    │   ├── globals.css       TOUT le système de design (variables + classes .ck-*)
    │   ├── layout.tsx
    │   ├── page.tsx          accueil : Hero, HomeServices, HomeMetiers, HomeFeatured
    │   ├── not-found.tsx     la 404, au-dessus de l'atmosphère
    │   ├── projets\ProjectsView.tsx   la page projets + les pop-up
    │   ├── a-propos\page.tsx
    │   └── contact\page.tsx
    ├── components\
    │   ├── Navbar.tsx        la barre, le cube, la fiche de profil
    │   ├── Hero.tsx          le premier écran
    │   ├── HomeServices.tsx  les trois métiers + leurs fenêtres
    │   ├── HomeMetiers.tsx   « Ce que je fais » : quatre pièces autour du titre
    │   ├── HomeFeatured.tsx  « Les projets », le carrousel un à la fois
    │   ├── Competences.tsx   « Savoir-faire & savoir-être », partagé
    │   ├── Footer.tsx        le pied de page et la signature pleine largeur
    │   ├── Providers.tsx     la langue, le thème, le dictionnaire FR/EN
    │   ├── ScrollToTop.tsx, ShareButton.tsx, CVModal.tsx, ReferenceModal.tsx
    │   └── chapters\         ChapterCard.tsx, ChapterModal.tsx, ChapterBlocks.tsx
    └── data\
        ├── projects.ts       tous les projets listés
        ├── chapters\         chapitre-01 à 06, index.ts, types.ts
        ├── references.ts     les fiches qui s'ouvrent depuis le texte
        ├── legacyLinks.ts    les anciennes adresses et leurs redirections
        └── toolLogo.ts + tool-*.json   les marques dessinées en une seule encre
```

Les fichiers `*.avant-refonte` sont les versions d'avant la refonte visuelle.
Ils servent de point de comparaison ; ils ne sont pas chargés par le site.

### Les documents

| Fichier | Contenu |
|---|---|
| `docs\00-paroles-de-calixte.md` | ses mots exacts. La source. |
| `docs\01-univers.md` | l'univers des nuages |
| `docs\02-architecture-projets.md` | pourquoi les projets portent ces noms |
| `docs\03-referentiel-infra.md` | adresses, VLAN, versions |
| `docs\04-urls-et-redirections.md` | les anciennes adresses |
| `docs\05-roadmap.md` | ce qui reste |
| `docs\06-complements.md` | notes diverses |
| `docs\07-captures-et-matiere.md` | les captures à produire |
| `docs\08-anatomie-dun-projet.md` | la structure d'un chapitre |
| `docs\09-chronologie-et-sources.md` | les dates |
| `docs\10-comment-on-lit-un-portfolio.md` | les trois publics |
| `docs\11-logos-a-telecharger.md` | les marques manquantes |
| `docs\12-comment-on-decrit-un-outil.md` | la règle outil / compétence |
| `docs\13-le-lab-docker-des-captures.md` | le labo des captures |
| `docs\14-outil-de-creation-de-vm.md` | l'automatisation des VM |
| `docs\15-regles-de-design.md` | **les règles visuelles et leurs mesures** |
| `docs\16-implementation-refonte.md` | ce qui a été fait, page par page |
| `docs\17-etude-couleur.md` | l'étude de couleur |
| `docs\chapitres\` | la matière des chapitres |

### Le reste de la racine

| Dossier | À quoi il sert |
|---|---|
| `croquis\` | les maquettes HTML validées avant le code |
| `maquette\`, `refs\` | les références visuelles |
| `a-mettre-en-ligne\` | le dossier préparé pour l'hébergement |
| `PLAN.md`, `README.md` | notes de haut niveau |

---

## 7. Comment travailler sur ce projet

### Compiler et vérifier

```
[Référence à un emplacement local retirée de cette édition publique.]
npx tsc --noEmit
npm run build
```

Puis servir l'export et vérifier **dessus** :

```
[Référence à un emplacement local retirée de cette édition publique.]
```

**Ne jamais vérifier sur le serveur de développement.** Sa connexion de
rechargement à chaud n'atteint pas le panneau d'aperçu : la page ne s'hydrate
pas, les carrousels ne répondent pas, les mesures JavaScript sont fausses. On
a perdu une session entière à chercher un bug qui n'existait pas.

Deux pièges Windows :

- le dossier `out` reste **verrouillé** si un terminal a son répertoire
  courant dedans, ou si un serveur le sert encore. Sortir du dossier et
  arrêter les `python -m http.server` avant de reconstruire ;
- la première compilation après un cache froid peut échouer sur les polices
  Google. **Relancer une fois** suffit.

### Modifier le code

Les remplacements se font par **script Python écrit dans le bac à sable**,
puis `python -I <script>`. Jamais de `sed` avec des antislashs, jamais de
heredoc bash contenant des accolades : cet environnement les casse.

**Un script de correction doit relire le fichier écrit et afficher le
résultat réel.** Une fois, un script a annoncé « appliqué » alors que le
remplacement n'avait rien trouvé. Depuis, chaque script se termine par une
vérification et sort en erreur si une ancre manque.

Les fichiers du projet sont en **CRLF**. Un script qui réécrit un fichier doit
le rendre en CRLF, sinon on obtient un fichier aux fins de ligne mélangées et
les ancres suivantes ne correspondent plus.

### Vérifier une couleur

Aucune couleur ne se décide à l'œil. On calcule le contraste
(WCAG, luminance relative) et on refuse en dessous de 4,5:1 pour le texte,
3:1 pour les icônes et les indicateurs. Pour comparer deux verts, on compare
leur **teinte** : deux teintes éloignées de plus de dix points ne vont pas
ensemble.

Pour mesurer une capture d'écran, un lecteur PNG en Python pur suffit
(`zlib` + `struct`) : il n'y a pas de Pillow sur cette machine.

---

## 8. L'univers, en une page

C'est sa vision, dans ses mots : un jeune ingénieur, « on peut également dire
un jeune prince », qui vit dans les nuages. Il y cherche des **opportunités**.
Il a sa **bibliothèque** (ses projets, son savoir) et sa **chambre** (la page
À propos, le lieu où on le connaît).

La statue de l'accueil, c'est lui : chemise blanche, cravate noire, veste en
cuir, posé sur un nuage, la main tendue vers un cube doré où est écrit
*opportunité*. La **404 est au sommet de l'atmosphère** : il n'y a plus rien
au-dessus. Les nuages traversent tout le site.

« j'ai envie que celui qui vient sur mon portfolio se sente bien dans les
nuages avec moi. »

---

## 9. Ce qui reste à faire

- **Le CV** : un seul désormais, celui d'administrateur systèmes et réseaux.
  Remplacer le PDF quand il le fournit, et retirer le second du sélecteur.
- **Les 22 captures d'écran** des chapitres 01, 02, 03, 04 et 06.
  `site\public\assets\captures\` n'existe pas encore, et le bouton qui y mène
  est commenté dans `ChapterModal.tsx` en attendant.
- **Deux projets de design** (Mimi Chips, Aura Financial) manquent dans le
  croquis `croquis\projets.html`.
- **Les chapitres 04 et 06** réutilisent `project_virtualix.png` : il leur
  faut leur propre image.
- **Rien n'est commité.** `site\` est un dépôt git avec deux commits du
  25 octobre 2026. Il a refusé le bouton de commit à chaque fois : ne pas
  commiter sans qu'il le demande.

---

## 10. Les erreurs déjà commises

Elles sont ici pour ne pas être refaites.

| L'erreur | Ce qu'il fallait faire |
|---|---|
| Affirmer qu'un greffon Vagrant coûtait 79 $, d'après un forum de 2020 | il est gratuit depuis juin 2021. Vérifier la date d'une source. |
| Proposer un titre « Trois chantiers » sans lire les cartes dessous | lire ce qu'on titre |
| Deviner que le fond était trop sombre | le mesurer : il était identique à celui de la référence |
| Mettre un halo lime sur un fond clair | un halo doit monter la clarté |
| Écrire en `--accent` sur du blanc : 1,84:1 | le lime ne s'écrit pas |
| Une règle `a:hover` globale qui repeignait les boutons | ne cibler que les liens sans classe |
| Un `padding: X 0 Y` sur une classe qui porte aussi `.lim` | le raccourci écrase les côtés. Deux fois le même piège. |
| Annoncer « appliqué » sans relire le fichier | toujours relire et afficher le résultat |

---

*Dernière mise à jour : 1er novembre 2026.*
