---
title: "Why is the sky blue (and sunsets red)?"
category: "Light & Color"
icon: "🌈"
order: 51
summary: "Air scatters short-wavelength blue light far more than red (Rayleigh scattering ∝ 1/λ⁴), so the daytime sky glows blue. At sunset the light travels a long slant through the air, scattering the blue away and leaving the red."
---

<p>Sunlight is a mix of all colors, and air molecules scatter it — but not evenly. This is
<strong>Rayleigh scattering</strong>, which is dramatically stronger for shorter wavelengths
(scattering ∝ 1/λ⁴). Blue and violet get bounced around the sky far more than red, so the whole
daytime sky glows blue (we see blue more than violet partly because the Sun emits less violet and
our eyes are less sensitive to it). At sunset the light skims through <em>much</em> more atmosphere,
so nearly all the blue is scattered away before it reaches you — what's left arriving straight from
the Sun is the leftover red and orange.</p>

<figure class="diagram">
  <svg viewBox="0 0 560 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Rayleigh scattering: blue scatters across the sky, red passes through at sunset">
    <defs>
      <marker id="skyblue" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#00A6D6"/></marker>
      <marker id="skyred" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c0392b"/></marker>
    </defs>
    <rect x="40" y="40" width="480" height="130" rx="10" fill="#00A6D6" fill-opacity="0.08" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4"/>
    <text x="55" y="60" font-size="10" fill="currentColor" opacity="0.7">atmosphere (air molecules)</text>
    <line x1="60" y1="80" x2="250" y2="120" stroke="#FFB81C" stroke-width="3"/>
    <text x="70" y="76" font-size="10" fill="currentColor">white sunlight</text>
    <circle cx="250" cy="120" r="4" fill="currentColor"/>
    <line x1="250" y1="120" x2="290" y2="70" stroke="#00A6D6" stroke-width="2" marker-end="url(#skyblue)"/>
    <line x1="250" y1="120" x2="210" y2="70" stroke="#00A6D6" stroke-width="2" marker-end="url(#skyblue)"/>
    <line x1="250" y1="120" x2="300" y2="150" stroke="#00A6D6" stroke-width="2" marker-end="url(#skyblue)"/>
    <text x="300" y="60" font-size="10" fill="#00A6D6" font-weight="700">blue scatters everywhere → blue sky</text>
    <line x1="250" y1="120" x2="480" y2="150" stroke="#c0392b" stroke-width="3" marker-end="url(#skyred)"/>
    <text x="360" y="180" font-size="10" fill="#c0392b" font-weight="700">red passes through → red sunset</text>
  </svg>
  <figcaption>Short-wavelength blue light scatters strongly in every direction (blue sky); the red
  that survives the long slant through the atmosphere at dusk gives us sunsets.</figcaption>
</figure>
