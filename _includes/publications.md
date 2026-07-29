<h2 id="publications" class="publications-heading">Publications and preprints</h2>

<div class="publications">
<ol class="bibliography">

{% for publication in site.data.publications.main %}

<li class="publication-item">
  <div class="publication-title">
    {% if publication.pdf %}
    <a href="{{ publication.pdf }}">{{ publication.title }}</a>
    {% else %}
    {{ publication.title }}
    {% endif %}
  </div>
  {% if publication.authors %}
  <div class="publication-authors">{{ publication.authors }}</div>
  {% endif %}
  {% if publication.conference %}
  <div class="publication-venue">{{ publication.conference }}</div>
  {% endif %}
</li>

{% endfor %}

</ol>
</div>
