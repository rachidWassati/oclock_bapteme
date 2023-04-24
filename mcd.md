## Retour sur un MCD d'un.e apprenant.e

Bonjour <Apprenant>

Avant toute chose excellent travail que tu as rendu là.
Ton MCD est conforme au cahier des charges à l'exception d'une petite erreur entre les tables `USER` et `PRODUCT`.

En effet, un `USER` peut liker 0 ou N `PRODUCT` et un `PRODUCT` peut etre liker par 0 ou N `USER`.

Donc les cardinalités au niveau de la table `USER` et `PRODUCT`, ce n'est pas `1,1` mais `0,N`.

Mise à aprt ça, le reste est bon !!

Prochaine étape: la réalisation de ton MCD sur un logiciel prévu à cet effet.

Voici une liste d'outils qui vont te permettre de réaliser des MCD :

- MySQLWorkbench, mon préféré je te l'avoue, avec celui-ci tu pourras créer tes MCD et MLD (prochaine étape du MCD), il est très puissant, car tu pourras à partir de ton MCD créer directement ta base de données grâce à l'outil "Forward Engineer".
- Lucidchart est un outil de création de diagrammes en ligne, qui permet de créer des MCD. Gratuit pour certaines fonctionnalitées
- JMerise, outil très puissant pour créer des MCD, seul bémol il est payant :-(
- Draw.io est comme Lucidchart, en ligne mais il te permttra de créer des MCD gratuitement, car opensource

Il y a d'autres outils pour créer des MCD, mais tu trouveras largement ton bonheur dans ceux cités ci-dessus
