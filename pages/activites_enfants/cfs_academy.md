---
layout: page
title: cfs academy
banner: "/assets/images/banner/academy/academy.png"
image: "/assets/images/banner/academy/academy.png"
permalink: "/activites/cfs_academy/"
menu: true
description: Pour les plus aguerris du sport, le CFS vous propose une formule "CFS
  Academy" avec plusieurs avantages.

---
{% include annonces/activites.html %}

<a class="desktop btn btn-info-filled" href="https://www12.iclub.be/myiclub3_CFS_register.asp?ClubID=559&LG=FR&Categorie=6" target="_blank" style="float: right;">Inscription rapide</a>

<a class="mobile btn btn-block btn-info-filled" href="https://www12.iclub.be/myiclub3_CFS_register.asp?ClubID=559&LG=FR&Categorie=6" target="_blank" style="margin-bottom: 25px;">Inscription rapide</a>

<!-- NE PAS MODIFIER AU DESSUS DE CETTE LIGNE -->

Pour les plus aguerris, le CFS vous propose une formule  avec certains avantages.

Voici nos différentes disciplines:

<!-- NE PAS MODIFIER EN DESSOUS DE CETTE LIGNE -->
<!-- La liste des cours est modifiable dans le fichier _data/academy.yml -->

<div class="container">
    <div class="team-members-tow mtb-50">
      <div class="row">

        {% for cours in site.data.academy.cours %}
        {% if cours.online %}
        <div class="col-xs-6 col-md-3">
          {% include coleen/bulle.html src=cours.src titre=cours.titre href=cours.href bouton=cours.bouton %}
        </div>
        {% endif %}
        {% endfor %}

      </div>

    </div>
</div>