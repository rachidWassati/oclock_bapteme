# Feedback 4

Bonjour Apprenant 4

Je tiens à féliciter pour l'effort donné dans ce travail, malheureusement beaucoup de fonctionnalités n'ont pas été écrites.
Tu as tout de même essayé et c'est un point à noter.

## Concernant l'application

Dans la page d'accueil, tu affiches bien toutes les cartes, mais on ne peut pas accéder aux détails d'une carte.

Il fallait pas grand chose, la méthode `getCard` de `dataMapper` à besoin d'un id que tu lui fournis grâce à `req.params.id`, et cet ID, tu le récupères depuis ton controller `mainController.cardPage`.

Dans ce même controller, une fois que tu récupères `card`, tu le passes en options de ton `render`, chose que tu as oublié en ligne 20 dans `mainController`

## Points à revoir

- les requêtes SQL pour pouvoir implémenter les recherches par critères.
- le MVC: Le controller récupère les données et les envoies dans le vue.
- la syntaxe EJS

Je suis convaincu que tu as le potentiel pour t'améliorer et progresser, revois les points ci-dessus et essaie de finir l'application.
