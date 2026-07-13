---
title: "Ultra-high vacuum: emptier than outer space"
category: "Keeping the experiment alive"
icon: "🌌"
order: 1
status: published
summary: "To image single atoms we first remove almost every stray gas molecule around the sample — reaching a pressure a hundred-billion times thinner than air, so the surface stays atomically clean for hours instead of nanoseconds."
---

<p>When you want to photograph <em>individual atoms</em> on a surface, your worst enemy is ordinary
air. At normal atmospheric pressure a freshly prepared surface is bombarded so violently by gas
molecules that it gets completely coated in less than a <strong>billionth of a second</strong>.
Whatever you were trying to study is instantly buried under a grime of oxygen, water, and nitrogen.
The only way out is to take the air away — almost all of it.</p>

<p>Our microscopes live inside <strong>ultra-high vacuum (UHV)</strong>, at pressures around
10⁻¹⁰&nbsp;Torr. That's roughly a <strong>hundred-billion times</strong> thinner than the air in the
room, and actually better than the vacuum in low Earth orbit. Two numbers explain why we go to such
extremes:</p>

<ul class="chips">
  <li class="chip">🧭 Mean free path: <strong>hundreds of km</strong></li>
  <li class="chip">🧼 Clean-surface lifetime: <strong>hours, not nanoseconds</strong></li>
</ul>

<p>In UHV a gas molecule travels hundreds of kilometres before it hits another one, and only a
trickle of them ever reach the sample. A surface that would be ruined in a nanosecond at atmosphere
now stays pristine for hours — long enough to find an interesting spot and map it atom by atom.</p>

<figure class="diagram">
  <svg viewBox="0 0 600 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="At atmospheric pressure a surface is instantly covered by gas; in ultra-high vacuum it stays clean for hours">
    <!-- left panel: atmosphere -->
    <text x="150" y="24" font-size="13" text-anchor="middle" font-weight="700" fill="currentColor">At 1 atm</text>
    <line x1="30" y1="150" x2="270" y2="150" stroke="currentColor" stroke-width="2"/>
    <text x="150" y="170" font-size="10" text-anchor="middle" fill="currentColor">sample surface</text>
    <!-- dense bombardment -->
    <g stroke="#c0392b" stroke-width="1.6">
      <line x1="55" y1="55" x2="70" y2="140" marker-end="url(#uhvred)"/>
      <line x1="95" y1="45" x2="105" y2="140" marker-end="url(#uhvred)"/>
      <line x1="135" y1="55" x2="140" y2="140" marker-end="url(#uhvred)"/>
      <line x1="175" y1="45" x2="170" y2="140" marker-end="url(#uhvred)"/>
      <line x1="215" y1="55" x2="205" y2="140" marker-end="url(#uhvred)"/>
      <line x1="245" y1="60" x2="235" y2="140" marker-end="url(#uhvred)"/>
    </g>
    <text x="150" y="195" font-size="11" text-anchor="middle" font-weight="700" fill="#c0392b">buried in ~1 nanosecond</text>
    <!-- right panel: UHV -->
    <text x="450" y="24" font-size="13" text-anchor="middle" font-weight="700" fill="currentColor">At 10⁻¹⁰ Torr (UHV)</text>
    <line x1="330" y1="150" x2="570" y2="150" stroke="currentColor" stroke-width="2"/>
    <text x="450" y="170" font-size="10" text-anchor="middle" fill="currentColor">sample surface</text>
    <line x1="470" y1="50" x2="455" y2="140" stroke="#2774AE" stroke-width="1.8" marker-end="url(#uhvblue)"/>
    <text x="450" y="195" font-size="11" text-anchor="middle" font-weight="700" fill="#2774AE">stays clean for hours</text>
    <defs>
      <marker id="uhvred" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c0392b"/></marker>
      <marker id="uhvblue" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#2774AE"/></marker>
    </defs>
  </svg>
  <figcaption>The same surface, two worlds apart: in air, a storm of molecules coats it instantly;
  in UHV, only the occasional straggler arrives, so the surface stays clean long enough to study.</figcaption>
</figure>

<h2 class="section-title">How we get there</h2>

<p>You can't reach UHV with a single pump — it takes a relay team, each stage handing off to the
next as the chamber gets emptier:</p>

<div class="feature">
  <h3><span class="tag">1</span> Rough &amp; turbo pumps</h3>
  <p>A scroll or rotary pump first drops the chamber from atmosphere down to a modest vacuum. Then a
  <strong>turbomolecular pump</strong> — a turbine spinning tens of thousands of times a minute —
  literally bats stray molecules out of the chamber, taking us into the 10⁻⁸&nbsp;Torr range.</p>
</div>

<div class="feature">
  <h3><span class="tag">2</span> The bakeout</h3>
  <p>The real enemy is water clinging to the inside walls. So we wrap the whole chamber in heaters
  and foil and <strong>bake it at ~120&nbsp;°C for several days</strong>, gently boiling that water
  off the metal so the pumps can carry it away. Skipping this step is the difference between good
  vacuum and <em>great</em> vacuum.</p>
</div>

<div class="feature">
  <h3><span class="tag">3</span> Ion &amp; sublimation pumps</h3>
  <p>For the final stretch we switch to pumps with no moving parts (and therefore no vibration, which
  the microscope hates). An <strong>ion pump</strong> ionizes the last remaining gas and buries it in
  a metal electrode, while a <strong>titanium sublimation pump</strong> flashes a fresh, chemically
  hungry titanium film that grabs stray molecules like flypaper. Together they hold us at
  ~10⁻¹⁰–10⁻¹¹&nbsp;Torr indefinitely.</p>
</div>

<div class="callout">
  <p>💡 <strong>Why it matters for my work:</strong> the charge-density-wave surfaces I study are
  delicate and react with air. UHV is what lets me cleave a fresh crystal face and then spend hours —
  sometimes days — imaging the very same atoms, confident that what I'm seeing is the material itself
  and not a layer of contamination.</p>
</div>

{% include gallery.html folder="/Photos/research/lab/uhv" %}
