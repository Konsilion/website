---
hide:
  - toc
---




![Repertoire GitHub](https://raw.githubusercontent.com/Konsilion/website/master/media/logo-github.png){ .md-button .md-button--primary onclick="window.open('{{ katalog_repo }}','_blank');" style="float:right; height: 40px; padding: 5px; margin: 5px; border-radius: 50px; border: 3px solid grey;"}

![Accueil du site](https://raw.githubusercontent.com/Konsilion/website/master/media/fleche-retour.png){ .md-button .md-button--primary onclick="window.open('{{ katalog_site }}','_self');" style="float:right; height: 40px; padding: 5px; margin: 5px; border-radius: 50px; border: 3px solid grey;"}

# Panneau de configuration

---

Le **panneau de configuration** vous permet de gérer et de configurer votre site. Utiliser le panneau de configuration pour diverses tâches telles que la création de pages web, la gestion  du contenu existant, accéder aux espaces de stockages, etc. 

=== "Espaces de stockages"

    <p></p>
    ### Médiathèque

    La médiathèque permet la mise en ligne de ressources communes, universelles. Les ressources déposées ici ne sont pas assignables à un projet, ou à un individu en particulier.
    
    <div class="ksln-grid">
        <div class="ksln-cards">
            <h3><b>Consulter</b></h3>
            <img src="https://cdn-icons-png.flaticon.com/512/3603/3603249.png" style="margin: 5px; max-width: 75px; width: 100%; float: right; opacity:0.4;">
            <button class="md-button md-button--secondary" href="{{ katalog_repo }}/tree/master/media" target="_blank">Lien</button>
            <br>
            <br>
        </div>
        <div class="ksln-cards">
            <h3><b>Déposer un fichier</b></h3>
            <img src="https://cdn-icons-png.flaticon.com/512/9121/9121674.png" style="margin: 5px; max-width: 75px; width: 100%; float: right; opacity:0.4;">
            <button class="md-button md-button--secondary" href="{{ katalog_repo }}/upload/master/media" target="_blank">Lien</button>
            <br>
            <br>
        </div>
    </div>

    ### Klouds - Catalogue de vos stockages

    [Tout vos espaces de stockages]({{ katalog_site }}/katalog/klouds/home){ .md-button .md-button--primary style="float: right; margin: 10px;"}

    Les espaces de stockages Kloud regroupent les fichiers qui se rapportent à un thème commun (une personne, un projet, etc.). Vous pouvez télécharger un modèle de Kloud en bas de cette page ou bien référencer un espace de stockage existant.

    <div class="ksln-grid">
        <div class="ksln-cards">
            <h3><b>Créer un dépôt de fichiers</b></h3>
            Pour créer un espaces communs où regrouper vos fichiers par projets, utilisateurs, etc. Pour cela un simple compte GitHub suffit.
            <br><br>
            <button class="md-button md-button--secondary" onclick="window.open('https://github.com/Konsilion/kloud-template/generate');"> Créer un espace Kloud</button>
            <br>
            <br>
        </div>
        <div class="ksln-cards">
            <h3><b>En savoir plus</b></h3>
            Afin de mieux comprendre la logique proposées derrière les Klouds et l'organisation de vos ressources numériques.
            <br><br>
            <button class="md-button md-button--secondary" onclick="window.open('{{ katalog_site }}/admin/tutoriels/klouds/en-savoirs-plus','_self');">En savoir plus</button>
            <br>
            <br>
        </div>
    </div>

    si vous n'avez pas de compte GitHub, vous pouvez en créer un en <a href="https://github.com/signup" target="_blank">suivant ce lien</a>


=== "Pages Web"

    <div class="ksln-grid">
        <div class="ksln-cards">
            <h3><b>Créer une page</b></h3>
            De l'article de blog à une page contact, créer et diffuser le contenu Web que vous souhaitez, sans compétence particulière.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/pages/page-creer" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Modifier une page</b></h3>
            Modifier une page Web existante en toute simplicité.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/pages/page-modifier" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Commenter une page</b></h3>
            Donner la possibilité aux utilisateurs de commenter une page.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/pages/page-commenter" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Supprimer une page</b></h3>
            Supprimer ou de-référencer une page Web. 
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/pages/page-supprimer" target="_self">Lien</button>
        </div>
    </div>


=== "Catalogues Web"

    <div class="ksln-grid">
        <div class="ksln-cards">
            <h3><b>Créer un catalogue</b></h3>
            Présenter vos données, ressources et autres intérêts dans un catalogue Web (de multiples disposition existes, les découvrir).
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/katalogs/catalogue-creer" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Modifier un catalogue</b></h3>
            Modifier une catalogue Web existant en toute simplicité.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/katalogs/catalogue-modifier" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Lier un catalogue</b></h3>
            Afficher dans votre site des catalogues partenaires externes. Ainsi garder un oeil sur ce qu'il se fait autour de vous.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/katalogs/catalogue-lier" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Supprimer un catalogue</b></h3>
            Supprimer ou de-référencer un catalogue Web.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/katalogs/catalogue-supprimer" target="_self">Lien</button>
        </div>
    </div>

=== "Administration"

    <div class="ksln-grid">
        <div class="ksln-cards">
            <h3><b>Gérer les contributions</b></h3>
            Accedez à la liste des contributions en attente faites sur votre site.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/admin/admin-gerer" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Gérer les droits d'administration</b></h3>
            Définissez la modération par les droits d'accès, de lecture et d'écriture de votre plateforme.
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/admin/admin-droits" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Associer un nom de domaine</b></h3>
            Relier ce site web à l'un de vos domaines ou sous-domaines (ex: konsilion.fr).
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/admin/admin-domaine" target="_self">Lien</button>
        </div>
        <div class="ksln-cards">
            <h3><b>Paramétrer votre plateforme</b></h3>
            Enregistrer trois informations essentielles au bon fonctionnement de votre plateforme (fichier konsilion.json).
            <hr>
            <button class="md-button md-button--secondary" href="{{ katalog_site }}/admin/tutoriels/admin/admin-parametrer" target="_self">Lien</button>
        </div>          
    </div>

[Premiers pas ici ?]({{ katalog_site }}/admin/tutoriels/premiers-pas){ .md-button .md-button--primary style="float:right; margin: 10px;" target="_self"}  

---

<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/admin.js"></script>
<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/slider-nav.js" defer></script>
<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/add-page.js" defer></script>
<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js" defer></script>
