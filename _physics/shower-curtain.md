---
title: "Why does the shower curtain billow inward?"
category: "Fluids & Flow"
icon: "🚿"
order: 12
summary: "The shower lowers the air pressure behind the curtain — fast-moving air dragged by the spray, plus a slow warm-air vortex — so the higher pressure outside pushes the curtain in against you."
---

<p>Turn on the shower and the curtain billows <em>inward</em>, sticking to your legs. The tidy
explanation is Bernoulli's principle — the fast-moving air dragged along by the falling water has
lower pressure, so the higher pressure outside pushes the curtain in. The fuller story is that the
spray also sets up a slow rotating vortex (a "bathroom buoyancy" plume from warm, humid air rising)
that lowers the pressure behind the curtain. Either way: lower pressure inside, so the curtain gets
shoved toward you. A weighted hem, or a curtain that bows outward, fixes it.</p>

<figure class="diagram">
  <svg viewBox="0 0 560 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Lower pressure behind a shower curtain pushes it inward">
    <defs>
      <marker id="showink" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="currentColor"/></marker>
      <marker id="showblue" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#00A6D6"/></marker>
    </defs>
    <line x1="60" y1="30" x2="60" y2="185" stroke="currentColor" stroke-width="3"/>
    <text x="70" y="24" font-size="10" fill="currentColor">wall / showerhead side</text>
    <!-- spray -->
    <line x1="80" y1="40" x2="95" y2="150" stroke="#00A6D6" stroke-width="2" marker-end="url(#showblue)"/>
    <line x1="100" y1="40" x2="115" y2="150" stroke="#00A6D6" stroke-width="2" marker-end="url(#showblue)"/>
    <text x="120" y="45" font-size="10" fill="#00A6D6">falling water drags air down → low pressure</text>
    <!-- curtain billowing in (curve bowing right-to-left) -->
    <path d="M470,30 Q360,105 470,185" fill="#2774AE" fill-opacity="0.14" stroke="currentColor" stroke-width="2.5"/>
    <text x="485" y="110" font-size="10" fill="currentColor">curtain</text>
    <!-- outside pressure arrows pushing left -->
    <line x1="540" y1="70" x2="480" y2="80" stroke="#c0392b" stroke-width="2.2" marker-end="url(#showink)"/>
    <line x1="540" y1="150" x2="480" y2="140" stroke="#c0392b" stroke-width="2.2" marker-end="url(#showink)"/>
    <text x="500" y="200" font-size="10" fill="#c0392b" text-anchor="middle" font-weight="700">higher outside pressure pushes in</text>
  </svg>
  <figcaption>Lower pressure on the shower side means the ordinary room-air pressure outside wins,
  bowing the curtain inward.</figcaption>
</figure>
