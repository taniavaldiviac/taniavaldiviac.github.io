---
layout: archive
title: "Estudiantes"
permalink: /estudiantes/
author_profile: true
translation: /en/students/
---

Formación de recursos humanos en ADN ambiental, metabarcoding, ecología molecular y bioinformática.

{% for grupo in site.data.estudiantes %}
<h2>{{ grupo.grupo }}</h2>
<div class="estudiantes">
  {% for persona in grupo.personas %}{% include estudiante-card.html persona=persona %}{% endfor %}
</div>
{% endfor %}

¿Te interesa trabajar conmigo? Escríbeme a [tvaldivia@cibnor.mx](mailto:tvaldivia@cibnor.mx).
