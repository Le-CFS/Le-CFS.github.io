---
layout: page
title: Ecole de natation
banner: "/assets/images/banner/activites_et_infos/ecoledenatation.png"
image: "/assets/images/banner/activites_et_infos/ecoledenatation.png"
permalink: "/activites/ecole_de_natation/"
menu: true
description: ''

---
{% include annonces/activites.html %}

{% include annonces/natation.html %}

{% assign natation = site.data.ecole_de_natation %}

{% for province in natation.provinces %}
{% if province.online %}
<div class="container">
    <div class="team-members-tow mtb-50">
      <div class="d-flex justify-content-between align-items-center">
        <div class="sub-title">
          <span>{{ province.nom }}</span>
        </div>
        <div>
          <a href="https://www12.iclub.be/myiclub3_CFS_register.asp?ClubID=559&LG=FR&Categorie=5" class="btn btn-info-filled">J'inscris mon petit nageur</a>
        </div>
      </div>
        <div class="row">

          {% for cours in province.cours %}
          {% if cours.online %}
          <div class="col-xs-6 col-md-3">
            {% include coleen/bulle.html src=cours.src titre=cours.titre href=cours.href bouton=cours.bouton %}
          </div>
          {% endif %}
          {% endfor %}

        </div>

    </div>
</div>
{% endif %}
{% endfor %}