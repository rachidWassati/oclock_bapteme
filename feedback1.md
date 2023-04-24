# Feedback 1

Bonjour Apprenant 1,

Avant toute chose, excellent travail que tu as rendu là!

Au niveau de l'application, tu as bien répondu à toutes les attentes.
Ce qui aurait été super c'est de ne pas rediriger l'utilisateur vers le Deck à chaque fois qu'il sélectionne les cartes, mais plutôt de les mettre en surbrillance et de changer le [+] en [-] sur la carte.
Et une fois ces cartes choisies il peut se rendre sur le Deck

Au niveau de la recherche par critères:
Attention, il y a une petite erreur d'affichage quand un utilisateur fait une recherche par élément, dans la page des résultats, on voit un NaN s'afficher au lieu de l'élément.
Rien de grave mais c'est dut au fait que tu as mis un + devant searchedElement dans le controller 'searchByElement' à la ligne 22 (avec ce '+' tu convertis searchedElement en type Number)
A part ça tout est nickel.

Au niveau du code:
+1 pour la structure de tes 'views' et avoir mis le middleware qui gère la session dans un fichier à part.
Attention toutefois à la nomination de celui-ci, le nom 'middleware.js' est trop vague, il faut lui donner un nom plus explicite, comme 'createSession' ou 'session'.
Pour rester dans le sujet du nommage, ton controller 'cardController' gère plus le Deck que les cartes à proprement parlé, 'deckController' aurait été plus pertinent comme nom.

+1 pour les commentaires dans ton code, ça aide vraiment à s'y retrouver.
Pense toutefois à nettoyer ton code de toutes les console.log() de tests que tu as fait, ainsi que les bout de code en commentaires qui ne sont plus utiles, et enfin des fonctions qui ne sont pas utilisées comme 'searchElementByNull' dans dataMapper.js
Et enfin dernier conseil, aère un peu plus de code pour une meilleure lisibilité, comme des sauts de lignes entre chaque méthode, ça m'aidera moi ( ;-) ) et tes futurs collègues à lire ton code plus facilement
