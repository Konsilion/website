---
hide:
    - toc
comments: true
---

<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js"></script>

[Retour]({{ katalog_site }}/admin){ .md-button .md-button--primary style="float:right; margin: 0 0 25px 5px; padding: 5px 15px;" target="_self"}

---

# Comment créer et éditer une page Web ?

---

Voici un tutoriel qui vous expliquera comment ajouter une page web et l'éditer en deux étapes seulement.

=== "Étape 1"

    [Étape 1 - Créer le fichier]({{ katalog_repo }}/new/master/docs/pages){ .md-button .md-button--primary style="float:right; margin: 15px;" target="_blank"}

    ## Créer la page et écrire le contenu

    Créez le fichier markdown correspondant à la page de votre site en cliquant sur ce bouton. 

    * Ce fichier doit porter l'extension `.md`, par exemple : `accueil.md` ou `ma-page.md`,

    * Pas d'espace dans le nom de votre fichier,

    * Placer le fichier dans `pages` ou un sous dossier `pages/sous-dossier/ma-page.md`,

    * Copier le modèle suivant dans le fichier,
    
    * et enregistrer.

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

    Chaque fichier markdown doit commencer par une ligne de front matter qui définit le titre de la page et d'autres paramètres.

    ??? info "À quoi servent les lignes `<script>` ?"

        Un script est un programme informatique écrit dans le langage JavaScript. Ils sont utilisés pour ajouter de la fonctionnalité à votre plateforme web, comme des actions en réponse aux événements de l'utilisateur, des saisies de texte dans des formulaires ou des gestions de compatibilité entre Mkdocs et Datami.

        Les scripts JavaScript sont généralement inclus dans le code HTML d'une page web à l'aide de la balise `<script>`.

        Ils ne sont **pas obligatoires pour les pages**, mais voici les fonctionnalités qu'ils apportent :

        * Modifier la page en cours :

        * Créer une page voisine :

        * Menu glissant :

=== "Étape 2" 

    [Étape 2 - Modifier mkdocs.yml]({{ katalog_repo }}/edit/master/mkdocs.yml){ .md-button .md-button--primary style="float:right; margin: 15px;" target="_blank"}

    ## Référencer votre page

    Dans le répertoire du projet, vous trouverez un fichier mkdocs.yml qui contient les paramètres de votre projet. Ouvrez ce fichier en cliquant sur le bouton et modifiez-le pour définir l'arborescence de vos pages. Par exemple :

    <div style="max-width: 650px; margin: 50px auto;" markdown>
        ``` yaml title="Éditer la navigation/ référencement dans mkdocs.yml"
        nav:
          - Accueil: pages/accueil.md
          - Tutoriels:
            - Introduction: pages/ma-page.md
            - Étape 1: pages/etape-1/ma-deuxieme-page.md
          - À propos: pages/contact.md
        ```
    </div>

=== "Aller plus loin"

    ### En savoir plus sur l'écriture Markdown

    Le markdown est un langage de balisage léger qui permet de formater du texte de manière simple et rapide. Il a été créé en 2004 par John Gruber et Aaron Swartz dans le but de rendre la mise en forme de documents plus facile et plus rapide. Le markdown est souvent utilisé pour la rédaction de documents sur internet, comme des articles de blog, des documents de documentation, etc.

    Pour utiliser le markdown, il suffit d'ajouter des symboles spéciaux devant ou autour des mots ou des phrases que vous voulez mettre en forme.

    [Débuter avec Markdown](https://blog.wax-o.com/2014/04/tutoriel-un-guide-pour-bien-commencer-avec-markdown/){ .md-button .md-button--secondary target="_blank"}

    ### Au besoin, compléter avec du code HTML

    Vous pouvez également ajouter du contenu HTML dans vos fichiers markdown en utilisant des balises HTML. Par exemple, pour ajouter une image à votre page suivi d'un saut de ligne, vous pouvez utiliser la balise <img> et <br> comme ceci :

    <div style="max-width: 650px; margin: 50px auto;" markdown>
        ``` html title="Ajout ponctuel d'éléments HTML"
        <img src="image.jpg" alt="Description de l'image">

        <br>
        ```
    </div>

---
