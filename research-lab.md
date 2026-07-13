---
layout: page
title: "Inside the Lab"
permalink: /research/lab/
---

<p><a href="{{ '/research/' | relative_url }}">← Back to Research</a></p>

# Inside the Lab 🛠️ <span class="wip">Growing</span>

<p class="lead">The pretty atomic-resolution images are only half the job. The other half is the
quiet, stubborn engineering that keeps the experiment alive: pulling a vacuum emptier than outer
space, cooling the microscope to a few degrees above absolute zero, keeping samples and tips
pristine, and getting a rack of noisy electronics to agree with one another. Here's a look behind
the curtain at what running an STM &amp; ARPES lab actually involves.</p>

{%- assign topics = site.lab | sort: "order" -%}
{%- assign live = topics | where_exp: "t", "t.status != 'planned'" -%}
{%- assign planned = topics | where_exp: "t", "t.status == 'planned'" -%}

<h2 class="section-title">How we keep the experiment running</h2>

<div class="card-grid">
  {%- for t in live -%}
  <a class="card" href="{{ t.url | relative_url }}">
    <span class="card-icon">{{ t.icon }}</span>
    <h3>{{ t.title }}</h3>
    <div class="verdict">
      {%- if t.summary -%}
      <p><span class="tag-yes">The short version</span> {{ t.summary }}</p>
      {%- endif -%}
    </div>
    <span class="card-more">Take a look →</span>
  </a>
  {%- endfor -%}
</div>

{% if planned.size > 0 %}
<h2 class="section-title">On the way</h2>

<p class="lead">Write-ups I'm still putting together — the day-to-day craft that makes or breaks a
measurement.</p>

<div class="card-grid">
  {%- for t in planned -%}
  <div class="card">
    <span class="card-icon">{{ t.icon }}</span>
    <h3>{{ t.title }} <span class="wip">Soon</span></h3>
    <p>{{ t.summary }}</p>
  </div>
  {%- endfor -%}
</div>
{% endif %}

<div class="callout">
  <p>🚧 This section grows over time. Want to hear about a particular part of the lab first?
  <a href="mailto:wesleywey0717@g.ucla.edu">Let me know</a> and I'll move it up the queue.</p>
</div>
