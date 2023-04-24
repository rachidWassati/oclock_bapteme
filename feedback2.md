# FeedBack 2

Bonjour Apprenant 2

Dans un premier je tiens à te féliciter pour ton travail !

## Concernant l'application:

Excellent rendu, quelques oublis toutefois, au niveau de la page de recherche, on ne peut rechercher des cartes que par élément. Les autres routes non pas été implémentées.
De plus tu affiches une liste des résultats et il faut choisir une carte en cliquant sur le lien pour la voir et enfin pouvoir l'ajouter au Deck, donc trop d'actions. Il faut faciliter à l'utilisateur l'utilisation de ton app, mais à part ça c'est nickel.

En ce qui concerne le Deck, bien vu le bouton pour revenir à la page d'accueil et nous permettre d'ajouter d'autres cartes, attention tout de même car on ne peut pas retirer la carte sélectionnée du deck, tu as oublié le [-] sur la carte.
L'idéal aurait été, depuis la page d'accueil, de mettre en surbrillance les cartes choisies pour le deck, de changer le [+] en [-] une fois la carte sélectionnée et enfin aller voir dans le deck les cartes choisies.

## Concernant le code:

Le dossier 'views' est bien structuré, tes controllers sont bien nommés. Petit bémol sur certains noms de méthodes:

- `addDeck` sous entend l'ajout d'un deck, je pense que tu voulais dire `addCardToDeck`, ou `addCard`.
- `item` n'est pas très clair comme nom, `cardDetail` lùest plus.

Pense à commenter ton code, pour toi avant tout (quand tu y reviendras dans 6 mois, tu seras content de le trouver commenté) et pour les autres qui liront ton code.
Ton controller 'cardsController' n'est pas indispensable, ta méthode 'item' tu peux la mettre dans le mainController.
Pense à sauter une ligne entre chaque méthode de controller ou dataMapper pour plus de lisibilité.

Pour finir, la création du deck dans la session est présente dans le controller `addDeck`, ce qui n'est pas pratique.

En faire un middleware, qu'on invoquerait dans index.js sera plus pratique.
