---
title: "Why does a coffee drop dry into a ring?"
category: "Fluids & Flow"
icon: "☕"
order: 13
summary: "The drop's edge is pinned and evaporates fastest, so liquid flows outward to refill it, carrying the suspended coffee particles to the rim and stranding them in a dark ring."
---

<p>A spilled drop of coffee dries darkest at its <em>edge</em>, not the middle — the famous
"coffee-ring effect." The rim of the drop is pinned to the surface and can't retreat, and liquid
evaporates fastest there. To replace what's lost, liquid flows outward from the center to the edge,
carrying the suspended coffee particles with it and stranding them in a ring. It's a headache for
inkjet printing and coating uniform films — and a neat way to see fluid flow with your own eyes.</p>

<figure class="diagram">
  <svg viewBox="0 0 560 190" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Coffee ring: outward flow carries particles to the pinned edge">
    <defs>
      <marker id="cofink" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#2774AE"/></marker>
      <marker id="cofred" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c0392b"/></marker>
    </defs>
    <line x1="60" y1="140" x2="500" y2="140" stroke="currentColor" stroke-width="2"/>
    <path d="M150,140 Q280,60 410,140 Z" fill="#2774AE" fill-opacity="0.22" stroke="currentColor" stroke-width="1.5"/>
    <line x1="160" y1="130" x2="140" y2="95" stroke="#c0392b" stroke-width="1.8" marker-end="url(#cofred)"/>
    <line x1="400" y1="130" x2="420" y2="95" stroke="#c0392b" stroke-width="1.8" marker-end="url(#cofred)"/>
    <text x="120" y="88" font-size="10" fill="#c0392b">evap.</text>
    <text x="425" y="88" font-size="10" fill="#c0392b">evap.</text>
    <line x1="270" y1="128" x2="185" y2="132" stroke="#2774AE" stroke-width="2" marker-end="url(#cofink)"/>
    <line x1="290" y1="128" x2="375" y2="132" stroke="#2774AE" stroke-width="2" marker-end="url(#cofink)"/>
    <text x="280" y="118" font-size="10" fill="#2774AE" text-anchor="middle" font-weight="700">flow carries particles out</text>
    <circle cx="155" cy="136" r="4" fill="#3a2b00"/><circle cx="163" cy="139" r="4" fill="#3a2b00"/>
    <circle cx="405" cy="136" r="4" fill="#3a2b00"/><circle cx="397" cy="139" r="4" fill="#3a2b00"/>
    <text x="280" y="175" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">→ dark ring at the pinned edge</text>
  </svg>
  <figcaption>Faster evaporation at the pinned rim drives an outward flow that piles particles up
  around the edge.</figcaption>
</figure>
