---
layout: page
title: "Interesting Life Physics"
permalink: /fun/physics/
---

<p><a href="{{ '/fun/' | relative_url }}">← Back to Fun Life</a></p>

# Interesting Life Physics ☕🚲✈️

<p class="lead">Physics isn't just something that happens in the lab — it's in your bathroom sink,
your shampoo bottle, your bike ride, the sky above you, and even your fridge. Each box below is a
small "wait, why does that happen?" question with a quick answer. Click any one to open the full
explanation, complete with a schematic diagram (and, where it helps, the math).</p>

{%- assign problems = site.physics | sort: "order" -%}
{%- assign groups = problems | group_by: "category" -%}

<div class="toc-box">
  <strong>Browse by category</strong>
  <ol>
    {%- for g in groups -%}
    <li><a href="#{{ g.name | slugify }}">{{ g.name }}</a> <span class="toc-count">· {{ g.items | size }}</span></li>
    {%- endfor -%}
  </ol>
</div>

{% for g in groups %}
<h2 class="section-title" id="{{ g.name | slugify }}">{{ g.name }}</h2>
<div class="card-grid">
  {%- for p in g.items -%}
  <a class="card" href="{{ p.url | relative_url }}">
    <span class="card-icon">{{ p.icon }}</span>
    <h3>{{ p.title }}</h3>
    <div class="verdict">
      {%- if p.myth and p.real -%}
      <p><span class="tag-no">Why not</span> {{ p.myth }}</p>
      <p><span class="tag-yes">Why yes</span> {{ p.real }}</p>
      {%- elsif p.summary -%}
      <p><span class="tag-yes">Short answer</span> {{ p.summary }}</p>
      {%- endif -%}
    </div>
    <span class="card-more">Full explanation →</span>
  </a>
  {%- endfor -%}
</div>
{% endfor %}

<h2 class="section-title">Gallery</h2>

{% include gallery.html folder="/Photos/life-physics" %}

<div class="callout">
  <p>💬 Have an everyday mystery you'd like me to tackle?
  <a href="mailto:wesleywey0717@g.ucla.edu">Send it my way</a> and it might become the next entry.
  Any photos I add to <code>Photos/life-physics/</code> will show up above automatically.</p>
</div>
