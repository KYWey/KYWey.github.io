---
layout: page
title: "LA Food"
permalink: /fun/food/
---

<p><a href="{{ '/fun/' | relative_url }}">← Back to Fun Life</a></p>

# LA Food 🌆🍴

<p class="lead">My running map of great eating within about an hour's drive of UCLA — Westwood and
Sawtelle out to Torrance, Koreatown, Downtown, Pasadena, and the San Gabriel Valley. Part
reference list, part to-do list.</p>

<div class="callout">
  <p>📋 <strong>How this list works:</strong> everything here scores <strong>4.0★ or higher on both
  Google Maps and Yelp</strong>. Within each category, places are ranked by their Google rating.
  Scores and price levels ($–$$$$) are snapshots from <em>July 2026</em> and drift over time — the
  <strong>Maps / Yelp links on every card</strong> jump straight to the live listing so you can
  double-check before driving out.</p>
</div>

<h2 class="section-title">Jump to a craving</h2>

<ul class="chips">
{% for cat in site.data.food.categories %}
  <li><a class="chip" href="#{{ cat.id }}">{{ cat.icon }} {{ cat.title }}</a></li>
{% endfor %}
</ul>

{% for cat in site.data.food.categories %}
<h2 class="section-title" id="{{ cat.id }}">{{ cat.icon }} {{ cat.title }}</h2>
<p class="lead" style="font-size:1em">{{ cat.blurb }}</p>

{% if cat.entries and cat.entries.size > 0 %}
<div class="food-grid">
{% assign sorted = cat.entries | sort: "google" | reverse %}
{% for r in sorted %}
{% assign slug = r.name | slugify %}
  <div class="food-card">
    <div class="food-banner" style="background:linear-gradient(135deg,{{ cat.c1 }},{{ cat.c2 }})" title="Photo slot: Photos/Food/{{ slug }}.jpg">
      <span class="food-emoji" aria-hidden="true">{{ r.emoji }}</span>
      <img src="{{ '/Photos/Food/' | relative_url }}{{ slug }}.jpg" alt="{{ r.dish }} at {{ r.name }}" loading="lazy" onerror="this.remove()">
      <span class="food-rank">#{{ forloop.index }}</span>
    </div>
    <div class="food-body">
      <h3>{{ r.name }}</h3>
      <p class="food-dish">{{ r.emoji }} {{ r.dish }}</p>
      <div class="food-meta">
        <span class="chip">Google ★{{ r.google }}</span>
        <span class="chip">Yelp ★{{ r.yelp }}</span>
        <span class="chip">{{ r.price }}</span>
        <span class="chip">📍 {{ r.area }}</span>
        <span class="chip">{{ r.style }}</span>
      </div>
      {% if r.note %}<p class="food-note">💡 {{ r.note }}</p>{% endif %}
      <p class="food-links">
        <a href="https://www.google.com/maps/search/?api=1&query={{ r.name | append: ' ' | append: r.city | append: ' CA' | url_encode }}" target="_blank" rel="noopener">Google Maps ↗</a>
        <a href="https://www.yelp.com/search?find_desc={{ r.name | url_encode }}&find_loc={{ r.city | url_encode }}%2C%20CA" target="_blank" rel="noopener">Yelp ↗</a>
      </p>
    </div>
  </div>
{% endfor %}
</div>
{% else %}
<div class="callout">
  <p>🚧 Reserved for the true champions — restaurants get promoted here only after repeat visits.
  Watch this space.</p>
</div>
{% endif %}
{% endfor %}

<h2 class="section-title">Notes</h2>

<div class="callout">
  <p>🖼️ <strong>Photos:</strong> each card shows a food emoji until I drop a real photo into
  <code>Photos/Food/</code>. Hover over a card's banner to see the exact filename it expects
  (e.g. <code>pine-crane.jpg</code>) — add the file and it replaces the emoji automatically.</p>
  <p>🚗 <strong>"One hour from UCLA"</strong> is measured in the theoretical LA where the 405 is
  moving. Calibrate expectations (and departure times) accordingly.</p>
  <p>✍️ Adding a place is one small edit to <code>_data/food.yml</code> — the page sorts and
  numbers everything by itself.</p>
</div>
