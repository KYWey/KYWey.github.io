---
layout: page
title: "Research"
permalink: /research/
---

# My Research, in Plain Language

<p class="lead">I study <strong>quantum materials</strong> — crystals whose electrons organize
themselves in strange, collective ways. To do that, I use two of the most powerful "cameras"
in condensed-matter physics. Here's what they are and what I'm looking for.</p>

{%- assign hero = site.static_files | where_exp: "f", "f.path contains '/Photos/research/research_page.'" | first -%}
{% if hero %}
<figure class="page-photo">
  <img src="{{ hero.path | relative_url }}" alt="Kuan-Yu Wey next to the low-temperature STM at UCLA">
  <figcaption>In the lab at UCLA, next to our low-temperature STM.</figcaption>
</figure>
{% endif %}

<h2 class="section-title">The two instruments I use</h2>

<div class="feature">
  <h3><span class="tag">STM</span> Scanning Tunneling Microscopy</h3>
  <p>Imagine a needle so sharp it ends in a <em>single atom</em>. We bring that tip within a
  billionth of a metre of a surface — close enough that electrons "tunnel" across the gap, a purely
  quantum-mechanical jump. By measuring that tiny current as the tip scans back and forth, we build
  up a map of the surface <strong>one atom at a time</strong>. STM doesn't just show where atoms are;
  by tuning the voltage, it also reveals the <em>energy landscape</em> the electrons live in
  (this mode is called scanning tunneling spectroscopy, or STS).</p>
</div>

{%- comment -%} Hand-arranged: three columns at one shared height (see .stm-row in custom.css). {%- endcomment -%}
<div class="stm-row">
  <figure class="stm-sputter">
    <img src="{{ '/Photos/research/stm/Gold_Sputter.JPG' | relative_url }}" alt="Ar⁺ sputtering of a gold crystal" loading="lazy">
    <figcaption>{{ site.data.captions["Gold_Sputter.JPG"] }}</figcaption>
  </figure>
  <figure class="stm-gold">
    <img src="{{ '/Photos/research/stm/Gold_STM_image.png' | relative_url }}" alt="Atomic-resolution STM image of Au(111)" loading="lazy">
    <figcaption>{{ site.data.captions["Gold_STM_image.png"] }}</figcaption>
  </figure>
  <figure class="stm-stack">
    <img src="{{ '/Photos/research/stm/STM_Optical_Access.png' | relative_url }}" alt="Optical view of the STM tip on a blue bronze crystal" loading="lazy">
    <img src="{{ '/Photos/research/stm/BlueBronze_Topo_CDW1_Phase.png' | relative_url }}" alt="STM topography, charge density wave wavefronts, and phase map of blue bronze" loading="lazy">
    <figcaption>{{ site.data.captions["STM_Optical_Access.png"] }}</figcaption>
  </figure>
</div>

<div class="feature">
  <h3><span class="tag">ARPES</span> Angle-Resolved Photoemission Spectroscopy</h3>
  <p>Here we shine light on the material and knock electrons out of it (the photoelectric effect
  that Einstein won his Nobel Prize for). By carefully measuring each escaping electron's
  <strong>energy</strong> and the <strong>angle</strong> it flew off at, we can reconstruct the
  "rules of the road" that electrons obey inside the crystal — its <em>band structure</em>. If STM
  is a photograph in <strong>real space</strong> (where the atoms are), ARPES is the complementary
  photograph in <strong>momentum space</strong> (how the electrons move).</p>
</div>

{% include gallery.html folder="/Photos/research/arpes" layout="row" %}

<div class="callout">
  <p><strong>Why use both?</strong> A single technique only tells half the story. STM shows the
  atomic-scale texture; ARPES shows the global electronic behavior. Put them together and you get a
  complete picture of a material — which is exactly what my work tries to do.</p>
</div>

<h2 class="section-title">Seeing it come together</h2>

<p>The animation below unifies both viewpoints — the real-space, atom-by-atom STM picture and the
momentum-space ARPES picture — into a single story of how the charge density wave and its electronic
bands are connected.</p>

<div class="video-wrap">
  <video controls preload="metadata" playsinline>
    <source src="{{ '/stm_arpes_unified.mp4' | relative_url }}" type="video/mp4">
    Your browser can't play embedded video —
    <a href="{{ '/stm_arpes_unified.mp4' | relative_url }}">download the clip here</a>.
  </video>
</div>
<p class="video-caption">STM &amp; ARPES, unified: real-space atomic structure alongside the
electronic band structure of the material I study.</p>

<div class="callout">
  <p>I keep a running list of review papers on STM and ARPES (with my own, admittedly still-growing,
  notes and intuitions). If you'd like recommendations to dig deeper, feel free to
  <a href="mailto:wesleywey0717@g.ucla.edu">reach out</a> — I'm always happy to chat.</p>
</div>

<h2 class="section-title">What I'm working on</h2>

<p>My thesis is about imaging — and controlling — <strong>charge density waves (CDWs)</strong>. In
some materials the electrons spontaneously arrange themselves into a repeating ripple pattern, a
kind of self-organized electronic traffic jam. In a <strong>quasi-one-dimensional</strong> material
that ripple prefers to run along a single direction, like grooves on a record. Two projects make up
most of the thesis.</p>

<div class="project">
  <div markdown="1">
### Driving a charge density wave with a current

I run a controlled electrical current straight through the sample and use STM to watch, atom by
atom, how the electronic order **shifts, slides, and responds** — while ARPES tells me how the
underlying electronic bands are set up. The goal is to understand how you might *tune* and
*control* these quantum states, not just observe them. In more technical words: probing the
atomic-scale dynamics of a quasi-1D charge density wave by in-plane, current-tuned scanning
tunneling microscopy and spectroscopy (STM/STS).
  </div>
  <figure>
    <img src="{{ '/Photos/research/overview/STM25_PresentPhoto.JPG' | relative_url }}" alt="Talk at the IBS Conference on STM '25" loading="lazy">
    <figcaption>{{ site.data.captions["STM25_PresentPhoto.JPG"] }}</figcaption>
  </figure>
</div>

<div class="project">
  <div markdown="1">
### Short-range order of alkali ions on a charge density wave surface

The surface of a CDW material is not just the wave. Alkali ions sitting on it — left there when
the crystal is cleaved, or deposited afterwards — don't line up into a perfect lattice, yet they
aren't random either: each ion keeps a regular arrangement with its neighbours that fades out over
longer distances. That is **short-range order**. I deposit alkali atoms *in situ* and map how they
arrange using STM and qPlus AFM at the same time, to learn how the ions and the charge density
wave underneath influence each other.
  </div>
  <figure>
    <img src="{{ '/Photos/research/overview/2024_MarchMeeting.JPG' | relative_url }}" alt="Talk at the 2024 APS March Meeting" loading="lazy">
    <figcaption>{{ site.data.captions["2024_MarchMeeting.JPG"] }}</figcaption>
  </figure>
</div>

<h2 class="section-title">Current work</h2>

<p>Alongside the two projects above, these are the tools I've been building recently.</p>

<h3 class="subsection-title">1. Home-built qPlus AFM sensors</h3>

<p>An STM only senses electrical current, so it needs a conducting surface. A <strong>qPlus
sensor</strong> adds a sense of touch: the tip sits on one prong of a tiny quartz tuning fork — the
same kind that keeps time in a wristwatch — and as the tip comes within atomic distances of the
surface, the forces between them shift the fork's ringing frequency ever so slightly. Tracking that
shift gives an atomic force microscope (AFM) image, recorded at the same time as the STM image.</p>

<p>I build these sensors in-house from commercial tuning forks, as a low-cost alternative to
commercial ones, and use them to study how alkali atoms deposited on a charge density wave surface
arrange themselves.</p>

{% include gallery.html folder="/Photos/research/qPlus" layout="row" %}

<h3 class="subsection-title">2. Deposition gun</h3>

<p>To put atoms onto a surface on purpose, I added a deposition source — a "gun" — to the
microscope's preparation chamber. Passing a current through the source releases a gentle,
controllable stream of alkali atoms (potassium, here) onto a clean sample, without ever breaking
vacuum. It is what makes the short-range-order experiments above possible.</p>

{% include gallery.html folder="/Photos/research/Deposition_Gun" layout="row" width="32em" %}

<h3 class="subsection-title">3. Autonomous SPM</h3>

<p>A scanning probe microscope spends much of its time on chores: reshaping a tip that has gone
blunt, and hunting for a clean, flat area worth measuring. We are building our own routines so
the instrument can calibrate its tip and run experiments on its own. A fuller write-up will come;
for now, these are the references we build on:</p>

<ul class="ref-list">
  <li><a href="https://github.com/abred/DeepSPM" target="_blank" rel="noopener">DeepSPM</a> —
  artificial-intelligence-driven scanning probe microscopy.</li>
  <li><a href="https://pubs.acs.org/jpcafh/article/125/6/1384/503219/Automated-Tip-Conditioning-for-Scanning-Tunneling" target="_blank" rel="noopener">Automated
  Tip Conditioning for Scanning Tunneling Spectroscopy</a>, <em>J. Phys. Chem. A</em>
  <strong>125</strong>, 1384 (2021).</li>
  <li><a href="https://claude.com/claude-code" target="_blank" rel="noopener">Claude Code</a> —
  AI-assisted development, used to build and maintain the control software.</li>
</ul>

<h2 class="section-title">Explore more</h2>

<div class="card-grid">
  <a class="card" href="{{ '/research/lab/' | relative_url }}">
    <h3>Inside the Lab</h3>
    <p>The hands-on engineering behind the images — ultra-high vacuum, cooling to 4 kelvin, and the
    everyday craft of keeping an STM &amp; ARPES experiment running.</p>
    <span class="card-more">Go behind the scenes →</span>
  </a>
  <a class="card" href="{{ '/research/related/' | relative_url }}">
    <h3>Related Topics</h3>
    <p>Other corners of condensed matter I find fascinating — different instruments and quantum
    platforms like semiconductor and superconducting qubits.</p>
    <span class="card-more">Dive in →</span>
  </a>
</div>
