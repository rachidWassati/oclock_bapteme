# Methode fetch()

Bonjour Apprenant 1,

La méthode `fetch()` est utilisée pour récupérer des données depuis un serveur distant (le plus souvent). Anciennement on utilisait la méthode `XMLHttpRequest`.

La méthode `fetch()` renvoie une réponse sous forme de promesse, tiens voici un exemple :

```
fetch('https://api.fr/v1/cards')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error(error));
```

Ici dans cet exemple on lance une requête sur l'URL `https://api.fr/v1/cards` pour récupérer toutes les cartes. Ce serveur distant va nous envoyé une `response`.

La méthode `then()` (qui veut dire ensuite, en somme: "suite à la réponse reçu") va récupérer cette réponse et la convertir en json avec la méthode `json()`.
Et cette méthode `json()` tout comme la méthode `fetch()` va également renvoyer une promesse, c'est pour cela qu'on la fait suivre à nouveau par la méthode `then()` ("suite à la convertion en JSON").
Cette dernière méthode `then()` va récupérer les données issues du `json()` et on va les afficher avec une `console.log()`

Et enfin la méthode `catch()` est utilisée pour attraper une exception et l'afficher en cas d'erreur. Les erreurs les plus courantes sont une url erronée, des droits d'accès à l'API qu'on n'a pas ou encore des données inexistantes.

Ce même code peut être écrire de la manière suivante:

```
try {
   const response = await fetch('https://api.fr/v1/cards');
   const data = await response.json();
   console.log(data)
} catch (error) {
   console.error(error)
}
```

J'espère que cette explication t'aura donné une idée de l'utilité et de commment utiliser `fetch()`.

Au besoin n'hésite pas à me solliciter, je t'enverrai des ressources plus détaillées sur cette méthode.
