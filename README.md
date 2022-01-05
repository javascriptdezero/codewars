# Déboguez vos exercices codewars depuis Visual Studio Code

## Installation

Depuis le répertoire racine du dépôt, installez les paquets nécessaires :

```
npm i
```

Choisissez un exercice sur le site codewars, prenons par exemple [Opposite number](https://www.codewars.com/kata/56dec885c54a926dcd001095/train/javascript).

1. Copiez le contenu du bloc **Solution** en haut à droite de l'éditeur dans le fichier `codewars.js`.
2. Copiez le contenu du bloc **Sample Tests** en bas à droite de l'éditeur dans le fichier `codewars.js`.

Votre fichier `codewars.js` doit maintenant ressembler à ça :

```js
// Ne supprimez pas la ligne ci-dessous
const Test = require("@codewars/test-compat");

// Rédigez la fonction répondant à l'exercice ci-dessous
function opposite(number) {
  //your code here
}

// Indiquez le code de test fourni par codewars ci-dessous
// (section Sample Tests en bas à droite de l'éditeur)
describe("Tests", () => {
  it("test", () => {
Test.assertEquals(opposite(1), -1,)
  });
});
```

Rédigez votre code dans la fonction répondant à l'exercice (dans mon exemple il s'agit de la fonction `opposite`).

Vous n'avez plus qu'à exécuter la configuration "Jouer les tests" (définie dans le fichier `.vscode/launch.json`) en appuyant sur `CTRL+F5` ou en faisant menu **Exécuter > Exécuter sans débogage** pour vérifier que votre code est correct.

Si vous souhaitez déboguer votre code, il vous suffit de placer un point d'arrêt dans le corps de la fonction répondant à l'exercice (fonction `opposite` dans mon exemple) puis de lancer le débogueur avec `F5` ou le menu **Exécuter > Démarrer le débogage**.

Profitez de la puissance du débogueur de VSCode pour déboguer votre exercice et réussir tous les tests !

# Formation algorithmique

Ce dépôt a été créé pour aider mes étudiants à apprendre l'algorithmique et devenir performant lors d'entretiens techniques pour décrocher un poste de développeur.

Si vous êtes intéressés par ma formation algorithmique, je vous invite à lire la page de présentation du [module algorithmique de ma formation](https://www.javascriptdezero.com/algorithmique).

N'hésitez pas à me contacter si vous avez des questions.
- Email : jeremy@javascriptdezero.com
- Twitter : [@jeremymouzin](https://twitter.com/jeremymouzin)