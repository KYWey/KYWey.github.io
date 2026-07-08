---
title: "Einstein's tea-leaf paradox"
category: "Fluids & Flow"
icon: "🍵"
order: 14
myth: "Stirring the tea should fling the leaves outward and pin them against the rim."
real: "Friction at the bottom sets up a secondary flow — inward along the base, up the middle — that sweeps the leaves into a neat pile at the center. Einstein worked this one out."
---

<p>Stir a cup of tea and the leaves gather in a neat pile at the <em>center</em> of the bottom — not
flung to the rim as you'd expect. Einstein explained it: spinning liquid piles up slightly at the
outer wall (higher pressure there), but friction at the bottom slows the fluid near the base, so it
can't spin fast enough to balance that pressure. The result is a gentle <strong>secondary
flow</strong> — inward along the bottom, up the middle, out along the top — that sweeps the leaves
into the center. The same "teacup" secondary flow explains how river bends erode their outer banks,
and it's used in engineering to separate particles from liquids.</p>

<figure class="diagram">
  <svg viewBox="0 0 560 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Secondary flow in a stirred cup sweeps leaves to the center">
    <defs>
      <marker id="teaink" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#2774AE"/></marker>
    </defs>
    <path d="M120,40 L140,170 L420,170 L440,40" fill="#2774AE" fill-opacity="0.12" stroke="currentColor" stroke-width="1.8"/>
    <line x1="120" y1="40" x2="440" y2="40" stroke="currentColor" stroke-width="1.8"/>
    <path d="M175,160 Q160,90 275,60 Q400,90 385,160" fill="none" stroke="#2774AE" stroke-width="2" stroke-dasharray="6 4"/>
    <path d="M280,160 L200,163" fill="none" stroke="#2774AE" stroke-width="2.2" marker-end="url(#teaink)"/>
    <path d="M280,160 L360,163" fill="none" stroke="#2774AE" stroke-width="2.2" marker-end="url(#teaink)"/>
    <line x1="280" y1="150" x2="280" y2="80" stroke="#2774AE" stroke-width="2.2" marker-end="url(#teaink)"/>
    <text x="280" y="110" font-size="10" fill="#2774AE" text-anchor="middle" font-weight="700">up the middle</text>
    <text x="280" y="150" font-size="10" fill="#2774AE" text-anchor="middle">inward along the bottom</text>
    <circle cx="272" cy="166" r="4" fill="#3a2b00"/><circle cx="282" cy="167" r="4" fill="#3a2b00"/><circle cx="290" cy="165" r="4" fill="#3a2b00"/>
    <text x="280" y="192" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">leaves collect in the center</text>
  </svg>
  <figcaption>Bottom friction breaks the balance between spin and pressure, driving a slow inward
  sweep along the base — right into the center.</figcaption>
</figure>
