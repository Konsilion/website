---
comments: true
---


[Retour]({{ katalog_site }}/admin){ .md-button .md-button--primary style="float:right; margin: 0 0 25px 5px; padding: 5px 15px;" target="_self"}

<hr><br>

# Tout ce qu'il faut savoir sur les pages Web.

---

Voici un tutoriel qui vous expliquera comment écrire une page web avec Katalog :

## Créer le fichier et écrire le contenu

[Créer le fichier]({{ katalog_site }}/admin){ .md-button .md-button--secondary style="float:right; margin: 0 0 25px 5px; padding: 5px 15px;" target="_self"}

---

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

[En savoir plus]({{ katalog_site }}/admin){ .md-button .md-button--secondary style="float:right;" target=""}



### Pourquoi copier les quelques lignes de `<script>`


## Référencer votre page

[Référencer ma page]({{ katalog_site }}/admin){ .md-button .md-button--secondary style="float:right; margin: 0 0 25px 5px; padding: 5px 15px;" target="_self"}

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



<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/slider-nav.js" defer></script> <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js" defer></script> <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/add-page.js" defer></script>





{% if page.meta.comments %}
   <h2 id="__comments">{{ lang.t("meta.comments") }}</h2>
   <!-- Insert generated snippet here -->
   <script src="https://giscus.app/client.js"
           data-repo="konsilion/website-giscus"
           data-repo-id="R_kgDOIspq8w"
           data-category="General"
           data-category-id="DIC_kwDOIspq884CTVE0"
           data-mapping="pathname"
           data-strict="0"
           data-reactions-enabled="1"
           data-emit-metadata="0"
           data-input-position="bottom"
           data-theme="preferred_color_scheme"
           data-lang="fr"
           crossorigin="anonymous"
           async>
   </script>
   <!-- Synchronize Giscus theme with palette -->
   <script>
    var giscus = document.querySelector("script[src*=giscus]")
    /* Set palette on initial load */
    var palette = __md_get("__palette")
    if (palette && typeof palette.color === "object") {
      var theme = palette.color.scheme === "slate" ? "dark" : "light"
      giscus.setAttribute("data-theme", theme) 
    }
    /* Register event handlers after documented loaded */
    document.addEventListener("DOMContentLoaded", function() {
      var ref = document.querySelector("[data-md-component=palette]")
      ref.addEventListener("change", function() {
        var palette = __md_get("__palette")
        if (palette && typeof palette.color === "object") {
          var theme = palette.color.scheme === "slate" ? "dark" : "light"

          /* Instruct Giscus to change theme */
          var frame = document.querySelector(".giscus-frame")
          frame.contentWindow.postMessage(
            { giscus: { setConfig: { theme } } },
            "https://giscus.app"
          )
        }
      })
    })
   </script>
{% endif %}
