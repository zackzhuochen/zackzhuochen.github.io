<h2 id="publications" style="margin: 2px 0px -15px;">Fieldwork</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.fieldwork.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.location %} 
    <abbr class="badge">{{ link.location }}</abbr>
    {% endif %}
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="author">{{ link.note }}</div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>
