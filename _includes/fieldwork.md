<h2 id="fieldwork" style="margin: 2px 0px -15px;">Field Research</h2>

<div class="fieldwork">
<ol class="introduction">

{% for link in site.data.fieldwork.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="author">{{ link.authors }}</div>      
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>
