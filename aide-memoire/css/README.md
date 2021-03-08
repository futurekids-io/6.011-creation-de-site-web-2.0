# Aide-mémoire CSS

## Plans
- [Créer un lien vers le fichier CSS](#créer-un-lien-vers-le-fichier-css)
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

Pour encore plus d'informations sur le CSS, vous pouvez consulter la documentation du langage sur [le site de W3Schools](https://www.w3schools.com/css/default.asp).

## Créer un lien vers le fichier CSS

 Dans un fichier HMTL. Dans la balise head :

```html
<link rel="stylesheet" type="text/css" href="monstyle.css">
```

## Syntaxe

Dans votre fichier CSS, on utilise la syntaxe suivante :

```css
nomBalise (p, h1, ...) {
  propriete: valeur;
  background-color: red;
  font-size: 14px;
  etc.
}

#id {
  color: blue;
  font-weight: bold;
}

.class {
  margin: auto;
  width: 100%;
}
```

Il est possible de sélectionner plusieurs balises, classes ou identifiants pour les styliser en une fois :

```css
h1, p, .maClass, #monIdentifiant {
  ...
}
```

## Couleurs

<table>
  <tr>
    <td>Couleur du texte</td><td>`color: red`</td>
  </tr>
  <tr>
    <td>Couleur de fond</td><td>`background-color: red`</td>
  </tr>
</table>


Les couleurs peuvent se noter de différentes manières :

<table>
    <tr>
        <th></th>
        <th>Nom</th>
        <th>Hexadecimal</th>
        <th>RGB</th>
    </tr>
    <tr>
        <td style="background-color: black;"></td>
        <td>black</td>
        <td>#000000</td>
        <td>rgb(0, 0, 0)</td>
    </tr>
    <tr>
        <td style="background-color: silver;"></td>
        <td>silver</td>
        <td>#c0c0c0</td>
        <td>rgb(192, 192, 192)</td>
    </tr>
    <tr>
        <td style="background-color: gray;"></td>
        <td>gray</td>
        <td>#808080</td>
        <td>rgb(128,128,128)</td>
    </tr>
    <tr>
        <td style="background-color: white;"></td>
        <td>white</td>
        <td>#ffffff</td>
        <td>rgb(255,255,255)</td>
    </tr>
    <tr>
        <td style="background-color: maroon;"></td>
        <td>maroon</td>
        <td>#800000</td>
        <td>rgb(128,0,0)</td>
    </tr>
    <tr>
        <td style="background-color: red;"></td>
        <td>red</td>
        <td>#ff0000</td>
        <td>rgb(255,0,0)</td>
    </tr>
    <tr>
        <td style="background-color: purple;"></td>
        <td>purple</td>
        <td>#800080</td>
        <td>rgb(128,0,128)</td>
    </tr>
    <tr>
        <td style="background-color: fuchsia;"></td>
        <td>fuchsia</td>
        <td>#ff00ff</td>
        <td>rgb(255,0,255)</td>
    </tr>
    <tr>
        <td style="background-color: green;"></td>
        <td>green</td>
        <td>#008000</td>
        <td>rgb(0,128,0)</td>
    </tr>
    <tr>
        <td style="background-color: lime;"></td>
        <td>lime</td>
        <td>#00ff00</td>
        <td>rgb(0,255,0)</td>
    </tr>
    <tr>
        <td style="background-color: olive;"></td>
        <td>olive</td>
        <td>#808000</td>
        <td>rgb(128,128,0)</td>
    </tr>
    <tr>
        <td style="background-color: yellow;"></td>
        <td>yellow</td>
        <td>#ffff00</td>
        <td>rgb(255,255,0)</td>
    </tr>
    <tr>
        <td style="background-color: navy;"></td>
        <td>navy</td>
        <td>#000080</td>
        <td>rgb(0,0,128)</td>
    </tr>
    <tr>
        <td style="background-color: blue;"></td>
        <td>blue</td>
        <td>#0000ff</td>
        <td>rgb(0,0,255)</td>
    </tr>
    <tr>
        <td style="background-color: teal;"></td>
        <td>teal</td>
        <td>#008080</td>
        <td>rgb(0,128,128)</td>
    </tr>
    <tr>
        <td style="background-color: aqua;"></td>
        <td>aqua</td>
        <td>#00ffff</td>
        <td>rgb(0,255,255)</td>
    </tr>
</table>

Pour trouver exactement la couleur dont vous avez besoin, vous pouvez utiliser <a href="https://www.w3schools.com/colors/colors_picker.asp" target="_blank">le sélecteur de couleur du W3C</a>.

## Typographie

| Nom du paramètre | Description                                | Exemples                                                     |
| ---------------- | ------------------------------------------ | ------------------------------------------------------------ |
| font             | Réglage global d'une police de caractères. | `font: bold 14px Arial;`                                       |
| font-family      | Choix de la police de caractères.          | `font-family:  Georgia, serif;`<br />`font-family:  Arial, sans-serif;` |
| font-size        | Taille de la police de caractères.         | `font-size: 1em;`<br />`font-size: 14px;`                            |
| font-style       | Style de la police                         | `font-style: normal;`<br />`font-style: italic;`<br />`font-style: oblique;` |
| font-weight      | Epaisseur de la police                     | `font-weight: normal;`<br />`font-weight: bold;`<br />`font-weight: bolder;` |
| text-decoration  | Soulignement ou surlignement.              | `text-decoration: none;`<br />`text-decoration: underline;`<br />`text-decoration: line-through;`<br />`text-decoration: overline;` |
| font-variant     | Affichage en petites majuscules.           | `font-variant: normal;`<br />`font-variant: small-caps;`     |
| text-transform   | Mise en majuscules/minuscules.             | `text-transform: none;`<br />`text-transform: capitalize;`<br />`text-transform: uppercase;`<br />`text-transform: lowercase;` |
| text-align       | Alignement du texte                        | `text-align: left;`<br />`text-align: center;`<br />`text-align: right;`<br />`text-align: justify;` |
| text-indent      | Décallage de la première ligne du texte    | `text-indent: 5px;`                                          |
| line-height      | Hauteur des caractères                     | `line-height: normal;`  <br />`line-height: 12px;`           |
| letter-spacing   | Espacement entre les caractères            | `letter-spacing: 12px;`                                      |
| word-spacing     | Espacement entre les mots                  | `word-spacing: 12px;`                                        |

## Arrière-plan

| Paramètre             | Description                                                  | Exemples                                                     |
| --------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| background            | Caractéristique globale d'un fond.                           | `background-color:  red url(images/fond.png) no-repeat scroll center top;` |
| background-color      | Couleur de fond                                              | `background-color: red ;`                                    |
| background-image      | Image de fond.                                               | `background-image: url(‘lienVersImage’);`                    |
| background-repeat     | Répétition de l'image de fond.                               | `background-repeat:  repeat;`<br />`background-repeat:  repeat-x;`<br />`background-repeat:  repeat-y;`<br />`background-repeat:  no-repeat;` |
| background-attachment | Fixation de l'image sur le navigateur  (contre le défilement). | `background-attachment:  scroll;`<br />`background-attachment:  fixed;` |
| background-position   | Position de l'image sur le fond (x, y).                      | `background-position:  left top ;`<br />`background-position:  center center ;`<br />`background-position:  right bottom ;`<br />`background-position:  50% 50% ;`<br />`background-position: 5px 10px;` |

## Bloc et bordure

| Paramètre    | Description                                | Exemples                                                     |
| ------------ | ------------------------------------------ | ------------------------------------------------------------ |
| margin       | Réglage des marges autour des blocs        | `margin: 5px 5px 5px 5px;`<br />`margin-top: 10px;`<br />`  margin-bottom: 10px; `<br />` margin-left: 10px; `<br />` margin-right: 10px;` |
| padding      | Réglage des marges à l'intérieur des blocs | `padding: 1px 2px 3px 4px;`<br />`padding-top: 10%;`<br />`padding-bottom: 20px;`<br />`padding-right: 30px;`<br />`padding-left:  40px;` |
| border       | Affichage global d'une bordure.            | `border: 5px dotted green;`                                  |
| border-width | Largeur de la bordure.                     | `border-width: 1px 2px 3px 4px;`<br />`border-width-top: 1px;`<br />`border-width-bottom: 1px;`<br />`border-width-left: 1px;`<br />`border-width-right: 1px;` |
| border-color | Couleur de la bordure.                     | `border-color: red;`                                         |
| border-style | Type de la bordure.                        | `border-style: none;`<br />`border-style: solid;`<br />`border-style: dotted;`<br />`border-style: dashed;`<br />`border-style: inset;`<br />`border-style: outset;`<br />`border-style: double;`<br />`border-style: groove;`<br />`border-style: ridge;` |
| cursor       | Type de pointeur affiché pour la souris.   | `cursor: auto;`<br />`cursor: pointer;`<br />`cursor: defaut;`<br />`cursor: crosshair;`<br />`cursor: move;`<br />`cursor: help;`<br />`cursor: wait;` |

## Tableau

| Paramètre       | Description                                                  | Exemples                                                     |
| --------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| border-collapse | Séparation ou collage des cellules du  tableau (espace ou non entre les cellules). | `border-collapse: separate;`<br />`border-collapse: collapse;` |
| border-spacing  | Taille de l'espacement entre les cellules  (si on est en "border-collapse: separate;") | `border-spacing: 3px;`                                       |
| empty-cell      | Gère l'affichage ou non d'une cellule si  elle est vide.     | `empty-cell: hide;`<br />`empty-cell: show;`                 |
| caption-side    | Placement de la légende du tableau.                          | `caption-side: top;`<br />`caption-side: right;`<br />`caption-side: bottom;`<br />`caption-side: left;` |
| vertical-align  | Alignement vertical dans la cellule d'un  tableau.           | `vertical-align: baseline;`<br />`vertical-align: top;`<br />`vertical-align: middle;`<br />`vertical-align: bottom;` |

## Positionnement

| Paramètre                | Description                                                  | Exemples                                                     |
| ------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| display                  | Mode d'affichage (ou non) d'un bloc ou d'un  élément.        | `display: none;`<br />`display: block;`<br />`display: inline;`<br />`display: inline-block;`<br />`display: flex;` |
| width, height            | Largeur d'un block. height : Hauteur d'un  block.            | `width: 60px;`<br />`min-width: 100px;`<br />`max-width: 100px;`<br />`height: 60px;`<br />`min-height: 100px;`<br />`max-height: 100px;` |
| position                 | Position d'un block.                                         | `position: static;`<br />`position: absolute;`<br />`position: fixed;`<br />`position: relative;` |
| top, right, left, bottom | Pour placer un bloc (hors static). par  rapport à un ou deux bords. | `top: 5px;`<br />`right: 10em;`<br />`bottom: 0;`<br />`left: 10%;` |
| float                    | Pour laisser flotter un bloc à droite ou à  gauche.          | `float: none ;`<br />`float: left ;`<br />`float: right ;`   |
| clear                    | Pour obliger un bloc à se placer derriere un  flottant.      | `clear: none;`<br />`clear: left;`<br />`clear: right;`<br />`clear: both;` |
| overflow-x, overflow-y   | Pour gérer le dépassement du contenu d'un objet en horizontal ou vertical | `overflow-x: auto;`<br />`overflow-x: visible;`<br />`overflow-y: hidden;`<br />`overflow-y: scroll;` |
| z-index                  | hors static, permet de gérer l'empilement  des blocs.        | `z-index: auto;`<br />`z-index: 10;`<br />`z-index: 999;`    |

## Liste

| Paramètre           | Description                                                  | Exemples                                                     |
| ------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| list-style          | Réglage globale d'une liste.                                 | `list-style: circle outside url(toto.jpg);`                  |
| list-style-type     | Type de liste.                                               | `list-style-type: none;`<br /> `list-style-type: disc;`<br /> `list-style-type: circle;`<br /> `list-style-type: square;`<br /> `list-style-type: decimal;`<br /> `list-style-type: upper-roman;`<br /> `list-style-type: lower-alpha;`<br /> `list-style-type: upper-alpha;` |
| list-style-position | Position du marqueur de liste dans la liste  ou hors de la liste (outside est plus normal). | `list-style-position: outside;`<br /> `list-style-position: inside;` |
| list-style-image    | Image pour remplacer le marqueur de la  liste.               | `list-style-image: none;` <br />`list-style-image: url(images/point.jpg);` |

## Sélecteurs

| Paramètre          | Description                                                  | Exemples                                                     |
| ------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ::after / ::before | Insère du contenu avant ou après l’élément                   | `div::after {content: "hello";}`<br />`div::before {content: "hello";}` |
| :active            | Changement d’un lien lorsqu’il est actif  (lors du clic)     | `a:active { color: red; }`                                   |
| ::first-letter     | Sélectionne la première lettre d’un élément                  | `p::first-letter { font-weight: bold; color: red; }`         |
| ::first-line       | Sélectionne la première ligne d’un élément                   | `p::first-line { font-weight: bold; color: red; }`           |
| ::first-child      | Sélectionne le premier enfant d’un élément                   | `p:first-child { font-size: 30px; }`                         |
| ::first-of-type    | Sélectionne la première occurrence d’un  élément             | `p:first-of-type { font-size: 15px; }`                       |
| :focus             | Sélectionne un élément qui est activé par le  clavier ou la souris | `textarea:focus { background: pink; }`<br />`a:focus { background: pink; }` |
| :hover             | Sélectionne un élément lorsque la souris est  dessus         | `a:hover { color: green; text-decoration: underline overline;}` |
| :last-child        | Sélectionne le dernier enfant d’un élément                   | `p:last-child { font-size: 30px; }`                          |
| :last-of-type      | Sélectionne la première occurrence d’un  élément             | `p:last-of-type { font-size: 15px; }`                        |
| :visited           | Changement d’un lien après qu’il ait été  visité             | `a:visited { color: gray; }`                                 |

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