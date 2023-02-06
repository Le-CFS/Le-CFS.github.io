---
layout: page
title: Pour les écoles
banner: "/assets/images/slider-sart-messire-guillaume.jpg"
image: "/assets/images/banner-sart-messire-guillaume.jpg"
permalink: "/pour-les-ecoles/"
menu: true
description: Pour les écoles

---
#### **Un cadre convivial pour vos enfants !**

Voici tous les services proposés par le CFS dans les écoles :

<table class="table table-striped mt-4 mb-4">
    <thead>
        <tr>
        <th scope="col" style="width:25%"><center>Activités parascolaires</center></th>
        <th scope="col" style="width:25%"><center>Garderies</center></th>
        <th scope="col" style="width:25%"><center>Journées pédagogiques</center></th>
        <th scope="col" style="width:25%"><center>Stages</center></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><center><i class="fa fa-check-circle-o text-success fa-2x"></i></center></td>
            <td><center><i class="fa fa-check-circle-o text-success fa-2x"></i></center></td>
            <td><center><i class="fa fa-check-circle-o text-success fa-2x"></i></center></td>
            <td><center><i class="fa fa-check-circle-o text-success fa-2x"></i></center></td>
        </tr>
    </tbody>
</table>

### Nos écoles partenaires

<div class="container">
	<div class="team-members-tow mtb-50">
		<div class="row">
		{% for partenaire in site.data.partenaires.liste %}
            {% if partenaire.online and partenaire.categorie contains 'écoles' %}
                <div class="col-sm-6 col-md-4">
                    <img src="{{ partenaire.logo }}" alt="" style="border-radius: 5%;">
                </div>
            {% endif %}
		{% endfor %}
		</div>
	</div>
</div>