---
title: "Why won't my cold food box (or fridge door) reopen?"
category: "Heat & Gases"
icon: "🧊"
order: 41
summary: "As the trapped warm air cools it contracts (ideal gas law), so its pressure falls below the room's. The higher outside pressure then clamps the lid — or fridge door — shut until the seal leaks or you let air back in."
---

<p>I read this as the classic <em>"I put a warm food box in the fridge, it got cold, and now the
lid won't come off"</em> — the same effect that makes a fridge door feel glued shut for a moment
right after you close it. Either way the culprit is <strong>thermal contraction of the trapped air</strong>.</p>

<p>When you seal warm air inside a container (or shut warm room air into the fridge) and it cools,
the gas obeys the ideal gas law. At (roughly) fixed volume, pressure falls in step with absolute
temperature:</p>

<div class="eq">
  \( \dfrac{P_1}{T_1} = \dfrac{P_2}{T_2} \qquad\Rightarrow\qquad F = \Delta P \cdot A \)
  <span class="eq-note">Cool 25 °C (298 K) → 5 °C (278 K) and the inside pressure drops ~7%.
  Water vapor condensing inside lowers it even more.</span>
</div>

<p>Now the higher outside air pressure clamps the lid (or door) shut, and the force is bigger than
it feels like it should be. A 7% drop is about 7 kPa; over a modest 0.03 m² lid that's roughly
<strong>200 N — like a 20 kg weight sitting on it</strong>. On a big fridge door the seal usually
leaks fast enough to equalize in a few seconds (which is exactly why waiting a moment lets you open
it); a well-sealed food box can stay stuck much longer. The fixes are all about breaking the seal
or letting air back in: run the lid rim under warm water (re-expands the gas), pry a corner to let
air whistle in, or — for the fridge — just wait a beat.</p>

<figure class="diagram">
  <svg viewBox="0 0 640 290" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="A sealed container's air contracts as it cools, so outside pressure clamps the lid">
    <defs>
      <marker id="frink" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="currentColor"/></marker>
    </defs>
    <text x="160" y="30" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Just sealed · warm (25 °C)</text>
    <rect x="90" y="90" width="140" height="120" rx="6" fill="none" stroke="currentColor" stroke-width="2"/>
    <rect x="82" y="78" width="156" height="16" rx="4" fill="#2774AE" fill-opacity="0.5" stroke="currentColor"/>
    <text x="160" y="72" font-size="10" fill="currentColor" text-anchor="middle">lid (loose)</text>
    <g fill="#c0392b">
      <circle cx="118" cy="120" r="4"/><circle cx="160" cy="110" r="4"/><circle cx="205" cy="130" r="4"/>
      <circle cx="130" cy="165" r="4"/><circle cx="185" cy="170" r="4"/><circle cx="150" cy="145" r="4"/>
      <circle cx="200" cy="185" r="4"/><circle cx="110" cy="190" r="4"/>
    </g>
    <text x="160" y="235" font-size="10" fill="currentColor" text-anchor="middle" opacity="0.8">inside pressure = outside</text>
    <line x1="270" y1="150" x2="350" y2="150" stroke="currentColor" stroke-width="2.5" marker-end="url(#frink)"/>
    <text x="310" y="140" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">cools</text>
    <text x="480" y="30" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Cold (5 °C) · lid clamped</text>
    <rect x="410" y="90" width="140" height="120" rx="6" fill="none" stroke="currentColor" stroke-width="2"/>
    <rect x="402" y="86" width="156" height="16" rx="4" fill="#2774AE" fill-opacity="0.75" stroke="currentColor"/>
    <line x1="440" y1="64" x2="440" y2="84" stroke="#c0392b" stroke-width="2.4" marker-end="url(#frink)"/>
    <line x1="480" y1="64" x2="480" y2="84" stroke="#c0392b" stroke-width="2.4" marker-end="url(#frink)"/>
    <line x1="520" y1="64" x2="520" y2="84" stroke="#c0392b" stroke-width="2.4" marker-end="url(#frink)"/>
    <text x="480" y="56" font-size="10" fill="#c0392b" text-anchor="middle" font-weight="700">outside air pushes in</text>
    <g fill="#2774AE">
      <circle cx="455" cy="185" r="4"/><circle cx="475" cy="190" r="4"/><circle cx="495" cy="183" r="4"/>
      <circle cx="465" cy="170" r="4"/><circle cx="488" cy="172" r="4"/><circle cx="505" cy="192" r="4"/>
      <circle cx="445" cy="196" r="4"/><circle cx="515" cy="178" r="4"/>
    </g>
    <text x="480" y="235" font-size="10" fill="currentColor" text-anchor="middle" opacity="0.85">lower pressure inside → partial vacuum</text>
    <text x="320" y="272" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">Same air, colder → less pressure → outside wins → stuck lid</text>
  </svg>
  <figcaption>Cooling doesn't remove air, it just makes the trapped air press outward less. The
  unchanged outside pressure then wins, clamping the lid (or door) until the seal leaks or you let
  air back in.</figcaption>
</figure>

<div class="callout">
  <p>📝 If by "fuse box" you literally meant your electrical panel, let me know — that would be a
  totally different question and I'll write it up separately!</p>
</div>
