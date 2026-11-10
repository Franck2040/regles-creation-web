# 12 — Comment on décrit un outil

> Règle née le 29 octobre, de cette remarque :
>
> « lorsque on veut présenter une alternative, la base serait d'abord de présenter l'outil avec les termes qu'il faut, puis dire ce pourquoi l'outil est souvent utilisé et en quoi ça peut être utile. De par la description de ce que l'outil fait et de comment il s'utilise, le lecteur saura à quoi ça sert. »

## Trois paragraphes, toujours dans cet ordre

### 1. Ce que c'est

Avant toute opinion. **Ça commence par le type de service** : un ITSM, une CMDB, un UEM,
un NMS, un SIEM, un EDR, un XDR, un NDR, un IAM, un IGA. Le lecteur range l'outil dans
une famille avant d'en lire la description, et il peut survoler le sigle pour savoir ce
qu'elle recouvre et qui d'autre en fait, en Europe d'abord.

Puis quatre choses, dans la même phrase ou presque :

- **qui l'édite** et sous quelle licence (libre, payant, loué au mois) ;
- **sous quelle forme il arrive** : un logiciel qu'on installe sur un serveur, un service qu'on loue, une distribution, un rôle d'un système déjà présent ;
- **ce qu'il fait concrètement**, en termes de métier, pas en adjectifs ;
- **comment on s'en sert** : qu'est-ce qu'on installe, qu'est-ce qu'on écrit, qu'est-ce que ça produit.

Un lecteur qui n'a jamais entendu le nom doit pouvoir expliquer l'outil à quelqu'un d'autre après ce paragraphe.

### 2. Pourquoi on le choisit

Le cas où cet outil est le bon. Pas ses qualités en général : la situation précise dans laquelle quelqu'un le prend plutôt qu'un autre.

Pour l'outil que j'ai utilisé, c'est « pourquoi je l'ai choisi », et la raison doit se rattacher à quelque chose de raconté dans le chapitre.

### 3. Sa limite

**Seulement pour l'outil que j'ai utilisé.** On ne reproche rien à une alternative : elle est là parce qu'elle a sa place, pas pour être battue.

## Ce qui est interdit

**Une phrase qui défend un choix au lieu de décrire.** Les trois paragraphes disent ce qu'un
outil est, dans quel cas on le prend, et où il s'arrête. Ils ne plaident pas. Dès qu'une
phrase commence par « c'est une méthode », « ce qu'on obtient en échange » ou « ce n'est
pas X, c'est Y », elle est à couper. Voir la règle en tête de
[docs/10](10-comment-on-lit-un-portfolio.md).

**Une phrase qui ne tiendrait pas si on remplaçait le nom de l'outil par un autre.** Test à faire sur chaque phrase : si « le même travail décrit dans un fichier plutôt que dans un script » marche aussi bien pour trois outils différents, la phrase ne dit rien.

**Un raccourci qui devient faux.** « PowerShell lit un fichier et crée les comptes » est faux : c'est un script `.ps1`, exécuté sur le contrôleur de domaine par un compte qui en a le droit, et seulement si la politique d'exécution l'autorise. Le détail n'alourdit pas, il est la matière du métier.

**Un mot vague là où il existe un mot juste.** « Inclus dans le système » ne veut rien dire : *livré avec Windows Server*, *inclus dans la licence Windows Server*, *inclus dans l'abonnement Microsoft 365* disent chacun autre chose.

**Un nom d'outil qui n'en est pas un.** « Un outil de gouvernance des identités » n'est pas un nom : on écrit le produit.

**Un outil rangé sous la mauvaise tâche.** Un outil qui configure des machines n'est pas un outil qui crée des comptes, même s'il sait techniquement en créer.

## Où ça se voit

- Dans le pop-up d'un chapitre : le bandeau au-dessus du bloc vert montre, au survol, le paragraphe **Ce que c'est**.
- Dans « Les outils, et leurs alternatives » : les trois paragraphes, dans l'ordre.

Le champ s'appelle `what` dans [`site/src/data/chapters/types.ts`](../site/src/data/chapters/types.ts).

## Le glossaire

Les sigles vivent dans [`site/src/data/glossary.ts`](../site/src/data/glossary.ts), avec
pour chacun : ce que c'est, à quoi ça sert, et **qui en fait**, les éditeurs européens
en premier, parce que c'est le marché visé. Une entrée suffit : le texte des chapitres
ne déclare rien, la reconnaissance se fait à l'affichage, et un sigle n'est souligné
qu'à sa première apparition dans un paragraphe.

## La longueur

Un paragraphe de description dépasse souvent trois lignes, et c'est normal : c'est là
que se joue la précision. Il se replie alors derrière un « voir plus », qui coupe à la
fin d'une phrase. On ne raccourcit pas le texte, on le laisse se déplier à la demande.
