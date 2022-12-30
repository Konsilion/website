---
hide:
   - toc
---

[Retour]({{ katalog_site }}/pages/accueil){ .md-button .md-button--primary style="float:right; margin: 25px 5px; padding: 5px 15px;" target="_self"}
 
<hr>

# Créer une page Web

[Créer une page]({{ katalog_repo }}/new/master/docs/pages/){ .md-button .md-button--secondary style="float:right; margin: 10px;" target="_self"}
    
---

Voici un tutoriel qui vous expliquera comment écrire une page web avec Katalog :

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


Créez les fichiers markdown correspondants aux pages de votre site. Vous pouvez utiliser un éditeur de texte simple pour cela. Chaque fichier markdown doit commencer par une ligne de front matter qui définit le titre de la page et d'autres paramètres. Par exemple :


``` yaml title="Navigation dans mkdocs.yml"
---
title: Introduction
template: tutorial.html
---

# Introduction

Bienvenue dans notre tutoriel sur MkDocs !
```

Vous pouvez également ajouter du contenu HTML dans vos fichiers markdown en utilisant des balises HTML. Par exemple, pour ajouter une image à votre page, vous pouvez utiliser la balise <img> comme ceci :

``` html title="Ajout ponctuel d'éléments HTML"
<img src="image.jpg" alt="Description de l'image">
```

Pour prévisualiser votre site en local, utilisez la commande mkdocs serve dans votre terminal. Vous pouvez alors accéder à votre site en ouvrant votre navigateur et en saisissant l'adresse http://localhost:8000.

Lorsque vous êtes prêt à publier votre site, utilisez la commande mkdocs build pour générer les fichiers HTML statiques de votre site. Vous pouvez alors télécharger ces fichiers sur un serveur web pour les rendre accessibles en ligne.

J'espère que ce tutoriel vous aidera à démarrer avec MkDocs. N'hésitez pas à me poser d'autres questions si vous avez besoin de plus d'aide.



<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/slider-nav.js" defer></script> <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js" defer></script> <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/add-page.js" defer></script>
