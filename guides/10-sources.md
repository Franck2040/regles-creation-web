# 10. Sources, traçabilité et limites

## Corpus utilisé

Cette méthode s’appuie sur les messages fournis dans la conversation de reprise, les notes locales du dossier Portfolio/docs, les croquis disponibles, le code actuel de chatgpt/site et l’observation du site publié le 9 novembre 2026. Les messages comprennent des demandes directes de Calixte et des audits d’autres assistants qu’il a cités. Ces audits ne sont pas assimilés automatiquement à ses propres décisions.

Ce dépôt n’est pas un export exhaustif octet par octet de toutes les conversations historiques. Il conserve une synthèse détaillée de leurs corrections accessibles, un registre de décisions et des archives pertinentes. Les dates exactes de chaque aller-retour ne sont pas toutes connues. Aucun historique absent n’a été inventé.

## Quatre statuts de connaissance

1. **Demande explicite :** Calixte demande un comportement ou valide une direction. Exemple : supprimer l’animation d’introduction.
2. **Observation :** élément vu dans une capture ou dans le rendu actuel. Exemple : signature sous le titre.
3. **Interprétation :** raison probable reliant plusieurs remarques. Exemple : recherche d’une qualité perceptible avant d’être expliquée.
4. **Recommandation :** méthode proposée pour obtenir ce résultat. Exemple : matrice de contrôle avec plusieurs largeurs.

Un assistant ne doit pas présenter le quatrième statut comme une parole de Calixte. Une archive rédigée par un assistant ne devient pas une source technique fiable simplement parce qu’elle figure dans docs.

## Références visuelles

- [Relab](https://relab-html.vercel.app/) : hero, annotations, couleurs, hiérarchie, chevauchements.
- [Minux Work](https://minux-html.netlify.app/work) : contraste sans-serif/calligraphie, surfaces et appel à projet.
- [Portfolio publié](https://kenmeugnecalixte.com/) et pages [Projets](https://kenmeugnecalixte.com/projets/), [À propos](https://kenmeugnecalixte.com/a-propos/), [Contact](https://kenmeugnecalixte.com/contact/).
- Croquis local `croquis/hauteurs-1440,960.png`, conservé comme prototype historique.

Les captures de templates sont des références d’étude attribuées. Leurs sources, images et composants ne sont pas redistribués comme un kit à réutiliser. Ce dépôt ne confère aucun droit sur les créations des auteurs des templates.

## Références de vérification

- [W3C : contraste du texte](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html).
- [W3C : taille minimale des cibles](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html).
- [W3C : animations déclenchées par interaction](https://www.w3.org/WAI/WCAG22/Understanding/animation-from-interactions.html).
- [W3C : dialogue modal](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/).

Les guides paraphrasent les points utiles et ne constituent pas un audit de conformité. Vérifier la documentation actuelle lors d’une implémentation future.

## Points volontairement non certifiés

Les captures de cette étude sont desktop. Une tentative de changement de viewport n’a pas effectivement produit une largeur mobile ; elle n’est pas comptée comme test mobile. Les problèmes mobiles décrits proviennent des retours et captures historiques de Calixte.

Les projets techniques n’ont pas tous été réexécutés pour ce guide. Les exemples de rédaction qui supposent un résultat sont marqués comme conditionnels. Ni le nombre de contrôles de sécurité, ni une restauration, ni un basculement ne doivent être affirmés sans preuve du projet concerné.

Le code consulté permet d’identifier des styles et des polices, mais seul le rendu permet de juger leur résultat. La version en ligne peut évoluer après la date des captures. Consulter la preuve datée plutôt que supposer qu’une URL reste identique.

## Informations datées à maintenir à part

Disponibilité, formation, rythme, certifications et catalogue sont des données du profil. Elles ne sont pas des règles esthétiques. La disponibilité dès octobre 2026 est le dernier choix explicite connu, pas une phrase à réutiliser indéfiniment.

## Confidentialité et conservation

Cette édition publique a été préparée à la demande de Calixte le 10 novembre 2026, sous le nom regles-creation-web. Elle est publiée séparément du dépôt privé afin de ne pas exposer son ancien historique. Les adresses e-mail et les chemins locaux ont été retirés des archives publiques. Le dépôt ne contient pas les secrets de déploiement, mots de passe, sessions de navigation ou CV complets. Les captures des références sont conservées comme illustrations de l’analyse, avec attribution des sites sources. Elles ne constituent pas des ressources graphiques libres à réutiliser.
