---
comments: true
---


[Retour]({{ katalog_site }}/admin){ .md-button .md-button--primary style="float:right; margin: 0 0 25px 5px; padding: 5px 15px;" target="_self"}

<hr><br>

# Comment créer et éditer une page Web ?

---

Voici un tutoriel qui vous expliquera comment ajouter une page web et l'éditer.

## Créer le fichier et écrire le contenu

[Étape 1 - Créer le fichier]({{ katalog_site }}/admin){ .md-button .md-button--secondary style="float:right; margin: 15px;" target="_self"}

---

Créez les fichiers markdown correspondants aux pages de votre site. Vous pouvez utiliser un éditeur de texte simple pour cela. Chaque fichier markdown doit commencer par une ligne de front matter qui définit le titre de la page et d'autres paramètres. Par exemple :

<div style="max-width: 650px; margin: 50px auto;" markdown>
  ``` html title="Page Web - Modèle de base"
  ---
  title: Introduction
  comments: true
  hide:
    - toc
  ---

  # Introduction

  Bienvenue dans notre tutoriel sur MkDocs !

  (votre texte ici ...)



  <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/slider-nav.js" defer></script>
  <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js" defer></script> 
  <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/add-page.js" defer></script>
  ```
</div>

??? info "À quoi servent les lignes `<script>` ?"

    Un script est un programme informatique écrit dans le langage JavaScript. Ils sont utilisés pour ajouter de la fonctionnalité à votre plateforme web, comme des actions en réponse aux événements de l'utilisateur, des saisies de texte dans des formulaires ou des gestions de compatibilité entre Mkdocs et Datami.

    Les scripts JavaScript sont généralement inclus dans le code HTML d'une page web à l'aide de la balise `<script>`.

    Ils ne sont **pas obligatoires pour les pages**, mais voici les fonctionnalités qu'ils apportent :

    * Modifier la page en cours :

    * Créer une page voisine :

    * Menu glissant :

### En savoir plus sur l'écriture Markdown

Le markdown est un langage de balisage léger qui permet de formater du texte de manière simple et rapide. Il a été créé en 2004 par John Gruber et Aaron Swartz dans le but de rendre la mise en forme de documents plus facile et plus rapide. Le markdown est souvent utilisé pour la rédaction de documents sur internet, comme des articles de blog, des documents de documentation, etc.

Pour utiliser le markdown, il suffit d'ajouter des symboles spéciaux devant ou autour des mots ou des phrases que vous voulez mettre en forme.

[Débuter avec Markdown](https://blog.wax-o.com/2014/04/tutoriel-un-guide-pour-bien-commencer-avec-markdown/){ .md-button .md-button--secondary}

### Au besoin, compléter avec du code HTML

Vous pouvez également ajouter du contenu HTML dans vos fichiers markdown en utilisant des balises HTML. Par exemple, pour ajouter une image à votre page suivi d'un saut de ligne, vous pouvez utiliser la balise <img> et <br> comme ceci :

``` html title="Ajout ponctuel d'éléments HTML"
<img src="image.jpg" alt="Description de l'image">

<br>
```

## Référencer votre page

[Étape 2 - Référencer la page]({{ katalog_site }}/admin){ .md-button .md-button--secondary style="float:right; margin: 15px;" target="_self"}

---

Dans le répertoire du projet, vous trouverez un fichier mkdocs.yml qui contient les paramètres de votre projet. Ouvrez ce fichier et modifiez-le pour définir le titre de votre site et les pages que vous souhaitez inclure. Par exemple :

``` yaml title="Navigation dans mkdocs.yml"
site_name: Mon site MkDocs

nav:
  - Accueil: index.md
  - Tutoriels:
    - Introduction: tutorial-intro.md
    - Étape 1: tutorial-step1.md
    - Étape 2: tutorial-step2.md
  - À propos: about.md
```




Pour prévisualiser votre site en local, utilisez la commande mkdocs serve dans votre terminal. Vous pouvez alors accéder à votre site en ouvrant votre navigateur et en saisissant l'adresse http://localhost:8000.

Lorsque vous êtes prêt à publier votre site, utilisez la commande mkdocs build pour générer les fichiers HTML statiques de votre site. Vous pouvez alors télécharger ces fichiers sur un serveur web pour les rendre accessibles en ligne.

J'espère que ce tutoriel vous aidera à démarrer avec MkDocs. N'hésitez pas à me poser d'autres questions si vous avez besoin de plus d'aide.
