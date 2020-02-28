# Variables JS

## Le calculateur d'approvisionnement à vie
Vous êtes-vous déjà demandé quelle est la quantité d'un "stock à vie" de votre collation préférée ? Ne vous posez plus de questions !
1. Enregistrez votre âge actuel dans une variable.
2. Enregistrez un âge maximum dans une variable.
3. Enregistrez un montant estimé par jour (sous forme de nombre).
4. Calculer la quantité totale que vous mangeriez pour le reste de votre vie.
5. Affichez le résultat à l'écran de la même manière : "Vous aurez besoin de NN pour tenir jusqu'à l'âge mûr de X".
## Le Géomètre
Calculer les propriétés d'un cercle, en utilisant les définitions ici : http://math2.org/math/geometry/circles.htm.
1. Stocker un rayon dans une variable.
2. Calculer la circonférence en fonction du rayon, et sortir "La circonférence est NN".
3. Calculer l'aire sur la base du rayon, et sortir "L'aire est NN".
## Le convertisseur de température
Il fait chaud dehors ! Faisons un convertisseur en suivant les étapes ici.
1. Enregistrer une température en degrés Celsius dans une variable.
2. Convertissez-la en fahrenheit et sortez "NN°C is NN°F".
3. Enregistrez maintenant une température en Fahrenheit dans une variable.
4. Convertissez-la en degrés Celsius et sortez "NN°F est NN°C".
# Functions JS
## Le calculateur d'approvisionnement à vie
Ever wonder how much a "lifetime supply" of your favorite snack is? Wonder no more!
1. Write a function named calculateSupply that:
- takes 2 arguments: age, amount per day.
- calculates the amount consumed for rest of the life (based on a constant max age).
- outputs the result to the screen like so: "You will need NN to last you until the ripe old age of X"
2. Call that function three times, passing in different values each time.
Bonus: Accept floating point values for amount per day, and round the result to a round number.
## Le Géomètre
Créez 2 fonctions qui calculent les propriétés d'un cercle, en utilisant les définitions ici.
1. Créez une fonction appelée calcCircumfrence :
- Passez le rayon à la fonction.
- Calculer la circonférence en fonction du rayon, et sortir "La circonférence est NN".
2. Créez une fonction appelée calcArea :
- Passez le rayon à la fonction.
- Calculez l'aire sur la base du rayon, et sortez "L'aire est NN".

## Le convertisseur de température
Il fait chaud dehors ! Faisons un convertisseur en suivant les étapes ici.
1. Créez une fonction appelée celsiusToFahrenheit :
- Enregistrez une température en degrés Celsius dans une variable.
- Convertissez-la en fahrenheit et sortez "NN°C is NN°F".
2. Créez une fonction appelée fahrenheitToCelsius :
- Enregistrez maintenant une température en fahrenheit dans une variable.
- Convertissez-la en degrés Celsius et obtenez "NN°F is NN°C".
## Instructions
The code of this exercise can be executed via Node.js or in the console tab of your browser's developer tools.
1. Define an `addFavoriteBook(..)` function that receives a single parameter, called `bookName`.
2. If the provided `bookName` string does *NOT* have the word "Great" in it, add it to the `favoriteBooks` array.

Hints:
	- `someString.includes(anotherString)` will return `true` if `anotherString` is found inside `someString`, or `false` otherwise.

	- Use `!` to negate a boolean value (change `true` to `false` or vice versa).

	- `someArray.push(value)` will add a value to the end of the array.

3. Define a `printFavoriteBooks()` function that receives no parameters.

4. `printFavoriteBooks()` should first print a message like "Favorite Books: ..", and include the number of books in the `favoriteBooks` array.

	Hint:

	- Use the \` back-tick operators for strings that need to include values in them.

	- Use `console.log(..)` to print a message to the screen.

5. Finally, `printFavoriteBooks()` should loop through the `favoriteBooks` array and print out each value.

	Make sure to then call the `printFavoriteBooks()` function at the end of the program.

	Hint: Use the `for ( let .. of .. ) { }` style loop.

# Three Pillars of JS

This is an exercise to briefly practice the three pillars of JS: Types / Coercion, Scope / Closures, and `this` / Prototypes.

## Instructions

The code of this exercise can be executed via Node.js or in the console tab of your browser's developer tools.

1. In the `printFavoriteBooks()` function, make sure there's no accidental type conversion (ie, from number to string).

	Hint: Use `String(..)` to coerce something to a string type.

2. Move the `addFavoriteBook(..)` and `printFavoriteBooks()` functions into the `Bookshelf` class as methods. Modify them so they use the `this` keyword to access the `favoriteBooks` array.

	Hint: `class` methods don't use the `function` keyword, just their name.

3. Fill out the definition of the `loadBooks(..)` function, which should receive an instance of the `Bookshelf` class that you will pass to it.

4. `loadBooks(..)` should call the provided `fakeAjax(..)`, using `BOOK_API` as the URL and an inline function expression as the callback.

5. The callback will be passed an array of book names. Loop through this array, passing each book name to the `addFavoriteBook(..)` method of the `Bookshelf` instance passed to `loadBooks(..)`. Then call the `printFavoriteBooks()` method.

6. Create an instance of `Bookshelf` class, and pass it as an argument to `loadBooks(..)`.

	Hint: Class instantiation: `new Whatever()`.