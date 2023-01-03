---
title: Modification de page Web
hide:
   - toc
   - navigation
---

![Retour configuration](https://raw.githubusercontent.com/Konsilion/website/master/media/fleche-retour.png){ .md-button .md-button--primary onclick="window.history.back();" style="float:right; height: 40px; padding: 5px; margin: 5px; border-radius: 50px; border: 3px solid grey;"}

# Comment modifier une page Web existante ?

---


!!! tip ""

    Sur votre page en haut à droite de votre écran, retrouvé le bouton `Modifier la page` (non-disponible sur téléphone)

Afin de faciliter la contribution et les modifications autour de vos pages Web, pensez à ajouter la balise `script` suivante en bas de votre page: 

<div style="max-width: 650px; margin: 50px auto;" markdown>
    ``` html title="Page Web - Modèle de base"
    <script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js" defer></script>
    ```
</div>

En savoir plus sur les scripts proposés pour votre plateforme Web, <a href="{{ katalog_site }}/admin/tutoriels/pages/page-creer">c'est par ici</a>.

## Modification d'une page non balisée

Si vous souhaitez modifier une page ponctuellement, copier sont url à partir de `/pages/...` et ajouter avant le lien suivant : 

`{{ katalog_repo }}/edit/master/pages/...`



<script type="text/javascript" src="https://konsilion.github.io/katalog-setup/js/functionality/modif-page.js" defer></script> 
