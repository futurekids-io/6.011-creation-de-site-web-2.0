# Aide-mémoire HTML 5

## Plan
- [Structure du document](#structure-du-document)
- [Balises de formatage](#balises-de-formatage)
- [Balises de contenu](#balises-de-contenu)
- [Listes](#listes)
- [Liens](#liens)
- [Images](#images)
- [Tableaux](#tableaux)

Pour encore plus d'informations sur le HTML, vous pouvez consulter la documentation du langage sur [le site de W3Schools](https://www.w3schools.com/html/default.asp).

## Structure du document

| Balise                   | Description                                                  |
| ------------------------ | :----------------------------------------------------------- |
| ```<html>...</html>```   | Doit apparaître au début et à la fin du document. Indique que le fichier est codé en HTML. |
| ```<head>...</head>```   | Contient des informations spécifiques à la page et qui ne sont pas affichées. |
| ```<body>...</body>```   | Tout ce qui doit apparaître dans la page web sera entre ces balises. |
| ```<title>...</title>``` | Titre de la page qui est affiché dans l’onglet du navigateur. |

**Exemple**

```html
<!DOCTYPE html>
<html>
  <head>
  	<title>TITRE</title>
  </head>
  <body>
    …
  </body>
</html>
```

## Balises de formatage

```html
<b>Cette balise affiche le texte en gras.</b>
<i>Cette balise affiche le texte en italique.</i>
<u>Et cette balise affiche le texte souligné.</u>
```

## Balises de contenu

| Balise                                    | Description                                                  |
| :----------------------------------------- | :------------------------------------------------------------ |
| ```<h1>...</h1>``` ... ```<h6>...</h6>``` | Titre. Disponible en 6 niveau différent. Chaque niveau a une taille et une épaisseur différente. H1 est le plus au niveau et h6 le plus petit. |
| ```<p>...</p>```                          | Cette balise est utilisée pour organiser des paragraphes dans un texte. |
| ```<div>...</div>```                      | Cette balise est un conteneur générique. Elle permet de créer des sections. |
| ```<br/>```                               | Cette balise est une de celle qui ne se ferme pas. Elle fait un renvoie à la ligne |
| ```<hr>```                                | Cette balise est une de celle qui ne se ferme pas. Elle crée un trait horizontal. |
| ```<section>...</section>```              | Permet de créer des sections telles que entête, chapitre, pied de page, … |
| ```<span>...</span>```                    | Cette balise est un conteneur qui laisse les éléments sur une même ligne. |

## Listes

| Balise                                    | Description                                                  |
| :---------------------------------------- | :----------------------------------------------------------- |
| ```<h1>...</h1>``` ... ```<h6>...</h6>``` | Titre. Disponible en 6 niveau différent. Chaque niveau a une taille et une épaisseur différente. H1 est le plus au niveau et h6 le plus petit. |
| ```<p>...</p>```                          | Cette balise est utilisée pour organiser des paragraphes dans un texte. |
| ```<div>...</div>```                      | Cette balise est un conteneur générique. Elle permet de créer des sections. |

**Exemple**

```html
<ul>
  <li>Ceci est une liste non-ordonnée</li>
  <li>aussi appelée "liste à puces"</li>
</ul>

<ol>
  <li>Et ceci est une liste ordonnée</li>
  <li>ou liste numérotée</li>
</ol>
```

## Liens

| Balise                    | Description                                                  |
| :------------------------ | :----------------------------------------------------------- |
| ```<a href="#">...</a>``` | Cette balise est un lien. Dans le *href* il faut mettre un lien url ou un lien vers une autre page web locale. |

**Exemple**

```html
<a href="">Ce lien est un lien interne, il mène vers une autre page du site.</a>
<a href="www.google.com" target="_blank">Ce lien est un lien externe, il mène vers un autre site internet, on y ajoute donc l'attribut target</a>
```

## Image

| Balise                          | Description                                                  |
| :------------------------------ | :----------------------------------------------------------- |
| ```<img src="..." alt="...">``` | Cette balise sert à afficher une image. Dans *src* il faut mettre l’adresse de l’image soit par un lien URL soit par un lien en local. L’attribut *alt* est l’information qui s’affiche lorsque l’image ne se charge pas. |

**Exemple**

```html
<img src="chat.png" alt="Une image de chat">
```

## Tableaux

| Balise                   | Description                                                  |
| :----------------------- | :----------------------------------------------------------- |
| ```<table>...</table>``` | Cette balise permet d’ouvrir un tableau.                     |
| ```<tr>...</tr>```       | Cette balise permet de créer une ligne de tableau. Elle peut se mettre uniquement à l’intérieur d’une balise *table*. |
| ```<th>...</th>```       | Cette balise crée une case d’un tableau, mais représente l’entête. Elle peut se mettre uniquement à l’intérieur d’une balise *tr* (et se met à la place d’un *td*). |
| ```<td>...</td>```       | Cette balise crée une case d’un tableau. Elle peut se mettre uniquement à l’intérieur d’une balise *tr*. |

**Exemple**

```html
<table>
  <tr>
    <th>Balise</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Voici un exemple d'utlisation des balises de tableaux</td>
    <td>Cet exemple correspond plus ou moins au tableau ci-dessus.</td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
  </tr>
</table>
```