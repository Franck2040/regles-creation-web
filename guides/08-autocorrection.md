# 08. Une méthode d’autocorrection avant validation

## 1. Établir un diagnostic court

Écrire cinq lignes : visiteur principal, besoin, impression recherchée, action principale, contraintes. Puis relever les éléments déjà validés et les modifications demandées. Cela évite de remplacer un design accepté au prétexte de l’améliorer.

Exemple pour une modification de signature : « Garder le thème clair, la navigation et les projets. Recomposer uniquement le titre et le nom. Le nom doit appartenir au groupe sans concurrencer les domaines. Les boutons doivent rester libres. Tester le nom complet et une signature prénom dans une réserve dédiée. »

## 2. Examiner les références à deux échelles

À l’échelle de la page : rythme, masses, alternance de densité, place des actions. À l’échelle du détail : tailles relatives, bords, transparence, interlignage, alignements et états interactifs.

Décrire une relation transférable plutôt qu’un objet à copier. « Une annotation secondaire s’ancre au bord du titre » aide davantage que « mettre une étoile comme Relab ». La référence sert à comprendre une logique ; elle ne prouve pas que chaque détail convient au nouveau sujet.

## 3. Construire une maquette accessible

Utiliser de vrais textes de longueur réaliste et les vrais visuels disponibles. Un faux titre de trois mots ne permet pas de valider un vrai titre de neuf mots. Le prototype HTML doit ouvrir dans le navigateur annoncé, avec ses polices et images. Un screenshot peut documenter le résultat, mais ne remplace pas la maquette demandée.

S’il faut comparer, proposer deux ou trois directions réellement distinctes, pas trois couleurs sur le même modèle. Nommer ce qui varie : structure, relation image/texte, rythme, degré de décor. Recommander une option avec une raison liée au visiteur.

## 4. Corriger avant de montrer

Faire une première passe de composition sans chercher une note numérique globale. Une seule collision importante peut ruiner un écran qui serait « bon à 90 % ». Corriger par priorité : contenu inaccessible, promesse fausse, action ambiguë, hiérarchie confuse, incohérence de style, puis finition.

| Observation | Question de diagnostic | Action possible |
|---|---|---|
| Tout attire l’œil | Où est le premier point de lecture ? | Réduire les accents secondaires et garder une dominante |
| Le nom paraît ajouté après coup | Partage-t-il un axe ou une zone avec le titre ? | Recomposer son emplacement et son échelle |
| Le fond paraît sale | Les textures traversent-elles le texte ? | Localiser, atténuer ou retirer la texture |
| L’effet verre ressemble à du métal | Le fond reste-t-il perceptible ? | Réduire l’opacité et revoir les reflets |
| Une carte semble hors famille | Cadre, rayon, lumière et couleur diffèrent-ils sans raison ? | Harmoniser les rôles, pas forcément toutes les dimensions |
| L’écran est trop long | Quelles informations servent le premier regard ? | Résumer et déplier les détails ; ne pas miniaturiser le texte |
| Le bouton existe mais n’est pas visible | Est-il hors écran, couvert ou trop peu contrasté ? | Corriger la disposition avant de changer sa couleur |
| Le texte semble pompeux | Quelle réalisation vérifiable décrit-il ? | Revenir au besoin et à l’action |

## 5. Vérifier une matrice réelle

Choisir des largeurs représentatives, par exemple 360, 390, 768, 1280 et 1440 pixels, avec au moins une hauteur courte. Ce sont des points de contrôle proposés, pas des certifications de compatibilité. Ajouter les dimensions du problème rapporté par l’utilisateur.

Pour chaque taille : ouverture de page, navigation, titre, cartes, fenêtres, footer, formulaire et 404. Vérifier français et anglais, zoom à 200 %, clavier, mouvement réduit et absence de survol. Un test automatisé d’absence de débordement ne détecte pas une statue visuellement décentrée ; il faut regarder.

Dans le navigateur, confirmer que la taille demandée est effectivement appliquée. Une tentative d’émulation qui laisse `innerWidth` à 1280 ne compte pas comme test mobile. Les captures mobiles historiques renseignent les problèmes passés, mais ne valident pas la version actuelle.

## 6. Contrôler le sens des interactions

- Chaque bouton porte une action compréhensible et l’exécute.
- Les images sans action ne prennent pas un curseur ou un effet qui promet un clic.
- Une fenêtre se ferme au bouton, au clavier et selon le comportement annoncé du déclencheur.
- Le focus reste visible et revient à une place logique après fermeture.
- Les liens externes, téléchargements et changements de page ne surprennent pas.
- Les champs invalides expliquent quoi corriger ; une erreur d’envoi ne prétend pas que le message est arrivé.

## 7. Faire une passe éditoriale indépendante

Lire les cartes seules, puis les paragraphes seuls, puis l’enchaînement complet. Chercher les pronoms sans antécédent, les promesses absolues, les répétitions et les raccourcis techniques. Vérifier que la version anglaise raconte le même fait avec le même niveau de certitude.

Ne pas compter seulement les mots. Un paragraphe de quatre phrases précises peut être plus facile à lire qu’une phrase de cinquante mots compressant trois projets. Ne pas introduire une faute pour raccourcir un titre.

## 8. Présenter une version contrôlée

Dire ce qui change, pourquoi et où le voir. Mentionner les contrôles réalisés et les limites. Éviter « tout est parfait », « responsive sur tous les appareils » ou « sécurisé à 100 % ». Ne pas raconter chaque commande exécutée.

Exemple de compte rendu : « La signature possède maintenant sa propre ligne sous les domaines. Les deux boutons restent visibles à 1280 × 720 et à 390 × 844, en français et en anglais. J’ai conservé le cube et la palette. Le test de réception du formulaire sur LWS reste à faire. » Cette phrase ne doit être utilisée que si ces contrôles ont réellement eu lieu.

## 9. Apprendre de la correction

Après retour de Calixte, noter l’intention comprise et la portée. Si « baisse un peu » corrige une collision avec la navigation, enregistrer la collision et sa cause, pas seulement « marge +12 ». La prochaine page n’aura pas forcément les mêmes hauteurs.

Éviter l’accumulation de correctifs contradictoires. Supprimer ou consolider une ancienne règle remplacée lorsque le code est concerné, puis revoir les pages qui l’utilisent. Conserver le raisonnement dans le journal pour ne pas réintroduire la mauvaise piste six jours plus tard.

## Critères de livraison

Un élément ne passe pas la validation s’il est coupé, masque une action, invente un fait, introduit une navigation inattendue ou reste impossible à consulter. Les détails de goût peuvent être discutés ; ces défauts visibles doivent être corrigés avant la présentation.

La validation esthétique vient ensuite : cohérence des masses, valeurs, matières, rythmes et microdétails. On peut expliquer cette cohérence, mais on doit surtout la voir dans le rendu.
