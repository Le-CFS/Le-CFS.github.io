---
layout: page
title: Pour les écoles
banner: "/assets/images/cfs_ecoles_activites_950px400px.jpg"
image: "/assets/images/cfs_ecoles_activites_950px400px.jpg"
permalink: "/pour-les-ecoles/"
menu: true
description: Pour les écoles
lieux:
- bierges
- ottignies
- liernu
type_page: ''
activite_garderie: false
activite_parascolaire: false
activite_pedagogique: false
activite_stage: false
bulle: ''

---
#### **Un cadre convivial pour vos enfants !**

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
            <td><center>{% if page.activite_parascolaire %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
            <td><center>{% if page.activite_garderie %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
            <td><center>{% if page.activite_pedagogique %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
            <td><center>{% if page.activite_stage %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
        </tr>
    </tbody>
</table>

## Nos écoles partenaires

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