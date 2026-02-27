<div class="publications" style="margin-top: 30px;">
  <h2 style="font-size: 1.2rem; font-weight: 700; margin-bottom: 20px;">Preprints & Under Review</h2>
  {% for item in site.data.works %}
    {% if item.type == 'publication' %}
      <div class="row" style="display: flex; gap: 20px; align-items: flex-start; margin-bottom: 30px;">
        <div class="col-sm-4"><img src="{{ item.img | relative_url }}" class="img-fluid rounded border"></div>
        <div class="col-sm-8">
          <h4 style="font-size: 1.05rem; font-weight: 600;">{{ item.title }}</h4>
          <p style="font-size: 0.9rem; margin-bottom: 5px;">{{ item.authors }}</p>
          <p style="font-size: 0.9rem; color: #666; font-style: italic;">{{ item.venue }}</p>
          <p style="font-size: 0.85rem; line-height: 1.4; color: #444;">{{ item.desc }}</p>
          <a href="{{ item.code }}" class="btn btn-outline-dark btn-sm mt-2">Code</a>
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>
