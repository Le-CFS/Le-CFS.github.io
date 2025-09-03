---
layout: page
title: Les centres CFS
permalink: "/cfs/les_centres_cfs/"
menu: true
description: Nos différents centres CFS situés à Bruxelles, Liège et dans le Brabant
  wallon sont prêt à vous accueillir lors des activités et des stages.
image: ''
intro: Vous trouverez certainement un centre <strong>CFS</strong> proche de chez vous.
provinces:
- name: Bruxelles
  banner: "/assets/images/bxl-banner.jpg"
  image_annee: "/assets/images/BXL-a-l-annee.png"
  image_stages: "/assets/images/BXL-stages.png"
  url_annee: ''
  url_stages: ''
- name: Brabant
  banner: "/assets/images/brt-banner.jpg"
  image_annee: "/assets/images/BRT-a-l-annee.png"
  image_stages: "/assets/images/BRT-stages.png"
  url_annee: ''
  url_stages: ''
- name: Liege
  banner: "/assets/images/lie-banner.jpg"
  image_annee: "/assets/new-images/durant l annee - liege.png"
  image_stages: "/assets/new-images/durant les stages - liege.png"
  url_annee: ''
  url_stages: ''

---
<center><span style="color:#2980b9; font-size:20px">{{ page.intro }}</span></center>

<div class="desktop mb-60"></div>

{% for province in page.provinces %}

<img alt="" src="{{ province.banner }}" style="width:100%" />

{% if province.image_annee != "" %}
<a href="{{ province.url_annee }}" target="_blank"><img alt="" src="{{ province.image_annee }}" style="width:100%" /></a>
{% endif %}

{% if province.image_stages != "" %}
<a href="{{ province.url_stages }}" target="_blank"><img alt="" src="{{ province.image_stages }}" style="width:100%" /></a>
{% endif %}

{% endfor %}
