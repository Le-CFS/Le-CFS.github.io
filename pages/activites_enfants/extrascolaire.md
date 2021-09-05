---
layout: page
title: Extrascolaire pour tous
permalink: /activites/extrascolaire/
menu: activites
js: portfolio.js
---
{% include annonces/activites.html %}

<div class="col-md-4" style="float: right; margin-bottom: 20px;">
	<a href="https://www12.iclub.be/myiclub3_CFS_register.asp?ClubID=559&LG=FR&Categorie=6" class="btn btn-block btn-info-filled" target="_blank">Inscription extrascolaire</a>
</div>

<!-- NE PAS MODIFIER AU DESSUS DE CETTE LIGNE -->

Le CFS propose des activités sportives ou culturelles qui débutent au mois de septembre et se déroulent tout au long de l’année scolaire jusqu’à la fin du mois de mai.

Chaque enfant a le droit à une séance d’essai avant de s’engager de manière définitive.

On peut s’inscrire en cours d’année en fonction des places disponibles (le prix est alors calculé au prorata des séances restantes) et des activités.

Nous appliquons pour nos activités [le protocole général des stages](/stages/protocole/general/) qui a fait ses preuves cet été.

<!-- NE PAS MODIFIER EN DESSOUS DE CETTE LIGNE -->

<div id="content">
    <section id="portfolio" class="section">
         <div class="row">
            <div class="col-md-12">
              	<div class="controls text-center wow fadeInUpQuick" data-wow-delay=".6s">
	                <a class="filter active btn-stage btn-stage-all btn btn-common col-md-12 btn-block" data-filter="all">
	                  Toutes les activités
	                </a>
	                <a class="filter btn-stage btn-stage-bouts btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".bouts">
	                  Les Petits Bouts 
	                </a>
	                <a class="filter btn-stage btn-stage-culturelles btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".culturelles">
	                  Sportives & Culturelles
	                </a>
	                <a class="filter btn-stage btn-stage-danse btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".danse">
	                  Danse & Gymnastique
	                </a>
	                <a class="filter btn-stage btn-stage-fun btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".fun">
	                  Activités Fun 
	                </a>
	                <a class="filter btn-stage btn-stage-sportives btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".sportives">
	                  Activités Sportives 
	                </a>
	                <a class="filter btn-stage btn-stage-artistiques btn btn-common col-md-6 col-lg-4 col-xl-3" data-filter=".artistiques">
	                  Artistique & Loisirs
	                </a>
              	</div>
            </div>
            
            <div id="portfolio" class="row wow fadeInUpQuick" data-wow-delay="0.8s">

							{% assign liste_stages = site.data.extrascolaire.activites | sort: "name" %}
								
								{% for stage in liste_stages %}
								  {% if stage.online %}

										{% include coleen/carte_extrascolaire.html %}

								  {% endif %}
								{% endfor %}

        	</div>
        </div>
	</section>
</div>