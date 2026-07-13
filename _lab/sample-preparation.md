---
title: "Preparing & keeping samples clean"
category: "The craft"
icon: "🧫"
order: 3
status: published
summary: "We expose a fresh, atomically flat crystal face by cleaving it inside vacuum — then shuttle it from chamber to chamber on specialized holders without ever letting it touch air."
---

<p>Before we can image a material, we have to give the microscope a surface worth looking at. A
crystal that's been sitting in a drawer is coated in a skin of oxide, water, and dust — useless for
atomic-resolution work. What we actually want is a surface that has <em>never</em> met air. The trick
is to make one <strong>inside</strong> the vacuum, and then never break that seal.</p>

<h2 class="section-title">Making a fresh surface: cleaving</h2>

<p>Many of the quantum materials I study are <strong>layered</strong> — stacks of atomic sheets held
together weakly, a bit like a deck of cards or a block of mica. We take advantage of that. We glue a
small post to the top of the crystal, pump the whole thing down to <a href="{{ '/research/lab/ultra-high-vacuum/' | relative_url }}">ultra-high vacuum</a>,
and then knock the post off. The crystal splits cleanly along a single atomic plane, revealing a
mirror-flat face that is <strong>pristine and air-free from the moment it's born</strong>.</p>

<figure class="diagram">
  <svg viewBox="0 0 560 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="A post glued on top of a layered crystal is knocked sideways, splitting the crystal along a clean atomic plane">
    <defs>
      <marker id="clvarrow" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c0392b"/></marker>
    </defs>
    <!-- layered crystal -->
    <g stroke="currentColor" stroke-width="1.3">
      <rect x="140" y="140" width="200" height="10" fill="#2774AE" fill-opacity="0.28"/>
      <rect x="140" y="128" width="200" height="10" fill="#2774AE" fill-opacity="0.22"/>
      <rect x="140" y="116" width="200" height="10" fill="#2774AE" fill-opacity="0.16"/>
      <rect x="140" y="104" width="200" height="10" fill="#2774AE" fill-opacity="0.10"/>
    </g>
    <text x="240" y="172" font-size="10" text-anchor="middle" fill="currentColor">layered crystal on its holder</text>
    <!-- post -->
    <rect x="215" y="60" width="50" height="44" fill="currentColor" fill-opacity="0.35" stroke="currentColor"/>
    <text x="240" y="52" font-size="10" text-anchor="middle" fill="currentColor">glued post</text>
    <!-- knock -->
    <line x1="330" y1="82" x2="272" y2="82" stroke="#c0392b" stroke-width="2.2" marker-end="url(#clvarrow)"/>
    <text x="392" y="86" font-size="11" text-anchor="middle" font-weight="700" fill="#c0392b">knock it off</text>
    <!-- cleavage plane -->
    <line x1="140" y1="103" x2="340" y2="103" stroke="#FFB81C" stroke-width="2.5" stroke-dasharray="6 4"/>
    <text x="240" y="96" font-size="10" text-anchor="middle" font-weight="700" fill="#b8860b">← fresh surface splits off here →</text>
  </svg>
  <figcaption>Cleaving in vacuum: a post glued to the top layer is knocked sideways, and the crystal
  peels apart along one atomic plane — exposing a surface that has never touched air.</figcaption>
</figure>

<h2 class="section-title">Holding the sample</h2>

<p>A crystal is no good floating loose — it has to be clamped onto a standardized <strong>sample
holder</strong> that the microscope's grippers, manipulators, and cold stage all know how to grab.
Different chambers use different designs, but they all do the same job: hold the crystal flat, make
solid electrical contact, and give the in-vacuum tools something to latch onto. The photos below show
two of ours — one with spring clips and a moveable anvil that pin the sample down, and an
STM plate where the sample seats flush against a machined pocket.</p>

{% include gallery.html folder="/Photos/research/lab/sample" %}

<h2 class="section-title">Never breaking the seal</h2>

<p>Once a sample is inside, the whole game is keeping it there. We move it between chambers — a fast
entry <em>load-lock</em>, a preparation chamber, the cold microscope — using long
<strong>manipulator arms</strong> and "wobble sticks," all without ever exposing it to the room. A
sample can spend days migrating around the system and still present the same clean face it had the
second it was cleaved.</p>

<div class="callout">
  <p>💡 <strong>Why it matters for my work:</strong> the charge-density-wave surfaces I study would
  react and reorganize within seconds in air. Cleaving in vacuum and handling everything under
  UHV is the only way to be sure the atoms I'm imaging are the material's true surface — not a
  contaminated imposter.</p>
</div>
