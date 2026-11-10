# 05. Navigation, mouvement et mobile

## La promesse du clic

Le visiteur doit anticiper ce qui arrive. « Voir le projet » peut ouvrir sa présentation. « À propos » change de page. Une image de projet simplement posée sur une carte n’annonce pas forcément une navigation. Calixte a demandé de réserver l’accès aux trois projets de l’accueil au bouton explicite et de laisser leur image sans action.

Ce choix n’interdit pas une galerie avec agrandissement : dans ce cas, annoncer la fonction de zoom. Le principe est la correspondance entre apparence, libellé et résultat, pas l’interdiction universelle des images interactives.

Les quatre domaines flottants peuvent ouvrir un aperçu court avec un bouton vers le projet. On préserve ainsi la découverte de l’accueil. Le contenu de cet aperçu doit apporter quelque chose, pas répéter seulement le titre de la carte.

## Navigation flottante

La barre centrale est une préférence forte pour le portfolio. Elle doit garder un espace autour du cube et des zones de clic suffisantes. Quand le cube paraissait trop grand sur mobile, la correction finale a consisté à rétablir sa taille et à répartir les icônes dans les espaces latéraux inutilisés. Réduire l’objet avait traité le symptôme sans corriger l’organisation.

La barre ne doit masquer ni le haut du titre ni une ancre ciblée. Vérifier sa position en haut de page, après défilement et lorsqu’une fenêtre est ouverte. Préserver un repère d’état actif.

Le globe de langue ouvre un choix Français / English sur mobile. Il ne doit pas changer de langue de manière imprévisible. Le CV propose un choix FR/EN avant téléchargement. Un document ne doit pas surprendre par son ouverture immédiate quand le bouton suggère d’abord une consultation.

## Le cube doit mériter son emplacement

Sa position centrale attire naturellement le clic. Répéter une photo et des liens sociaux déjà présents partout utilise mal cette attention. Une sélection courte de problèmes et de réalisations peut donner une raison d’explorer, sans prétendre que le cube contient tout le portfolio.

Un deuxième clic doit fermer ce qu’un premier clic a ouvert. Prévoir également un bouton de fermeture, Échap, le retour du focus et une interaction tactile. Si c’est une fenêtre modale, le focus reste dedans et l’arrière-plan ne doit pas être interactif. Voir le [modèle W3C des dialogues](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/).

## Mouvement : signature, pas obstacle

L’animation d’introduction du prénom a été envisagée puis explicitement retirée. Ne pas la remettre au nom d’une ancienne demande de mémorisation. L’animation du cube constitue une décision différente et reste voulue.

Le contenu doit être disponible sans attendre un spectacle. Les effets de survol ne portent pas une information indispensable. Une réduction des mouvements doit conserver la lecture et l’usage. La [recommandation W3C sur les animations d’interaction](https://www.w3.org/WAI/WCAG22/Understanding/animation-from-interactions.html) est de niveau AAA ; ne pas présenter toutes ses prescriptions comme du AA. Les animations automatiques demandent aussi une analyse de leur durée et de leurs moyens de contrôle.

Ne pas faire défiler horizontalement toute la page pour montrer une collection. Un carrousel local à commandes explicites peut être utile : le choix final vise une expérience courte, stable et prévisible, pas l’interdiction de tout changement de carte.

## Mobile : recomposer

La statue doit être centrée optiquement. Les quatre cartes peuvent se rapprocher du centre, varier légèrement de taille et d’angle, tout en laissant le texte lisible. Le bloc des années ne doit pas casser une date arbitrairement. Le nom doit rester visible, sans chercher à préserver une mise en page desktop à tout prix.

Pour les projets sélectionnés, l’objectif était de voir un projet et ses flèches dans un écran mobile courant. L’image peut dépasser légèrement de la carte blanche, comme une pièce épinglée, sans devenir cliquable. Réduire le texte de présentation est préférable à couper les boutons. Au zoom ou sur écran très court, permettre un défilement normal : l’objectif « un écran » ne justifie jamais un contenu inaccessible.

Les grands emails exigent une stratégie de retour à la ligne et une flèche qui ne comprime pas le texte. Les marges du footer doivent être comparées à celles du contenu principal. Une correction sur l’accueil doit conduire à inspecter les mêmes composants sur Contact, Projets et À propos.

Les cibles tactiles doivent être suffisamment espacées. WCAG 2.2 AA prévoit 24 × 24 pixels CSS ou certaines exceptions, notamment d’espacement ; une cible proche de 44 px est souvent un objectif de confort utile, pas le seuil AA universel. [Source W3C](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html).

## Longueur et détails

Garder un résumé visible et proposer les détails à la demande. Les chapitres regroupent les compétences, pas une page pour chaque outil. Une présentation en fenêtre depuis une carte peut coexister avec une URL directe partageable. Les anciennes notes interdisant toute page autonome ne doivent pas casser l’accès direct déjà utilisé.

Ne pas multiplier les fenêtres imbriquées. Ne pas masquer une donnée essentielle derrière trois clics. Les missions du footer gagnent une définition courte dépliable ; la page Contact peut les expliquer davantage.

## États à concevoir

Prévoir chargement, erreur, vide et réussite quand ils ont un sens. Un catalogue local de dix-neuf projets n’exige pas automatiquement une pagination serveur. Une recherche sans résultat demande un message utile et un moyen de réinitialiser les filtres.

Le formulaire doit préserver le message en cas d’échec et proposer une alternative clairement lisible. Exemple : « Le message n’a pas été envoyé. Vous pouvez réessayer ou m’écrire à… ». Ne pas annoncer une réception avant confirmation du serveur. Dans le mail reçu par Calixte, conserver les intitulés des champs, y compris Objet vide, puisqu’il veut voir ce que le visiteur a renseigné.

La 404 stylée doit être servie pour une URL inconnue, avec un vrai statut 404 et des liens utiles. Le fonctionnement local n’est pas une preuve de configuration correcte sur l’hébergement. Les erreurs, le téléchargement des CV et l’envoi du formulaire font partie de l’expérience finale, pas d’une finition secondaire.
