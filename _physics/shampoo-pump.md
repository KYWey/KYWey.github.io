---
title: "How does a shampoo / soap pump work?"
category: "Machines & Motion"
icon: "🧴"
order: 21
summary: "It's a hand-powered piston pump with two one-way (check) valves and a return spring. Pressing forces a fixed dose out the nozzle; releasing sucks a fresh dose up from the bottle."
---

<p>That little dispenser is a <strong>positive-displacement piston pump</strong> with two one-way
(check) valves and a return spring. It moves a fixed slug of liquid on every press, no matter how
thick the shampoo is. The magic is that the two valves only ever let liquid flow <em>one way</em>,
so pushing and releasing both do useful work.</p>

<p><strong>Press down (the dispense stroke):</strong> the piston squeezes the liquid trapped in the
pump chamber. The rising pressure <em>seats</em> the bottom ball valve (sealing off the bottle) and
<em>opens</em> the top outlet valve, so the trapped liquid is forced out the nozzle.</p>

<p><strong>Let go (the refill stroke):</strong> the spring pushes the piston back up, expanding the
chamber. The pressure drops below atmospheric, which now <em>closes</em> the outlet valve and
<em>lifts</em> the bottom ball off its seat. Ordinary air pressure on the liquid in the bottle then
pushes fresh shampoo up the dip tube to refill the chamber — ready for the next press. (This is
also why the first few pumps on a new bottle spit air: the chamber has to "prime" first.)</p>

<figure class="diagram">
  <svg viewBox="0 0 640 380" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Cross-section of a lotion pump on the press and release strokes">
    <defs>
      <marker id="pumpblue" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="#00A6D6"/></marker>
      <marker id="pumpink" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="currentColor"/></marker>
    </defs>
    <text x="160" y="26" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Press down → dispense</text>
    <line x1="160" y1="34" x2="160" y2="60" stroke="currentColor" stroke-width="3" marker-end="url(#pumpink)"/>
    <rect x="120" y="60" width="80" height="20" rx="5" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
    <path d="M120,66 L92,66 L92,74 L120,74" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
    <line x1="90" y1="70" x2="60" y2="80" stroke="#00A6D6" stroke-width="3" marker-end="url(#pumpblue)"/>
    <circle cx="66" cy="86" r="3" fill="#00A6D6"/><circle cx="55" cy="92" r="2.5" fill="#00A6D6"/>
    <rect x="155" y="80" width="10" height="35" fill="currentColor" opacity="0.5"/>
    <rect x="130" y="115" width="60" height="120" rx="4" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <circle cx="160" cy="128" r="6" fill="none" stroke="#2774AE" stroke-width="2"/>
    <text x="198" y="126" font-size="10" fill="currentColor">outlet</text>
    <text x="198" y="138" font-size="10" fill="#2774AE" font-weight="700">OPEN</text>
    <rect x="132" y="150" width="56" height="12" rx="2" fill="#2774AE" fill-opacity="0.7" stroke="currentColor"/>
    <rect x="132" y="162" width="56" height="60" fill="#00A6D6" fill-opacity="0.28"/>
    <polyline points="150,222 170,225 150,228 170,231 150,234" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <path d="M148,246 L172,246 L160,232 Z" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <circle cx="160" cy="240" r="6" fill="#c0392b" fill-opacity="0.85"/>
    <text x="60" y="250" font-size="10" fill="currentColor" text-anchor="middle">inlet ball</text>
    <text x="60" y="262" font-size="10" fill="#c0392b" text-anchor="middle" font-weight="700">CLOSED</text>
    <rect x="153" y="246" width="14" height="80" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <rect x="95" y="326" width="130" height="44" fill="#00A6D6" fill-opacity="0.28" stroke="currentColor"/>
    <text x="160" y="352" font-size="10" fill="currentColor" text-anchor="middle">shampoo in bottle</text>
    <line x1="320" y1="35" x2="320" y2="360" stroke="currentColor" stroke-width="1" opacity="0.2"/>
    <text x="470" y="26" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Release → spring refills</text>
    <line x1="470" y1="60" x2="470" y2="34" stroke="#FFB81C" stroke-width="3" marker-end="url(#pumpink)"/>
    <text x="512" y="50" font-size="10" fill="currentColor">spring push</text>
    <rect x="430" y="52" width="80" height="20" rx="5" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
    <path d="M430,58 L402,58 L402,66 L430,66" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
    <rect x="465" y="72" width="10" height="30" fill="currentColor" opacity="0.5"/>
    <rect x="440" y="115" width="60" height="120" rx="4" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <circle cx="470" cy="128" r="6" fill="#c0392b" fill-opacity="0.85" stroke="currentColor"/>
    <text x="508" y="126" font-size="10" fill="currentColor">outlet</text>
    <text x="508" y="138" font-size="10" fill="#c0392b" font-weight="700">CLOSED</text>
    <rect x="442" y="120" width="56" height="12" rx="2" fill="#2774AE" fill-opacity="0.7" stroke="currentColor"/>
    <rect x="442" y="180" width="56" height="42" fill="#00A6D6" fill-opacity="0.28"/>
    <polyline points="460,150 480,153 460,158 480,163 460,168 480,173 460,178" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <path d="M458,246 L482,246 L470,232 Z" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <circle cx="470" cy="228" r="6" fill="#2774AE" fill-opacity="0.85"/>
    <text x="405" y="250" font-size="10" fill="currentColor" text-anchor="middle">inlet ball</text>
    <text x="405" y="262" font-size="10" fill="#2774AE" text-anchor="middle" font-weight="700">OPEN</text>
    <rect x="463" y="240" width="14" height="86" fill="none" stroke="currentColor" stroke-width="1.5"/>
    <line x1="470" y1="322" x2="470" y2="250" stroke="#00A6D6" stroke-width="3" marker-end="url(#pumpblue)"/>
    <rect x="405" y="326" width="130" height="44" fill="#00A6D6" fill-opacity="0.28" stroke="currentColor"/>
    <text x="470" y="352" font-size="10" fill="currentColor" text-anchor="middle">air pressure pushes liquid up</text>
  </svg>
  <figcaption>Two one-way valves + a spring. Pressing forces liquid out the top; releasing sucks
  a fresh dose up from the bottle. The same design (a reciprocating piston pump) scales all the way
  up to the pumps in your car and home.</figcaption>
</figure>
