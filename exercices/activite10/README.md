Cette activité est réservée au plus avancés. Dans cette activité, nous allons créer des animations en CSS. En se basant sur l’aide-mémoire CSS, réaliser les exercices suivants :

## Exercice 1

Créer une animation de 2 secondes qui permet de changer de couleur du rouge au bleu.

## Exercice 2

Ajouter les 5 étapes à l’animation ex2 (en utilisant 0%, 25%, 50%, 75%, and 100%):

1. 0% - mettre background color à "red", left position to "0px", top position to: "0px"
2. 25% - mettre background color à "blue", left position to "0px", top position to: "200px"
3. 50% - mettre background color à "green", left position to "200px", top position to: "200px"
4. 75% - mettre background color à "yellow", left position to "200px", top position to: "0px"
5. 100% - Set background color à "red", left position to "0px", top position to: "0px"

## Exercice 3 :

En se basant sur le code suivant, dire que l’animation ex3 dure 1 seconde :

```css
div {
width: 100px;
height: 100px;
position: relative;
background-color: red;
animation-name: example;
animation-duration: 2s;
}
@keyframes example {
0% {background-color: red; left:0px;}
50% {background-color: yellow; left:200px;}
100% {background-color: red; left:0px;}
}
```

## Exercice 4

Modifier animation ex3 pour qu’elle se répète à l’infini.
