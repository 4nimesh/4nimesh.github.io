<h2 id="publications">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="abbr">
    <img src="{{ link.image }}" class="teaser" alt="Teaser preview">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  {% endif %}
  
  <div class="pub-content">
      <div class="title">
        {% if link.pdf %}
          <a href="{{ link.pdf }}" target="_blank" rel="noopener noreferrer">{{ link.title }}</a>
        {% else %}
          {{ link.title }}
        {% endif %}
      </div>
      
      <div class="author">{{ link.authors }}</div>
      
      {% if link.conference %}
      <div class="periodical"><em>{{ link.conference }}</em></div>
      {% endif %}
      
      <div class="links">
        {% if link.code %} 
        <a href="{{ link.code }}" class="btn btn-sm" role="button" target="_blank" rel="noopener noreferrer">Code</a>
        {% endif %}
        {% if link.page %} 
        <a href="{{ link.page }}" class="btn btn-sm" role="button" target="_blank" rel="noopener noreferrer">Project Page</a>
        {% endif %}
        {% if link.bibtex %} 
        <a href="{{ link.bibtex }}" class="btn btn-sm" role="button" target="_blank" rel="noopener noreferrer">BibTeX</a>
        {% endif %}
        {% if link.notes %} 
        <span class="pub-notes">{{ link.notes }}</span>
        {% endif %}
        {% if link.others %} 
        <span class="pub-others">{{ link.others }}</span>
        {% endif %}
      </div>
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>