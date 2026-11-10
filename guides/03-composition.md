# 03. Typographie, composition et espace

## Commencer par les masses

Avant les reflets et les bordures, placer le titre, le visuel principal, le texte d’accompagnement et les actions. Regarder la page en petit : doit-on voir quatre objets également insistants, ou une hiérarchie ? Dans le portfolio, le titre porte les domaines, la signature identifie, la statue incarne l’univers et les boutons proposent la suite. Si la signature masque un bouton, la relation est incorrecte même si chaque élément est beau.

L’espace vide sert à séparer, regrouper ou laisser respirer. Un vide n’est pas automatiquement un défaut. Il devient problématique lorsqu’il casse une relation, laisse un groupe trop isolé ou donne l’impression que la page attend du contenu. Une trame peut enrichir une surface, mais ne répare pas une mauvaise position du titre.

## Composition du titre : enseignements de la signature

La séquence réelle a exploré un nom complet calligraphié, un K dominant, une disposition inspirée d’un cœur, une annotation latérale, puis « Calixte » sous le titre. Les essais n’ont pas tous été validés. La dernière direction retient une structure simple et une signature distincte sous les domaines.

| Défaut observé | Cause possible | Correction pertinente |
|---|---|---|
| Nom qui semble étranger | Finesse excessive face au gros sans-serif, position sans ancrage | Ajuster l’échelle et la place ; réserver une zone plutôt que forcer une fusion |
| K allongé et maigre | Transformation non uniforme | Choisir une forme adaptée ou une autre composition ; ne pas étirer le dessin |
| Lettres collées au K | Grande initiale sans réserve latérale | Recomposer le groupe entier et observer les contreformes |
| Y coupé | Hauteur de ligne ou masque trop serré | Donner de la place à la descendante sans éloigner inutilement les lignes |
| Calixte coupé | Débordement calligraphique hors boîte ou masque | Ajouter de l’espace réel autour du glyphe ; vérifier les boucles complètes |
| Boutons masqués | Position absolue sans place dans le flux | Réserver la hauteur de la signature avant le paragraphe et les actions |
| Ensemble sous la navbar | Espacement supérieur calculé indépendamment de la barre | Régler les deux blocs ensemble sur écran court et large |

Le bon réglage ne consiste pas à augmenter partout la hauteur de ligne. Il faut préserver la proximité voulue entre « Systèmes » et « réseaux » tout en laissant le y exister. Une réserve interne pour les glyphes peut résoudre la découpe sans éloigner les lignes visuellement.

## Typographie observée, pas déduite des noms de variables

Dans le code consulté, la variable nommée `--font-space-grotesk` charge Plus Jakarta Sans, et `--font-manrope` charge Inter. La calligraphie est Great Vibes. Un futur assistant doit vérifier les polices réellement chargées, pas seulement les noms historiques des variables.

Les valeurs de cette version sont des repères, non une recette : titre principal fluide jusqu’à environ 94 px, graisse 600, interligne proche de 1,02 ; paragraphe limité à environ 52 caractères de largeur ; dégradé des titres allant de l’encre au gris. Le rendu réel dépend de la police, du texte, de la largeur et des styles spécifiques au composant.

Pour un autre projet, repartir du contenu. Un mot long en anglais peut imposer une autre coupure. Ne pas réduire tout le titre à une taille insignifiante pour maintenir à tout prix deux lignes.

## Alignement géométrique et alignement optique

Une image transparente peut être centrée dans sa boîte tout en paraissant décalée : son sujet occupe une portion asymétrique. La statue doit être jugée sur sa masse visible, son nuage et son cube, pas seulement sur la largeur du fichier. Le texte ne doit toucher ni son visage ni le nuage par accident.

Même logique dans le footer : le long email, la flèche ronde et le bloc d’alternance doivent partager une largeur et des marges cohérentes. Un bouton mathématiquement centré peut sembler décalé si la flèche monopolise un côté. Vérifier le groupe et l’alignement des contenus voisins.

## Détails qui donnent vie

Les cadres blancs, les inclinaisons discrètes, les cercles fléchés et la variation d’échelle des images participent à l’identité. Leur fonction doit rester identifiable : séparer une image claire, suggérer une carte posée, désigner une action, instaurer un rythme.

Éviter de tout incliner. Une composition a besoin de repères stables pour que quelques écarts aient du sens. Si toutes les cartes flottent, tournent, brillent et changent de taille, aucune ne constitue plus une surprise.

## Premier écran et écrans courts

Le titre, la signature, le paragraphe et les actions forment un groupe. Le déplacer implique de vérifier tout le groupe. Les captures annotées en vert par Calixte signalaient une sélection de contenu, pas une demande de surlignage fluorescent permanent.

Sur un ordinateur peu haut, réduire d’abord les espaces excessifs avant de comprimer les lettres. Sur mobile, accepter que tout l’univers n’entre pas dans le premier écran. Les actions essentielles ne doivent pas être coupées par un conteneur à hauteur fixe.

## Test pratique

Observer successivement : silhouette globale, ordre de lecture, distances entre groupes, espace intérieur des lettres, bords des images, alignement des actions. Masquer mentalement les effets : si l’ensemble ne tient plus, il faut encore travailler sa composition.
