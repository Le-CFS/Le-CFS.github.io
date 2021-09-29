---
layout: page
title: Anniversaires
banner: "/assets/images/banner/anniversaires/anniversaires.png"
image: "/assets/images/banner/anniversaires/anniversaires.png"
permalink: "/anniversaires/"
menu: true
description: Viens fêter ton anniversaire à Bierges, Ottignies, Wavre, Auderghem ou
  Woluwé pour vivre un moment inoubliable avec tes amis et les moniteurs du CFS !
js: portfolio.js
---

{% include annonces/anniversaires.html %}

<div class="row">
  <div class="col-md-4 offset-md-4">
    <a href="/anniversaires/reservation/" class="btn btn-block btn-info-filled" style="margin-top: -5px;">RÉSERVATION</a>
  </div>
</div>

<div style="padding-top: 25px;"></div>

<div class="col-md-12 text-center" style="font-size: 24px;"><b>Nouveau à Louvain-la-Neuve</b></div>

<div style="padding-top: 12px;"></div>
{% comment%}
Modifier la largeur, la hauteur et le lien en fonction des besoins.
width = largeur
height = hauteur
src = lien
{% endcomment %}

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/n-gbscvwkGA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>


<!-- NE PAS MODIFIER EN DESSOUS DE CETTE LIGNE -->
<div id="content">
<section id="portfolio" class="section">
         <div class="row" style="display:inline;">
            <div class="col-md-12">
                <div class="controls text-center wow fadeInUpQuick" data-wow-delay=".6s">
                  <a class="filter active btn-stage btn-stage-all btn btn-common col-md-12 btn-block" data-filter="all">
                    Tous les anniversaires
                  </a>
                  <a class="filter btn-stage btn-stage-bouts btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".domicile">
                    À mon domicile
                  </a>
                  <a class="filter btn-stage btn-stage-culturelles btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".fun">
                    Sportif et Fun
                  </a>
                </div>
            </div>

            <div id="portfolio" class="row wow fadeInUpQuick" data-wow-delay="0.8s">
        {% assign anniversaires = site.data.anniversaires.anniversaires | sort: "name" %}
        
        {% for anniversaire in anniversaires %}
            {% if anniversaire.online %}

            {% include coleen/cartes_anniversaires.html %}

            {% endif %}
        {% endfor %}

          </div>
        </div>
  </section>
</div>

<!-- Boutons de fin -->
<div class="row">
  <div class="col-md-6">
    <a href="/anniversaires/reservation/" class="btn btn-block btn-info-filled" style="margin-top: 15px;">RÉSERVATION</a>
  </div>
  <div class="col-md-6">
    <a href="{{ page.url }}en_savoir_plus" class="btn btn-block btn-info-filled" style="margin-top: 15px;">EN SAVOIR PLUS</a>
  </div>
</div>
<!-- Fin des boutons de fin -->

<div class="row" style="margin-top: 45px;">
  <div class="col-md-4 offset-md-4">
    <img src="https://www12.iclub.be/images/upload/559/ballons_annif.jpg" style="width: 100%; height: auto;">
  </div>
</div>