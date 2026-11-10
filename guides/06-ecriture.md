# 06. Écrire avec précision, dignité et intérêt

## Ce que le lecteur doit comprendre

Il doit distinguer le problème, le contexte et le travail réalisé sans avoir besoin de lire tout le site. Un recruteur peut entrer directement dans un chapitre, ouvrir une carte puis repartir. Chaque section doit donc fournir assez de contexte local, tout en évitant de répéter une introduction entière.

Calixte veut présenter ses travaux avec honneur et simplicité. Ne pas inventer une expérience d’entreprise. Ne pas remplacer cette invention par une posture d’excuse : « petit étudiant », « seulement un labo », « je ne suis pas expert mais… ». Le contexte laboratoire est une information factuelle, pas une faiblesse à justifier.

## Une méthode en cinq questions

Pour chaque paragraphe : qui agit ? Sur quoi ? Dans quel contexte ? Que fait-il exactement ? Que sait-on du résultat ? Toutes les réponses n’ont pas à être écrites dans chaque phrase, mais l’assistant doit les connaître pour ne pas fabriquer du sens.

Ensuite demander : qu’apprend le visiteur ici qu’il ne savait pas dans le paragraphe précédent ? Si la réponse est « que Calixte est motivé et polyvalent », chercher un fait ou supprimer la phrase.

Enfin lire le paragraphe hors de son emplacement. « Cela améliore la sécurité » est incompréhensible seul et souvent trop vague. « Les règles du pare-feu limitent les échanges entre les réseaux du laboratoire » situe l’objet et l’action, si c’est bien ce qui a été configuré.

## Trois niveaux de lecture

**Carte :** un titre, une idée précise et une action. Ne pas résumer tout le chapitre en six lignes denses. Exemple proposé, à confirmer avec les travaux : « Créer les comptes à partir d’un fichier, sans les saisir un par un. »

**Ouverture de chapitre :** le contexte, l’objectif et le périmètre. Exemple : « Dans ce laboratoire Windows, j’ai automatisé la création des comptes utilisateurs à partir d’un fichier CSV. »

**Détail technique :** méthode, configuration, vérification et limites. Adresses, VLAN, ports et versions ont leur place ici lorsqu’ils sont réels. Un détail technique utile ne devient pas du bavardage simplement parce qu’il demande plus de trois lignes.

## Les phrases intéressantes ne sont pas forcément des slogans

Une question fonctionne quand elle nomme une difficulté reconnue : « Comment éviter de trier deux fois la même offre ? » La réponse décrit immédiatement le workflow. Une question vide comme « Et si on allait plus loin ? » n’oriente pas le lecteur.

« D’un domaine à l’autre » a été explicitement choisi pour la section des domaines. Le double sens peut enrichir la lecture, mais ne suffit pas seul : les images et exemples donnent le contenu concret. Ne pas construire tous les titres sur des jeux de mots.

Des labels ordinaires comme « Contact », « Projets » ou « Télécharger » restent utiles. L’interdiction des phrases génériques vise les promesses interchangeables, pas les conventions qui facilitent la navigation.

## Exemples de réécriture raisonnée

Les variantes ci-dessous sont des modèles éditoriaux, pas l’affirmation que toutes les actions ont été vérifiées dans les dépôts techniques.

| Formulation à examiner | Pourquoi | Variante ou décision |
|---|---|---|
| « Je construis des solutions innovantes et performantes » | Aucun problème ni fait identifiable | Nommer l’action : « Mon workflow classe les offres reçues par mail et retire les doublons. » |
| « Monter un serveur est une solution » | L’action ne donne pas le besoin | « Déployer un serveur de fichiers pour partager les documents du laboratoire. » si c’est l’usage réel |
| « Superviser des services » | Compétence, pas encore réalisation | « Déployer Zabbix pour suivre l’état des machines et recevoir des alertes. » si configuré |
| « Sept contrôles à chaque modification du code » | Déclenchement potentiellement faux | Si vérifié : « Le pipeline lance sept contrôles de sécurité à chaque push. » Sinon décrire les contrôles effectivement intégrés sans chiffre inventé |
| « Une boutique complète » | Périmètre flou et absolu | « Une boutique en ligne avec catalogue, comptes clients et panier. » uniquement pour les fonctions présentes |
| « Conception logicielle stricte » | Adjectif sans contenu | « Application de suivi de santé en Java et Spring Boot. » puis décrire une fonction réelle |
| « Plateforme innovante » | Jugement non démontré | « Projet collectif de plateforme d’apprentissage. » puis préciser sa contribution |
| « Ne jamais perdre les données » | Garantie impossible à soutenir | « Sauvegarder les données et tester leur restauration. » uniquement si les tests ont eu lieu |
| « Passerelle qui survit à une panne » | Image possible mais ambiguë | « Tester le basculement entre deux pare-feu en laboratoire. » si réalisé |
| « Expert bureautique » | Statut non nécessaire | Nommer les supports réalisés et réserver PowerPoint aux présentations |
| « Ce que je peux apporter » | Introduit un plaidoyer plutôt qu’un fait | Montrer les réalisations ou nommer directement les missions recherchées |
| « Quatre réalisations » autour des domaines | Peut faire croire que le catalogue est limité à quatre | Employer le titre validé « D’un domaine à l’autre » et montrer les exemples |
| « Projets choisis » | Dit que l’auteur a choisi, pas pourquoi regarder | « Ce que j’ai construit » pour les réalisations ; adapter au rôle réel de la section |
| « Disponible novembre 2026 » | Peut signifier un seul mois | « Disponible dès octobre 2026 » selon la dernière décision, à réactualiser avant publication future |
| « Coordination multisite, mission sans droits… » dans une longue phrase | Plusieurs réalisations et contraintes confondues | Séparer coordination, difficulté et documentation en phrases situées, sans les attribuer au même projet sans preuve |
| « J’ai tout développé seul » | Peut effacer équipe et assistance | Décrire la contribution réelle ; situer l’aide d’outils IA lorsque pertinent sans en faire une excuse répétée |

Une phrase technique précise ne doit pas être rendue vague par prudence excessive. Si les sept contrôles sont prouvés, le chiffre est utile. Le problème est l’exactitude de la condition et du périmètre, pas la précision elle-même.

## Exemple développé : une carte puis son ouverture

Version faible : « Automatisation innovante et optimisation du processus de veille grâce à une solution complète. »

Carte proposée : « Comment éviter de trier deux fois la même offre ? » Puis : « Mon workflow classe les offres reçues par mail et écarte les doublons avant leur ajout dans Notion. »

Ouverture proposée : « J’ai construit ce workflow pour ma recherche d’emploi. Il récupère les offres reçues dans Gmail, extrait leurs informations et les range dans Notion. »

Suite : expliquer l’identification des doublons, les champs réellement extraits et la gestion des erreurs. Ne pas inventer un gain de trois heures par jour. Si aucun temps n’a été mesuré, parler de suppression d’une saisie répétitive plutôt que de productivité chiffrée.

## Français et anglais : conserver l’intention

L’anglais doit être une rédaction naturelle, pas une substitution de mots. Préserver le sens, le niveau de certitude, le contexte et l’action. Vérifier ensuite la longueur dans la carte réelle.

| Intention française | Anglais proposé | Point de vigilance |
|---|---|---|
| Comment éviter de trier deux fois la même offre ? | Keeping duplicate job listings out of my search | Un titre idiomatique peut devenir affirmatif ; le sujet reste la déduplication |
| Mon workflow classe les offres reçues par mail… | My workflow organises job listings from incoming emails and removes duplicates before saving them to Notion. | Ne pas traduire « offre » comme proposition commerciale |
| D’un domaine à l’autre | Across my work | Le double sens français ne survit pas forcément ; les cartes précisent les domaines |
| Ce que j’ai construit | What I’ve built | Formule déjà naturelle, inutile de la changer pour le plaisir |
| Voir le projet | View project | L’action doit mener au projet, pas seulement à une image |
| Disponible dès octobre 2026 | Available from October 2026 | « From » exprime un début, pas un mois isolé |
| Rythme d’alternance | Work-study schedule | Expliquer ensuite three weeks with the employer, one week at school |
| Travaux en laboratoire | Lab projects | Ne pas convertir en professional deployments |
| Développement d’applications web et mobiles | Web and mobile application development | Éviter development seul si le contexte ne le précise pas |
| Le message n’a pas été envoyé | Your message couldn’t be sent | Ajouter une action concrète et conserver le contenu du formulaire |

« Have I already seen this vacancy? » est grammatical, mais déplace le problème vers la mémoire de l’auteur alors que le français parle du tri répétitif. Le défaut est surtout l’intention, pas le seul mot vacancy.

Ne pas réécrire toute la page anglaise quand l’utilisateur en valide déjà presque tout. Corriger les endroits identifiés et contrôler la cohérence des termes partagés.

## Profil : séparer compétence, intérêt et objectif

Calixte a une scolarité primaire et secondaire en anglais et décrit son niveau comme courant. Ne pas le réduire à « notions » ni inventer une certification linguistique. Les certifications projetées restent dans une feuille de route ; seules les attestations obtenues vont dans les acquis.

Canva, Photoshop, Affinity et PowerPoint appartiennent à ses outils, avec PowerPoint pour les présentations. Le graphisme n’a pas à être justifié artificiellement comme une technique réseau. Les missions de développement peuvent être mentionnées comme un intérêt réel, avec le lien à la formation et la validation pédagogique lorsque cette question est pertinente. Ne pas affirmer que toute mission sera acceptée par l’école.

## Titres et ponctuation

Pas de tiret cadratin dans les nouveaux textes publics. Utiliser une phrase, une virgule, un deux-points ou des parenthèses selon le sens. Éviter les majuscules prolongées pour des phrases entières. Elles peuvent convenir à un petit repère, mais pas automatiquement à un titre narratif comme celui de la 404.

La formulation finale demandée pour l’introduction doit être conservée tant qu’aucune révision n’est autorisée : « Je m’intéresse autant au fonctionnement des infrastructures informatiques qu’aux applications qui les accompagnent. À travers mes projets, j’explore leur installation, leur configuration, leur développement et leur sécurisation. »

Ne pas corriger une formulation validée uniquement pour montrer une intervention. Toute révision doit résoudre un problème précis de sens, de rythme ou de lecture.
