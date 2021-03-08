# Aide-mémoire CSS

***Ce document est en cours de rédaction***

## Plan
- [Syntaxe](#syntaxe)
- [Couleurs](#couleurs)
- [Typographie](#typographie)
- [Arrière-plan](#arrière-plan)
- [Bloc et bordure](#bloc-et-bordure)
- [Tableau](#tableau)
- [Positionnement](#positionnement)
- [Liste](#liste)
- [Sélecteurs](#sélecteurs)

**Pour les plus avancé-e-s**
- [Animations](#animations)
- [Transitions](#transitions)

## Syntaxe
## Couleurs
<style>
.colors tr:nth-child(1) { background: red; }
.colors tr:nth-child(2) { background: orange; }
.colors tr:nth-child(3) { background: green; }
</style>

<div class="colors">
    <table>
        <tr>
            <td></td><td>red</td>
        </tr>
    </table>
</div>

<iframe src="https://www.w3schools.com/colors/colors_picker.asp">

<a href="https://www.w3schools.com/colors/colors_picker.asp" target="_blank">Le sélecteur de couleur du W3C</a>

## Typographie
## Arrière-plan
## Bloc et bordure
## Tableau
## Positionnement
## Liste
## Sélecteurs
## Animations

**Exemple**

```css
@keyframes stretch {
    /* On déclare ici les actions de l'animation */
}
.element {
    animation-name: stretch;
    animation-duration: 1.5s;
    animation-timing-function: ease-out;
    animation-delay: 0s;
    animation-direction: alternate;
    animation-iteration-count: infinite;
    animation-fill-mode: none;
}
/* On peut aussi écrire la classe .element comme ceci : */
.element {
    animation:
        stretch
        1.5s
        ease-out
        0s
        alternate
        infinite
        none
        running;
}
```

## Transitions

**Exemple**

```css
div {
    width: 100px;
    height: 100px;
    background: red;
    transition: width 2s;
}

div:hover {
    width: 300px;
}
```