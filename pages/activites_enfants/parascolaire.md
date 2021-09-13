---
layout: page
title: parascolaire dans mon école
permalink: "/activites/parascolaire/"
menu: activites
description: ''

---
{% include annonces/activites.html %}

<div class="col-md-4" style="float: right; margin-bottom: 20px;">
	<a href="https://www12.iclub.be/myiclub3_CFS_register.asp?ClubID=559&LG=FR&Categorie=6" class="btn btn-block btn-info-filled" target="_blank">Inscription parascolaire</a>
</div>

<!-- NE PAS MODIFIER AU DESSUS DE CETTE LIGNE -->

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<!-- NE PAS MODIFIER EN DESSOUS DE CETTE LIGNE -->

#### Liste des activités

{% assign liste_activites = site.data.parascolaire.activites | sort: "name" %}

{% for activite in liste_activites %}

{% if activite.online %}

{% include coleen/carte_parascolaire.html %}

{% endif %}

{% endfor %}