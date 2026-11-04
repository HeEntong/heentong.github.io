<h2 id="publications" class="publications-heading">Selected publications and preprints</h2>

<div class="publications">
<ol class="bibliography">

{% for publication in site.data.publications.main %}

<li class="publication-item">
  <div class="publication-title">
    {% if publication.link %}
    <a href="{{ publication.link }}">{{ publication.title }}</a>
    {% else %}
    {{ publication.title }}
    {% endif %}
  </div>
  {% if publication.authors %}
  <div class="publication-authors">{{ publication.authors }}{% if publication.alphabetical_authors %} <small class="publication-author-note">(alphabetical order)</small>{% endif %}</div>
  {% endif %}
  {% if publication.conference %}
  <div class="publication-venue">{{ publication.conference }}</div>
  {% endif %}
</li>

{% endfor %}

</ol>
</div>
