---
title: "Making an atomically sharp STM tip"
category: "The craft"
icon: "📍"
order: 4
status: published
summary: "An STM is only as good as its tip. We shape a metal wire until it ends in a single atom — because the tunneling current is so lopsided that essentially all of it flows through that one frontmost atom."
---

<p>The whole idea of a scanning tunneling microscope rests on one delicate object: the
<strong>tip</strong>. It's just a fine metal wire, but its very end has to taper down to a
<em>single atom</em>. That sounds like an impossible manufacturing tolerance — until you realize
physics does most of the work for you.</p>

<h2 class="section-title">Why one atom is enough</h2>

<p>Tunneling current depends <strong>exponentially</strong> on the gap between tip and surface. Move
the tip away by just one atom's diameter and the current drops by roughly a factor of ten. So even on
a tip that looks blunt under a microscope, whichever atom happens to stick out farthest carries the
overwhelming majority of the current. That one lucky atom <em>is</em> the probe. Our job isn't to
carve a perfect needle — it's to make sure there's a single, stable atom out in front.</p>

<figure class="diagram">
  <svg viewBox="0 0 560 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Only the frontmost atom of the tip carries appreciable tunneling current to the surface">
    <!-- tip body: cluster of atoms tapering to one -->
    <g stroke="currentColor" stroke-width="1">
      <circle cx="230" cy="55" r="15" fill="#2774AE" fill-opacity="0.20"/>
      <circle cx="262" cy="55" r="15" fill="#2774AE" fill-opacity="0.20"/>
      <circle cx="294" cy="55" r="15" fill="#2774AE" fill-opacity="0.20"/>
      <circle cx="246" cy="82" r="15" fill="#2774AE" fill-opacity="0.24"/>
      <circle cx="278" cy="82" r="15" fill="#2774AE" fill-opacity="0.24"/>
      <circle cx="262" cy="108" r="15" fill="#2774AE" fill-opacity="0.30"/>
      <circle cx="262" cy="134" r="14" fill="#FFB81C" fill-opacity="0.85"/>
    </g>
    <text x="360" y="130" font-size="11" fill="#b8860b" font-weight="700">← frontmost atom</text>
    <!-- surface -->
    <line x1="90" y1="180" x2="470" y2="180" stroke="currentColor" stroke-width="2"/>
    <text x="280" y="198" font-size="10" text-anchor="middle" fill="currentColor">sample surface</text>
    <!-- current arrows: strong from front atom, faint from others -->
    <line x1="262" y1="148" x2="262" y2="176" stroke="#c0392b" stroke-width="3"/>
    <line x1="246" y1="96"  x2="240" y2="176" stroke="#c0392b" stroke-width="1" stroke-opacity="0.30" stroke-dasharray="3 3"/>
    <line x1="278" y1="96"  x2="286" y2="176" stroke="#c0392b" stroke-width="1" stroke-opacity="0.30" stroke-dasharray="3 3"/>
    <g font-size="11" font-weight="700">
      <text x="300" y="164" fill="#c0392b">most current here</text>
      <text x="150" y="150" fill="#c0392b" opacity="0.55">≈ none from</text>
      <text x="150" y="164" fill="#c0392b" opacity="0.55">the rest</text>
    </g>
  </svg>
  <figcaption>Because current falls off tenfold per atomic step, the single frontmost atom does
  almost all the tunneling — which is exactly why a tip only needs to be sharp in <em>one</em> spot.</figcaption>
</figure>

<h2 class="section-title">How we shape a tip</h2>

<div class="feature">
  <h3><span class="tag">1</span> Etch or cut the wire</h3>
  <p>We start from a fine wire — usually <strong>tungsten</strong>, which we sharpen by
  <em>electrochemical etching</em>: dipping the wire into a caustic bath and running a current so it
  dissolves fastest at the liquid's surface, eventually necking down to a fine point that drops away.
  For softer <strong>platinum–iridium</strong> wire, a good pair of cutters and a pulling motion is
  often enough to leave a jagged, usable apex.</p>
</div>

<div class="feature">
  <h3><span class="tag">2</span> Clean it in vacuum</h3>
  <p>A freshly etched tip is coated in oxide and grime. Inside UHV we heat it and pull electrons off
  it by <strong>field emission</strong>, blasting away the contamination until bare, clean metal is
  left at the end.</p>
</div>

<div class="feature">
  <h3><span class="tag">3</span> Condition it on a known surface</h3>
  <p>The real finishing happens on a clean, well-understood crystal (a gold surface is a favorite
  test bed). By gently touching the tip to the surface or applying small voltage pulses, we nudge its
  apex until it's stable and single-atom-sharp — judged by how crisply it images atoms we already know
  the answer for. Only then do we trust it on the material we actually care about.</p>
</div>

<div class="callout">
  <p>💡 <strong>The reality of it:</strong> tips are temperamental. A great one can go blunt in an
  instant by picking up a stray atom, and a huge part of the craft is quickly recognizing a bad tip
  and reshaping it — often dozens of times in a session — until the atoms snap into focus.</p>
</div>

{% include gallery.html folder="/Photos/research/lab/tips" %}
