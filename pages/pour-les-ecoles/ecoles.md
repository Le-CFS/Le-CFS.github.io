---
layout: page
title: Liste des partenaires
permalink: "/pour-les-ecoles/ecoles/"
menu: activites
description: ''

---

<!-- NE PAS MODIFIER AU DESSUS DE CETTE LIGNE -->

Voici la liste des activités parascolaires.

<!-- NE PAS MODIFIER EN DESSOUS DE CETTE LIGNE -->

<table class="table table-striped">
    <thead>
      <tr>
        <th scope="col">Établissement</th>
        <th scope="col">Garderies</th>
        <th scope="col">Journées pédagogiques</th>
        <th scope="col">Activités parascolaires</th>
      </tr>
    </thead>
    <tbody>

      {% for page in site.pages %}
            {% if page.type_page == "ecoles" %}
                {% if page.published == false %}
                {% else %}
                    <tr>
                        <td>{{ page.title }}</td>
                        <td><center>{% if page.activite_garderie %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
                        <td><center>{% if page.activite_parascolaire %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
                        <td><center>{% if page.activite_pedagogique %}<i class="fa fa-check-circle-o text-success fa-2x"></i>{% else %}<i class="fa fa-times-circle-o text-danger fa-2x"></i>{% endif %}</center></td>
                    </tr>
                {% endif %}
            {% endif %}
        {% endfor %}
    </tbody>
  </table>