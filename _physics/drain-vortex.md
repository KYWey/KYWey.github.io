---
title: "Which way does water swirl down the drain?"
category: "Fluids & Flow"
icon: "🌀"
order: 11
myth: "Water spins counter-clockwise in the Northern Hemisphere and clockwise in the Southern — it's the Coriolis force, the same thing that spins hurricanes."
real: "For a real sink or toilet the swirl is set by how the water was already moving plus the basin shape and inlet jets; the Coriolis force is thousands of times too weak to decide it."
---

<p>The Coriolis force is an apparent sideways deflection felt by anything moving over a rotating
planet. Its acceleration is</p>

<div class="eq">
  \( a_c = 2\,\Omega\, v \sin\varphi \)
  <span class="eq-note">Ω = Earth's rotation rate ≈ 7.3 × 10⁻⁵ s⁻¹, v = speed, φ = latitude</span>
</div>

<p>Plug in a sink: at mid-latitude, water creeping toward the drain at <em>v</em> ≈ 0.1 m/s gives
<em>a<sub>c</sub></em> ≈ 10⁻⁵ m/s² — around a millionth of gravity. Any leftover sloshing from
filling the basin, the tilt of the bowl, or the angle of the tap completely swamps it. The honest
way to compare the two effects is the <strong>Rossby number</strong>, the ratio of ordinary
(inertial) forces to the Coriolis force:</p>

<div class="eq">
  \( \mathrm{Ro} = \dfrac{U}{f L} \)
  <span class="eq-note">Coriolis matters only when Ro ≪ 1. Sink: Ro ≈ 10⁴ → negligible.
  Hurricane (L ~ 100s of km, slow): Ro ≪ 1 → Coriolis dominates.</span>
</div>

<figure class="diagram">
  <svg viewBox="0 0 640 320" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Coriolis rotation on Earth versus the swirl in a household sink">
    <circle cx="165" cy="160" r="118" fill="#2774AE" fill-opacity="0.10" stroke="currentColor" stroke-width="1.5"/>
    <line x1="47" y1="160" x2="283" y2="160" stroke="currentColor" stroke-width="1.3" stroke-dasharray="6 5"/>
    <text x="120" y="177" font-size="11" fill="currentColor" opacity="0.7">equator</text>
    <circle cx="165" cy="98" r="26" fill="none" stroke="#2774AE" stroke-width="3.5"/>
    <path d="M191,98 L182,88 L182,108 Z" fill="#2774AE"/>
    <text x="165" y="52" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">N: counter-clockwise</text>
    <circle cx="165" cy="222" r="26" fill="none" stroke="#c0392b" stroke-width="3.5"/>
    <path d="M191,222 L182,212 L182,232 Z" fill="#c0392b"/>
    <text x="165" y="284" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">S: clockwise</text>
    <text x="165" y="300" font-size="10" fill="currentColor" text-anchor="middle" opacity="0.7">(true for big storms only)</text>
    <line x1="330" y1="35" x2="330" y2="290" stroke="currentColor" stroke-width="1" opacity="0.2"/>
    <text x="500" y="45" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">Your sink / toilet</text>
    <ellipse cx="500" cy="165" rx="95" ry="72" fill="#00A6D6" fill-opacity="0.14" stroke="currentColor" stroke-width="1.5"/>
    <path d="M430,120 q35,15 55,30" fill="none" stroke="#00A6D6" stroke-width="2.5" marker-end="url(#drainarrow)"/>
    <path d="M572,205 q-35,-15 -55,-30" fill="none" stroke="#00A6D6" stroke-width="2.5" marker-end="url(#drainarrow)"/>
    <text x="415" y="112" font-size="10" fill="currentColor">jet</text>
    <text x="573" y="223" font-size="10" fill="currentColor">jet</text>
    <circle cx="500" cy="165" r="34" fill="none" stroke="#00A6D6" stroke-width="3.5"/>
    <path d="M534,165 L525,155 L525,175 Z" fill="#00A6D6"/>
    <circle cx="500" cy="165" r="6" fill="currentColor"/>
    <text x="500" y="255" font-size="10" fill="currentColor" text-anchor="middle" opacity="0.85">direction fixed by jets &amp; basin, not the planet</text>
    <defs>
      <marker id="drainarrow" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#00A6D6"/></marker>
    </defs>
  </svg>
  <figcaption>The Coriolis force does set the spin of hurricanes (huge, slow systems). A sink is
  tiny and fast, so its Rossby number is enormous and the planet's rotation is irrelevant.</figcaption>
</figure>

<p><strong>The twist:</strong> the effect <em>can</em> be seen in a sink — but only in a careful
experiment. In the classic 1962 tests (Ascher Shapiro at MIT, and a mirror-image one in Sydney), a
perfectly symmetric tank was filled and left to sit still for a full day so all residual motion
died away. Only then, with a tiny central drain, did the water reliably spin counter-clockwise in
the north and clockwise in the south. Your toilet, by contrast, just follows its rim jets — which
is why identical toilet models flush the same way in both hemispheres.</p>
