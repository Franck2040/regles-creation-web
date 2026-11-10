# 04. Couleur, lumière, matière et icônes

## Une palette distribue des rôles

La palette finale du portfolio associe un fond chaud clair, du blanc, de l’encre, plusieurs valeurs de vert et quelques accents chauds liés aux visuels. Le problème dénoncé n’était pas simplement « trop de noir », mais une succession de blocs tous aussi sombres qui écrasait l’identité claire.

Repères relevés dans le code consulté :

| Rôle | Valeur indicative | Usage |
|---|---|---|
| Fond | `#F4F3F0` | Surface générale chaleureuse |
| Carte | `#FFFFFF` | Détachement et lisibilité |
| Texte | `#1A2018` | Lecture principale |
| Texte secondaire | `#474C42` | Informations d’accompagnement |
| Accent lime | `#C6F641` | Sélection, détails d’action, lumière |
| Accent intermédiaire | `#7EAF1D` | Transition et profondeur |
| Feuille sombre | `#2D4610` | Signature et accents calmes |
| Forêt | `#16240A` à `#243A0D` | Actions fortes et surfaces ponctuelles |

Ces valeurs décrivent cette version. Elles ne constituent pas une preuve que chaque combinaison respecte le contraste. Mesurer la paire réelle avec son opacité et son arrière-plan, notamment pour le petit texte.

## Les verts doivent appartenir au même monde

Le cube demandé était transparent et lumineux. Un vert néon d’une autre famille pouvait rompre la relation avec les boutons et la signature. La correction utile consiste à garder la famille de couleur, puis à varier valeur, saturation et transparence pour différencier les faces.

Un dégradé ne doit pas être ajouté partout parce qu’un premier dégradé a été apprécié. Il peut donner du relief à un titre, un bouton ou un fond localisé. Les zones de lecture doivent rester calmes. Le dégradé noir-gris des titres a été préféré au vert afin d’accorder le texte et l’identité sans multiplier les accents.

## Verre et métal ne racontent pas la même matière

Le verre laisse percevoir ce qui est derrière. Il peut comporter une teinte, des bords éclairés, une réfraction suggérée et des faces légèrement différentes. Une surface opaque verte, fortement contrastée et réfléchissante peut évoquer le métal même si le composant s’appelle « glass ».

Pour vérifier : voit-on encore le fond ? Les faces laissent-elles de l’air ? Les arêtes décrivent-elles un volume ? L’ombre ancre-t-elle l’objet sans le rendre lourd ? Le halo est-il localisé ? Si la transparence ne se lit pas, augmenter le flou n’est pas nécessairement la solution.

Le cube peut garder son mouvement et changer de matière. La dernière demande validait sa forme vitrée et ses animations tout en rétablissant le vert du thème. L’ouverture et la fermeture doivent rester fonctionnelles ; l’objet n’est pas seulement une image.

## Une lumière se juge sur son fond

Le blanc pur se remarquait peu sur une barre blanche. Le vert trop sombre ressemblait à une ombre. Les essais ont conduit à une lumière légèrement chaude, entre jaune pâle et blanc, autour d’un cube vert. Cette séquence montre que le nom de la couleur ne suffit pas : intensité, diffusion, rayon et contraste avec la surface déterminent la perception.

Éviter un halo énorme et uniforme. Il brouille les icônes voisines et donne une tache plutôt qu’une source lumineuse. Observer le cube fermé, ouvert, au survol et sur mobile, où le survol peut ne pas exister.

## Fonds : présence légère et lisibilité

Les nuages réalistes étaient souhaités à des endroits précis, avec une interaction de dissipation. Les brouillards répartis en arrière-plan et les résidus près des barres de navigation ont été rejetés. Le cube a remplacé une piste de nuage animé dont la qualité n’atteignait pas l’attente. Cela ne prouve pas que tous les nuages sont mauvais ; cela établit qu’une matière approximative ne doit pas être livrée comme une réussite.

Les triangles ont ensuite été remplacés par des formes plus douces, puis une grille carrée légère. Dans le code observé, la trame repose sur des lignes fines espacées d’environ 32 px avec un masque progressif. Son rôle est d’habiter une surface, pas de concurrencer les mots. Sur les autres pages et près du footer, une variation cohérente suffit ; la répétition exacte de chaque effet n’est pas indispensable.

## Icônes et marques

Dans une liste dense de compétences, les logos multicolores créaient trop de sollicitations. Un traitement monochrome et des tailles optiques proches ont amélioré l’ensemble. Une marque déjà lisible comme un mot ne doit pas être suivie du même nom une deuxième fois.

Ne pas confondre catalogue partagé et dessin identique : les marques Simple Icons ont des proportions différentes. Une marque large comme VMware ne doit pas être forcée dans un carré de 18 px. Les glyphes de navigation doivent appartenir à une famille cohérente ; les logos peuvent garder leur identité lorsqu’ils sont utiles pour reconnaître un outil.

Pas de téléchargement manuel répétitif si une source locale organisée et un processus reproductible suffisent. Ne pas masquer une image opaque en supposant qu’elle est transparente : on risque un bloc plein.

## Pas de fausse science des couleurs

Les archives contiennent des affirmations trop absolues sur l’écart angulaire entre teintes, la fatigue oculaire et les proportions de lime. Elles ne sont pas retenues. Il n’existe pas ici de seuil démontré disant que deux verts distants de dix degrés ne peuvent cohabiter. L’inconfort exprimé est un signal à prendre au sérieux ; la cause doit être examinée dans la composition réelle.

Le contraste accessible est vérifiable. L’harmonie demande aussi du jugement. Pour le texte courant, WCAG donne généralement un minimum de 4,5:1, et 3:1 pour le grand texte selon sa définition, avec des exceptions précises. Lire la [référence W3C](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html). Ce seuil ne garantit pas à lui seul un beau design.
