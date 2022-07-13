---
layout: page
title: Court-Saint-Etienne - Sart-Messire-Guillaume
banner: "/assets/images/banner/events/journeesportives.png"
image: "/assets/images/banner/events/journeesportives.png"
permalink: "/pour-les-ecoles/ecoles/sart-messire-guillaume/"
menu: true
description: Ecole de Sart-Messire-GUillaume
type_page: ecoles
activite_garderie: false
activite_parascolaire: true
activite_pedagogique: true
bulle: ''
button_document_text: Voir le programme
button_document_color: 
button_document_link: #
published: false

---

<table class="table table-striped mt-4 mb-4">
  <thead>
    <tr>
      <th scope="col" style="width:33%"><center>Garderies</center></th>
      <th scope="col" style="width:33%"><center>Journées pédagogiques</center></th>
      <th scope="col" style="width:33%"><center>Activités parascolaires</center></th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td><center>{% if page.activite_garderie %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
        <td><center>{% if page.activite_parascolaire %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
        <td><center>{% if page.activite_pedagogique %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
    </tr>
  </tbody>
</table>

<div class="d-flex justify-content-center mb-3">
	<a href="{{ page.button_document_link}}" class="btn btn-info-filled" target="_blank">{{  page.button_document_text }}</a>
</div>

Coucou l'école !