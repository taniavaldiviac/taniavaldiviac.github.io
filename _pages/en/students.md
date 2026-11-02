---
layout: archive
title: "Students"
permalink: /en/students/
author_profile: true
lang: en
translation: /estudiantes/
---

Training the next generation in environmental DNA, metabarcoding, molecular ecology and bioinformatics.

{% for grupo in site.data.estudiantes %}
<h2>{{ grupo.grupo_en | default: grupo.grupo }}</h2>
<div class="estudiantes">
  {% for persona in grupo.personas %}{% include estudiante-card.html persona=persona %}{% endfor %}
</div>
{% endfor %}

Interested in working with me? Write to [tvaldivia@cibnor.mx](mailto:tvaldivia@cibnor.mx).
