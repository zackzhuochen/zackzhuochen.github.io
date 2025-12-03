<h2 id="fieldwork" style="margin: 2px 0px -15px;">Field Research</h2>

<div class="fieldwork">
  <ol class="introduction">

    {% for link in site.data.fieldwork.main %}

    <li>
      .fieldwork .pub-row {margin-top: 0 !important;}

        <!-- 图片列 -->
        <div class="col-sm-3 abbr" style="padding-right: 15px; padding-left: 15px;">
          {% if link.image %}
          <img src="{{ link.image }}" 
               class="teaser img-fluid z-depth-1" 
               style="width: 100%; height: 40%; display: block; border-radius: 6px;">
          {% endif %}
        </div>

        <!-- 文字列 -->
        <div class="col-sm-9" style="padding-left: 20px; padding-right: 15px;">
          <div class="author">{{ link.note }}</div>
        </div>

      </div>
    </li>

    {% endfor %}

  </ol>
</div>

