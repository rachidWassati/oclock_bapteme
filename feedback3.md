# Feedback 3

Bonjour Apprenant 3

Je tiens à féliciter pour l'effort donné dans ce travail, je peux voir que tu as fait de ton mieux pour aller jusqu'au bout.

## Concernant l'application

Dans la page d'accueil, tu affiches bien toutes les cartes, mais attention, il y a un problème de css, car c'est pas très lisible.

De plus tu as mis l'image de la carte ainsi qu'un lien pour afficher la carte en détail, tu aurais pu fusionner les deux pour qu'en cliquant sur l'image cela nous mène au détail de la carte.

Quand on clique sur une carte, on a un message d'erreur disant que `card is not defined`. Cette erreur vient du fait que dans ton controller `mainController` dans la methode `cardPage`, tu envoies dans ton rendu `oneCard` et que dans le template `cardDetails.ejs` tu fais appel à la variable `card` qui n'existe nul part dans ton controller.

De plus dans ce même template, tu boucles sur `card`, alors que ta méthode getCard, te renvoie un objet et non pas un array d'objets.

Pour ce qui est de la recherche par critères, tu as implémenté la recherche par élément, c'est très bien ! Mais elle ne fonctionne pas car tu as invoqué une méthode qui n'existe pas `cardElement`, il fallait invoqué la méthode `getCardByElement`.

Mise à part ça la logique métier est bonne.

## Concernant le code

Le code est propre, structuré, aéré et bien commenté, dommage qu'il n'y ait pas plus de méthodes à lire ;-)

## Points à revoir

- Revoir les requêtes SQL pour pouvoir implémenter les recherches par critères.

Dans l'ensemble, on constate que tu as mis beaucoup du tien, et qu'avec des notions plus solides tu aurais mis en place toutes les fonctionnalités attendus.
