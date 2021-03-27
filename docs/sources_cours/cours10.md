class: middle

<h1>Création <br/>de <span class="secondary-color">site web<span></h1>

### Cours 10

#### HTML & CSS

#### &copy; Mikaël Ruffieux, 03.2021

<img class="first-slide-image" src="../sources_cours/img/first_slide.jpg">
---

# Petit <span class="secondary-color">rappel</span>

```css
.maBox { 
  padding: 10px; /* 10px de chaque côté */ 
  margin: 10px auto; /* top & bottom - left & right */

  border: 1px solid black; /* épaisseur - type de trait - couleur */
}
.ma2emeBox {
  margin: 20px 10px 5px 0px; /* top - right - bottom - left */
}
```
<div style="text-align: center">
  <img style="max-height: 200px; width: auto;" src="../sources_cours/img/cours9_margin-padding.png" />
</div>

<small>Source image : <a href="https://miro.medium.com/max/725/1*FqGQIGmGdW5EetfS3HFkvA.png" target="_blank">Medium.com</a></small>

---

# Petit <span class="secondary-color">rappel</span>

Une [pseudo-classe](https://github.com/futurekids-io/6.011-creation-de-site-web-2.0/tree/main/aide-memoire/css#s%C3%A9lecteurs) est un **élément HTML** dans un **état spécial**.

Principalement utilisées pour les liens, il est toutefois possible d'utiliser une pseudo-classe sur **toutes les balises HTML**.

<style>
#lien { color: black; padding: 0px; margin: 0px;}

#lien:hover {color: white;background-color: red;}

#lien:active {background-color: green;}
</style>

<a href="#5" id="lien" ><h3>Mon super lien</h3></a>

```css
a { /* Lien normal */
  color: black;
}

a:hover { /* Au survol de la souris */
  color: white;
  background-color: red;
}

a:active { /* Lien sélectionné */
  background-color: green;
}
```

---
# Les <span class="secondary-color">animations</span> en CSS

Une animation en CSS permet de modifier progressivement l'apparence d'un élément. [Aide-mémoire](https://github.com/futurekids-io/6.011-creation-de-site-web-2.0/tree/main/aide-memoire/css#animations)

<div id="div"></div>
<style>
#div {
width: 50px;
height: 50px;
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
</style>

```css
#div {
  width: 50px;
  height: 50px;
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

---
# Rappel sur <span class="secondary-color">vos projets</span>

- Un menu
- Si possible, au minimum 2 pages
- Une zone de contenu principale
- Des images
- Un pied de page avec votre Prénom Nom
- ... et tout ce que **vous** avez envie de mettre sur votre site 

---

# Feedback sur le <span class="secondary-color">cours</span>

Afin d'avoir votre avis sur le cours, vous trouverez le lien vers un questionnaire sur la page du cours.

- Seriez-vous motivé.e.s à continuer ce cours, dans un futur proche ?
- *Would you like to continue immediately this course ?*

- Qu'est-ce que vous aimeriez apprendre par la suite ?
- *What would you like to learn next ?*

- Pourquoi est-ce que vous aimeriez en apprendre plus dans le domaine du web ?
- *Why would you want to learn further ?*

---
class: center, middle

<h1 class="secondary-color">À vos projets ! </h1>


???

<!-- ################ Fin de la présentation ################### -->