---
layout: page
title: "Interesting Life Physics"
permalink: /fun/physics/
mathjax: true
---

<p><a href="{{ '/fun/' | relative_url }}">← Back to Fun Life</a></p>

# Interesting Life Physics ☕🚲✈️

<p class="lead">Physics isn't just something that happens in the lab — it's in your bathroom sink,
your shampoo bottle, your bike ride, the sky above you, and even your fridge. This page collects
the small "wait, why does that happen?" moments and unpacks them in a friendly (but honest) way.
Where the popular explanation is a myth, I'll say so — and tell you what's really going on.</p>

<div class="toc-box">
  <strong>On this page</strong>
  <ol>
    <li><a href="#drain">Which way does water swirl down the drain?</a></li>
    <li><a href="#pump">How does a shampoo/soap pump actually work?</a></li>
    <li><a href="#bike">Why doesn't a moving bicycle fall over?</a></li>
    <li><a href="#flight">How does a plane fly — and how is a bird different?</a></li>
    <li><a href="#fridge">Why won't my cold food box (or fridge door) reopen?</a></li>
    <li><a href="#bonus">Bonus round: four more everyday mysteries</a></li>
  </ol>
</div>

<!-- ============================================================ -->
<h2 class="section-title" id="drain">1 · Which way does water swirl down the drain?</h2>

<div class="feature">
  <h3>🌀 Is it the Coriolis force?</h3>

  <div class="myth-real">
    <div class="myth">
      <h4>❌ The popular story</h4>
      <p>"Water spirals counter-clockwise down a drain in the Northern Hemisphere and clockwise in
      the Southern — it's the Coriolis force, the same thing that spins hurricanes."</p>
    </div>
    <div class="real">
      <h4>✅ What's really true</h4>
      <p>For an ordinary sink or toilet, the swirl direction is set by how the water was already
      moving and by the shape of the basin and its inlet jets. The Coriolis force is real, but on
      that scale it's <em>thousands of times too weak</em> to decide the direction.</p>
    </div>
  </div>

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
      <!-- Earth -->
      <circle cx="165" cy="160" r="118" fill="#2774AE" fill-opacity="0.10" stroke="currentColor" stroke-width="1.5"/>
      <line x1="47" y1="160" x2="283" y2="160" stroke="currentColor" stroke-width="1.3" stroke-dasharray="6 5"/>
      <text x="120" y="177" font-size="11" fill="currentColor" opacity="0.7">equator</text>
      <!-- Northern hemisphere: counter-clockwise -->
      <circle cx="165" cy="98" r="26" fill="none" stroke="#2774AE" stroke-width="3.5"/>
      <path d="M191,98 L182,88 L182,108 Z" fill="#2774AE"/>
      <text x="165" y="52" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">N: counter-clockwise</text>
      <!-- Southern hemisphere: clockwise -->
      <circle cx="165" cy="222" r="26" fill="none" stroke="#c0392b" stroke-width="3.5"/>
      <path d="M191,222 L182,212 L182,232 Z" fill="#c0392b"/>
      <text x="165" y="284" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">S: clockwise</text>
      <text x="165" y="300" font-size="10" fill="currentColor" text-anchor="middle" opacity="0.7">(true for big storms only)</text>
      <!-- divider -->
      <line x1="330" y1="35" x2="330" y2="290" stroke="currentColor" stroke-width="1" opacity="0.2"/>
      <!-- Sink -->
      <text x="500" y="45" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">Your sink / toilet</text>
      <ellipse cx="500" cy="165" rx="95" ry="72" fill="#00A6D6" fill-opacity="0.14" stroke="currentColor" stroke-width="1.5"/>
      <!-- inlet jets -->
      <path d="M430,120 q35,15 55,30" fill="none" stroke="#00A6D6" stroke-width="2.5" marker-end="url(#drainarrow)"/>
      <path d="M572,205 q-35,-15 -55,-30" fill="none" stroke="#00A6D6" stroke-width="2.5" marker-end="url(#drainarrow)"/>
      <text x="415" y="112" font-size="10" fill="currentColor">jet</text>
      <text x="573" y="223" font-size="10" fill="currentColor">jet</text>
      <!-- swirl -->
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
</div>

<!-- ============================================================ -->
<h2 class="section-title" id="pump">2 · How does a shampoo / soap pump work?</h2>

<div class="feature">
  <h3>🧴 A tiny hand-powered piston pump</h3>
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

      <!-- ===== LEFT: PRESS DOWN ===== -->
      <text x="160" y="26" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Press down → dispense</text>
      <!-- big down arrow on button -->
      <line x1="160" y1="34" x2="160" y2="60" stroke="currentColor" stroke-width="3" marker-end="url(#pumpink)"/>
      <!-- button + nozzle -->
      <rect x="120" y="60" width="80" height="20" rx="5" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
      <path d="M120,66 L92,66 L92,74 L120,74" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
      <!-- ejected liquid -->
      <line x1="90" y1="70" x2="60" y2="80" stroke="#00A6D6" stroke-width="3" marker-end="url(#pumpblue)"/>
      <circle cx="66" cy="86" r="3" fill="#00A6D6"/><circle cx="55" cy="92" r="2.5" fill="#00A6D6"/>
      <!-- rod -->
      <rect x="155" y="80" width="10" height="35" fill="currentColor" opacity="0.5"/>
      <!-- chamber -->
      <rect x="130" y="115" width="60" height="120" rx="4" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <!-- outlet valve OPEN (near top of chamber) -->
      <circle cx="160" cy="128" r="6" fill="none" stroke="#2774AE" stroke-width="2"/>
      <text x="198" y="126" font-size="10" fill="currentColor">outlet</text>
      <text x="198" y="138" font-size="10" fill="#2774AE" font-weight="700">OPEN</text>
      <!-- piston (pushed low) -->
      <rect x="132" y="150" width="56" height="12" rx="2" fill="#2774AE" fill-opacity="0.7" stroke="currentColor"/>
      <!-- liquid below piston being squeezed -->
      <rect x="132" y="162" width="56" height="60" fill="#00A6D6" fill-opacity="0.28"/>
      <!-- spring compressed (short zigzag) -->
      <polyline points="150,222 170,225 150,228 170,231 150,234" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <!-- inlet ball valve CLOSED (seated) -->
      <path d="M148,246 L172,246 L160,232 Z" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <circle cx="160" cy="240" r="6" fill="#c0392b" fill-opacity="0.85"/>
      <text x="60" y="250" font-size="10" fill="currentColor" text-anchor="middle">inlet ball</text>
      <text x="60" y="262" font-size="10" fill="#c0392b" text-anchor="middle" font-weight="700">CLOSED</text>
      <!-- dip tube + bottle liquid -->
      <rect x="153" y="246" width="14" height="80" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <rect x="95" y="326" width="130" height="44" fill="#00A6D6" fill-opacity="0.28" stroke="currentColor"/>
      <text x="160" y="352" font-size="10" fill="currentColor" text-anchor="middle">shampoo in bottle</text>

      <!-- divider -->
      <line x1="320" y1="35" x2="320" y2="360" stroke="currentColor" stroke-width="1" opacity="0.2"/>

      <!-- ===== RIGHT: RELEASE ===== -->
      <text x="470" y="26" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Release → spring refills</text>
      <!-- big up arrow on button -->
      <line x1="470" y1="60" x2="470" y2="34" stroke="#FFB81C" stroke-width="3" marker-end="url(#pumpink)"/>
      <text x="512" y="50" font-size="10" fill="currentColor">spring push</text>
      <!-- button + nozzle (raised) -->
      <rect x="430" y="52" width="80" height="20" rx="5" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
      <path d="M430,58 L402,58 L402,66 L430,66" fill="#2774AE" fill-opacity="0.55" stroke="currentColor"/>
      <!-- rod -->
      <rect x="465" y="72" width="10" height="30" fill="currentColor" opacity="0.5"/>
      <!-- chamber -->
      <rect x="440" y="115" width="60" height="120" rx="4" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <!-- outlet valve CLOSED -->
      <circle cx="470" cy="128" r="6" fill="#c0392b" fill-opacity="0.85" stroke="currentColor"/>
      <text x="508" y="126" font-size="10" fill="currentColor">outlet</text>
      <text x="508" y="138" font-size="10" fill="#c0392b" font-weight="700">CLOSED</text>
      <!-- piston (raised high) -->
      <rect x="442" y="120" width="56" height="12" rx="2" fill="#2774AE" fill-opacity="0.7" stroke="currentColor"/>
      <!-- chamber refilling -->
      <rect x="442" y="180" width="56" height="42" fill="#00A6D6" fill-opacity="0.28"/>
      <!-- spring extended -->
      <polyline points="460,150 480,153 460,158 480,163 460,168 480,173 460,178" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <!-- inlet ball valve OPEN (lifted) -->
      <path d="M458,246 L482,246 L470,232 Z" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <circle cx="470" cy="228" r="6" fill="#2774AE" fill-opacity="0.85"/>
      <text x="405" y="250" font-size="10" fill="currentColor" text-anchor="middle">inlet ball</text>
      <text x="405" y="262" font-size="10" fill="#2774AE" text-anchor="middle" font-weight="700">OPEN</text>
      <!-- liquid rising up dip tube -->
      <rect x="463" y="240" width="14" height="86" fill="none" stroke="currentColor" stroke-width="1.5"/>
      <line x1="470" y1="322" x2="470" y2="250" stroke="#00A6D6" stroke-width="3" marker-end="url(#pumpblue)"/>
      <rect x="405" y="326" width="130" height="44" fill="#00A6D6" fill-opacity="0.28" stroke="currentColor"/>
      <text x="470" y="352" font-size="10" fill="currentColor" text-anchor="middle">air pressure pushes liquid up</text>
    </svg>
    <figcaption>Two one-way valves + a spring. Pressing forces liquid out the top; releasing sucks
    a fresh dose up from the bottle. The same design (a reciprocating piston pump) scales all the way
    up to the pumps in your car and home.</figcaption>
  </figure>
</div>

<!-- ============================================================ -->
<h2 class="section-title" id="bike">3 · Why doesn't a moving bicycle fall over?</h2>

<div class="feature">
  <h3>🚲 It's steering, not (mostly) gyroscopes</h3>

  <div class="myth-real">
    <div class="myth">
      <h4>❌ The popular story</h4>
      <p>"The spinning wheels act like gyroscopes — conservation of angular momentum keeps the bike
      upright."</p>
    </div>
    <div class="real">
      <h4>✅ What's really true</h4>
      <p>The dominant effect is <strong>steering into the fall</strong>: whenever the bike leans, the
      front wheel turns toward the lean, curving the path so the wheels swing back under the center
      of mass. Gyroscopic and geometric effects help, but they aren't the whole story.</p>
    </div>
  </div>

  <p>Balancing a bike is a feedback-control problem. Start to tip right, and — whether by your hands
  or by the bike's own geometry — the front wheel steers slightly right. That makes the bike follow a
  curved path; the resulting sideways (centripetal) acceleration whips the contact patch back
  underneath your center of mass, standing you up again. You do this constantly with tiny corrections
  you barely notice. It's the same trick as balancing a broom on your palm by moving your hand under
  it. (It's also why turning at speed starts with a quick <em>counter-steer</em> — a brief nudge of
  the bars the "wrong" way to make the bike lean into the turn.)</p>

  <p>What makes a <em>riderless</em> bike coast upright on its own is a blend of three ingredients:
  <strong>trail</strong> (the front contact point sits behind the steering axis, like a shopping-cart
  caster, so it self-centers and steers into a lean), <strong>gyroscopic precession</strong> of the
  front wheel (a lean torque makes a spinning wheel steer, not just topple), and <strong>mass
  distribution</strong> (a front assembly weighted low and forward falls faster than the frame,
  auto-steering into the lean). A widely cited 2011 <em>Science</em> study built a bike with
  counter-spinning wheels (cancelling the gyro effect) and negative trail that was <em>still</em>
  self-stable — proving no single one of these is essential. Balance is an emergent, whole-machine
  property.</p>

  <figure class="diagram">
    <svg viewBox="0 0 640 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="A leaning bicycle steers into the fall; inset shows steering trail">
      <defs>
        <marker id="bikeink" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="currentColor"/></marker>
        <marker id="bikeblue" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="#2774AE"/></marker>
        <marker id="bikegold" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="#FFB81C"/></marker>
      </defs>
      <!-- ground -->
      <line x1="30" y1="235" x2="380" y2="235" stroke="currentColor" stroke-width="1.5"/>
      <!-- rear-view leaning bike (a tilted frame + CoM) -->
      <g transform="rotate(14 200 235)">
        <line x1="200" y1="235" x2="200" y2="120" stroke="currentColor" stroke-width="3"/>
        <circle cx="200" cy="105" r="16" fill="#2774AE" fill-opacity="0.6" stroke="currentColor"/>
        <text x="200" y="110" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">CoM</text>
        <ellipse cx="200" cy="235" rx="10" ry="26" fill="none" stroke="currentColor" stroke-width="3"/>
      </g>
      <!-- gravity pulling CoM sideways (tip direction) -->
      <line x1="228" y1="95" x2="270" y2="110" stroke="#c0392b" stroke-width="2.5" marker-end="url(#bikeink)"/>
      <text x="250" y="88" font-size="11" fill="#c0392b" font-weight="700">starts to fall →</text>
      <!-- corrective curved path -->
      <path d="M120,270 q120,-30 210,10" fill="none" stroke="#2774AE" stroke-width="2.5" stroke-dasharray="7 5" marker-end="url(#bikeblue)"/>
      <text x="150" y="292" font-size="11" fill="#2774AE" font-weight="700">front wheel steers into the lean → path curves back under CoM</text>

      <!-- divider -->
      <line x1="410" y1="30" x2="410" y2="270" stroke="currentColor" stroke-width="1" opacity="0.2"/>
      <!-- Trail inset -->
      <text x="525" y="40" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">Trail (the caster effect)</text>
      <line x1="470" y1="230" x2="590" y2="230" stroke="currentColor" stroke-width="1.5"/>
      <!-- steering axis (tilted) -->
      <line x1="560" y1="70" x2="505" y2="230" stroke="#2774AE" stroke-width="2" stroke-dasharray="5 4"/>
      <text x="575" y="70" font-size="10" fill="#2774AE">steering axis</text>
      <!-- fork + wheel -->
      <line x1="555" y1="95" x2="545" y2="185" stroke="currentColor" stroke-width="3"/>
      <circle cx="545" cy="200" r="30" fill="none" stroke="currentColor" stroke-width="3"/>
      <!-- axis hits ground ahead of contact -->
      <circle cx="505" cy="230" r="3.5" fill="#2774AE"/>
      <circle cx="545" cy="230" r="3.5" fill="#c0392b"/>
      <line x1="505" y1="245" x2="545" y2="245" stroke="#FFB81C" stroke-width="2.5" marker-end="url(#bikegold)"/>
      <line x1="545" y1="245" x2="505" y2="245" stroke="#FFB81C" stroke-width="2.5" marker-end="url(#bikegold)"/>
      <text x="525" y="262" font-size="10" fill="currentColor" text-anchor="middle">trail</text>
      <text x="525" y="285" font-size="9.5" fill="currentColor" text-anchor="middle" opacity="0.8">contact point trails behind → self-centering</text>
    </svg>
    <figcaption>Lean → steer into the lean → curved path pulls the wheels back under you. The front
    wheel's "trail" (its ground contact sitting behind where the steering axis meets the road) makes
    this happen automatically, the way a caster wheel straightens itself out.</figcaption>
  </figure>
</div>

<!-- ============================================================ -->
<h2 class="section-title" id="flight">4 · How does a plane fly — and how is a bird different?</h2>

<div class="feature">
  <h3>✈️ Fixed wings + separate thrust</h3>
  <p>A wing generates <strong>lift</strong> by throwing air downward. Two equivalent pictures describe
  it: (1) <em>Newton</em> — the wing's shape and tilt (angle of attack) deflect the oncoming air
  downward, and the reaction pushes the wing up; (2) <em>pressure</em> — air moving faster over the
  curved top has lower pressure than the slower air underneath, and that pressure difference sums to
  an upward force. Both are the same physics seen from two angles. (The old "the top is longer so air
  must speed up to meet at the back" story is a <strong>myth</strong> — the flows don't have to meet,
  and wings fly upside-down just fine.) Lift scales as:</p>

  <div class="eq">
    \( L = \tfrac{1}{2}\,\rho\, v^2\, S\, C_L \)
    <span class="eq-note">ρ = air density, v = airspeed, S = wing area, C<sub>L</sub> = lift
    coefficient (grows with angle of attack, until the wing stalls)</span>
  </div>

  <p>An airplane splits the job in two: the <strong>engines</strong> supply forward thrust to keep
  the airspeed <em>v</em> high, and the <strong>fixed wings</strong> turn that airspeed into lift.
  Steady, efficient, and simple — but only because there's a motor doing the pushing.</p>

  <h3>🦅 A bird's wing does both jobs at once</h3>
  <p>A bird (or bat, or insect) has no separate engine. Its flapping wing is
  <strong>lift and thrust in one</strong>: on the downstroke the wing pushes air down <em>and</em>
  back, so the reaction has both an upward component (lift) and a forward one (thrust). The wing also
  <em>twists</em> through the stroke to hold a useful angle of attack, and morphs its shape — folding
  on the upstroke to cut drag. Small flyers go further still: at their size, air feels "syrupy" (low
  Reynolds number), so insects and hummingbirds exploit <strong>unsteady aerodynamics</strong> —
  leading-edge vortices, "clap-and-fling," and rotational lift — tricks a fixed wing can't use. So the
  headline difference is <em>integration and motion</em>: a plane = rigid wing + separate thrust; an
  animal = one flexible, oscillating wing that produces both, often with cleverer, unsteady airflow.</p>

  <figure class="diagram">
    <svg viewBox="0 0 640 300" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Airfoil streamlines and forces, with a flapping bird wing inset">
      <defs>
        <marker id="airred" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="#c0392b"/></marker>
        <marker id="airblue" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="#2774AE"/></marker>
        <marker id="airink" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="currentColor"/></marker>
        <marker id="airgold" markerWidth="10" markerHeight="10" refX="6" refY="3" orient="auto"><path d="M0,0 L8,3 L0,6 Z" fill="#FFB81C"/></marker>
      </defs>
      <!-- airfoil (tilted teardrop) -->
      <g transform="rotate(-10 190 160)">
        <path d="M110,160 Q170,128 265,152 Q200,162 110,160 Z" fill="#2774AE" fill-opacity="0.55" stroke="currentColor" stroke-width="1.5"/>
      </g>
      <!-- streamlines over top (closer = faster/low P) -->
      <path d="M60,120 Q160,96 300,126" fill="none" stroke="#2774AE" stroke-width="1.6" marker-end="url(#airblue)"/>
      <path d="M60,134 Q160,112 300,140" fill="none" stroke="#2774AE" stroke-width="1.6" marker-end="url(#airblue)"/>
      <text x="150" y="92" font-size="10" fill="#2774AE" font-weight="700">faster air · LOW pressure</text>
      <!-- streamlines below (farther = slower/high P) -->
      <path d="M60,190 Q170,196 300,196" fill="none" stroke="currentColor" stroke-width="1.4" opacity="0.7"/>
      <text x="150" y="214" font-size="10" fill="currentColor" opacity="0.8">slower air · HIGH pressure</text>
      <!-- downwash -->
      <path d="M270,150 q40,10 55,45" fill="none" stroke="#c0392b" stroke-width="2.2" marker-end="url(#airred)"/>
      <text x="315" y="205" font-size="10" fill="#c0392b" font-weight="700">downwash</text>
      <!-- lift arrow -->
      <line x1="185" y1="150" x2="185" y2="70" stroke="currentColor" stroke-width="2.6" marker-end="url(#airink)"/>
      <text x="192" y="76" font-size="11" fill="currentColor" font-weight="700">lift</text>
      <!-- thrust / drag -->
      <line x1="150" y1="245" x2="230" y2="245" stroke="#FFB81C" stroke-width="2.6" marker-end="url(#airgold)"/>
      <text x="235" y="249" font-size="10" fill="currentColor">thrust (engine)</text>

      <!-- divider -->
      <line x1="400" y1="30" x2="400" y2="270" stroke="currentColor" stroke-width="1" opacity="0.2"/>
      <!-- bird flap inset -->
      <text x="520" y="40" font-size="12" fill="currentColor" text-anchor="middle" font-weight="700">Bird: one wing, both jobs</text>
      <circle cx="520" cy="120" r="10" fill="#2774AE" fill-opacity="0.6" stroke="currentColor"/>
      <!-- downstroke wing -->
      <path d="M520,120 Q470,140 445,175" fill="none" stroke="currentColor" stroke-width="3"/>
      <path d="M520,120 Q570,140 595,175" fill="none" stroke="currentColor" stroke-width="3"/>
      <!-- downstroke motion arrow -->
      <line x1="460" y1="150" x2="475" y2="195" stroke="#c0392b" stroke-width="2.4" marker-end="url(#airred)"/>
      <text x="430" y="210" font-size="10" fill="#c0392b" font-weight="700">downstroke pushes air down + back</text>
      <!-- resulting lift+thrust -->
      <line x1="520" y1="115" x2="520" y2="70" stroke="currentColor" stroke-width="2.4" marker-end="url(#airink)"/>
      <line x1="522" y1="118" x2="560" y2="100" stroke="#FFB81C" stroke-width="2.4" marker-end="url(#airgold)"/>
      <text x="520" y="64" font-size="10" fill="currentColor">lift</text>
      <text x="565" y="98" font-size="10" fill="currentColor">+ thrust</text>
      <text x="520" y="250" font-size="9.5" fill="currentColor" text-anchor="middle" opacity="0.85">wing twists &amp; morphs each stroke</text>
    </svg>
    <figcaption>Left: a wing deflects air down (Newton) which is the same as a top-vs-bottom pressure
    difference (Bernoulli). Right: a flapping wing angles its downstroke to make lift and thrust
    together — no separate engine needed.</figcaption>
  </figure>
</div>

<!-- ============================================================ -->
<h2 class="section-title" id="fridge">5 · Why won't my cold food box (or fridge door) reopen?</h2>

<div class="feature">
  <h3>🧊 A gentle vacuum, courtesy of the ideal gas law</h3>
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
      <!-- LEFT: warm, just sealed -->
      <text x="160" y="30" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Just sealed · warm (25 °C)</text>
      <rect x="90" y="90" width="140" height="120" rx="6" fill="none" stroke="currentColor" stroke-width="2"/>
      <rect x="82" y="78" width="156" height="16" rx="4" fill="#2774AE" fill-opacity="0.5" stroke="currentColor"/>
      <text x="160" y="72" font-size="10" fill="currentColor" text-anchor="middle">lid (loose)</text>
      <!-- spread-out molecules -->
      <g fill="#c0392b">
        <circle cx="118" cy="120" r="4"/><circle cx="160" cy="110" r="4"/><circle cx="205" cy="130" r="4"/>
        <circle cx="130" cy="165" r="4"/><circle cx="185" cy="170" r="4"/><circle cx="150" cy="145" r="4"/>
        <circle cx="200" cy="185" r="4"/><circle cx="110" cy="190" r="4"/>
      </g>
      <text x="160" y="235" font-size="10" fill="currentColor" text-anchor="middle" opacity="0.8">inside pressure = outside</text>

      <!-- arrow -->
      <line x1="270" y1="150" x2="350" y2="150" stroke="currentColor" stroke-width="2.5" marker-end="url(#frink)"/>
      <text x="310" y="140" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">cools</text>

      <!-- RIGHT: cold, lid sucked down -->
      <text x="480" y="30" font-size="13" fill="currentColor" text-anchor="middle" font-weight="700">Cold (5 °C) · lid clamped</text>
      <rect x="410" y="90" width="140" height="120" rx="6" fill="none" stroke="currentColor" stroke-width="2"/>
      <rect x="402" y="86" width="156" height="16" rx="4" fill="#2774AE" fill-opacity="0.75" stroke="currentColor"/>
      <!-- outside pressure arrows pressing down -->
      <line x1="440" y1="64" x2="440" y2="84" stroke="#c0392b" stroke-width="2.4" marker-end="url(#frink)"/>
      <line x1="480" y1="64" x2="480" y2="84" stroke="#c0392b" stroke-width="2.4" marker-end="url(#frink)"/>
      <line x1="520" y1="64" x2="520" y2="84" stroke="#c0392b" stroke-width="2.4" marker-end="url(#frink)"/>
      <text x="480" y="56" font-size="10" fill="#c0392b" text-anchor="middle" font-weight="700">outside air pushes in</text>
      <!-- contracted molecules (clustered low) -->
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
</div>

<!-- ============================================================ -->
<h2 class="section-title" id="bonus">Bonus round: four more everyday mysteries</h2>

<div class="feature">
  <h3>☕ Why a coffee drop dries into a ring</h3>
  <p>A spilled drop of coffee dries darkest at its <em>edge</em>, not the middle — the famous
  "coffee-ring effect." The rim of the drop is pinned to the surface and can't retreat, and liquid
  evaporates fastest there. To replace what's lost, liquid flows outward from the center to the edge,
  carrying the suspended coffee particles with it and stranding them in a ring. It's a headache for
  inkjet printing and coating uniform films — and a neat way to see fluid flow with your own eyes.</p>
  <figure class="diagram">
    <svg viewBox="0 0 560 190" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Coffee ring: outward flow carries particles to the pinned edge">
      <defs><marker id="cofink" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#2774AE"/></marker>
      <marker id="cofred" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c0392b"/></marker></defs>
      <line x1="60" y1="140" x2="500" y2="140" stroke="currentColor" stroke-width="2"/>
      <!-- droplet cross-section -->
      <path d="M150,140 Q280,60 410,140 Z" fill="#2774AE" fill-opacity="0.22" stroke="currentColor" stroke-width="1.5"/>
      <!-- evaporation arrows at edge -->
      <line x1="160" y1="130" x2="140" y2="95" stroke="#c0392b" stroke-width="1.8" marker-end="url(#cofred)"/>
      <line x1="400" y1="130" x2="420" y2="95" stroke="#c0392b" stroke-width="1.8" marker-end="url(#cofred)"/>
      <text x="120" y="88" font-size="10" fill="#c0392b">evap.</text>
      <text x="425" y="88" font-size="10" fill="#c0392b">evap.</text>
      <!-- outward flow -->
      <line x1="270" y1="128" x2="185" y2="132" stroke="#2774AE" stroke-width="2" marker-end="url(#cofink)"/>
      <line x1="290" y1="128" x2="375" y2="132" stroke="#2774AE" stroke-width="2" marker-end="url(#cofink)"/>
      <text x="230" y="118" font-size="10" fill="#2774AE" text-anchor="middle" font-weight="700">flow carries particles out</text>
      <!-- particle piles at edges -->
      <circle cx="155" cy="136" r="4" fill="#3a2b00"/><circle cx="163" cy="139" r="4" fill="#3a2b00"/>
      <circle cx="405" cy="136" r="4" fill="#3a2b00"/><circle cx="397" cy="139" r="4" fill="#3a2b00"/>
      <text x="280" y="175" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">→ dark ring at the pinned edge</text>
    </svg>
    <figcaption>Faster evaporation at the pinned rim drives an outward flow that piles particles up
    around the edge.</figcaption>
  </figure>
</div>

<div class="feature">
  <h3>🍵 Einstein's tea-leaf paradox</h3>
  <p>Stir a cup of tea and the leaves gather in a neat pile at the <em>center</em> of the bottom — not
  flung to the rim as you'd expect. Einstein explained it: spinning liquid piles up slightly at the
  outer wall (higher pressure there), but friction at the bottom slows the fluid near the base, so it
  can't spin fast enough to balance that pressure. The result is a gentle <strong>secondary
  flow</strong> — inward along the bottom, up the middle, out along the top — that sweeps the leaves
  into the center. The same "teacup" secondary flow explains how river bends erode their outer banks,
  and it's used in engineering to separate particles from liquids.</p>
  <figure class="diagram">
    <svg viewBox="0 0 560 200" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Secondary flow in a stirred cup sweeps leaves to the center">
      <defs><marker id="teaink" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#2774AE"/></marker></defs>
      <!-- cup cross-section -->
      <path d="M120,40 L140,170 L420,170 L440,40" fill="#2774AE" fill-opacity="0.12" stroke="currentColor" stroke-width="1.8"/>
      <line x1="120" y1="40" x2="440" y2="40" stroke="currentColor" stroke-width="1.8"/>
      <!-- secondary flow loops (both sides) -->
      <path d="M175,160 Q160,90 275,60 Q400,90 385,160" fill="none" stroke="#2774AE" stroke-width="2" stroke-dasharray="6 4"/>
      <path d="M280,160 L200,163" fill="none" stroke="#2774AE" stroke-width="2.2" marker-end="url(#teaink)"/>
      <path d="M280,160 L360,163" fill="none" stroke="#2774AE" stroke-width="2.2" marker-end="url(#teaink)"/>
      <line x1="280" y1="150" x2="280" y2="80" stroke="#2774AE" stroke-width="2.2" marker-end="url(#teaink)"/>
      <text x="280" y="110" font-size="10" fill="#2774AE" text-anchor="middle" font-weight="700">up the middle</text>
      <text x="280" y="150" font-size="10" fill="#2774AE" text-anchor="middle">inward along the bottom</text>
      <!-- leaf pile -->
      <circle cx="272" cy="166" r="4" fill="#3a2b00"/><circle cx="282" cy="167" r="4" fill="#3a2b00"/><circle cx="290" cy="165" r="4" fill="#3a2b00"/>
      <text x="280" y="192" font-size="11" fill="currentColor" text-anchor="middle" font-weight="700">leaves collect in the center</text>
    </svg>
    <figcaption>Bottom friction breaks the balance between spin and pressure, driving a slow inward
    sweep along the base — right into the center.</figcaption>
  </figure>
</div>

<div class="feature">
  <h3>🚿 Why the shower curtain attacks you</h3>
  <p>Turn on the shower and the curtain billows <em>inward</em>, sticking to your legs. The tidy
  explanation is Bernoulli's principle — the fast-moving air dragged along by the falling water has
  lower pressure, so the higher pressure outside pushes the curtain in. The fuller story is that the
  spray also sets up a slow rotating vortex (a "bathroom buoyancy" plume from warm, humid air rising)
  that lowers the pressure behind the curtain. Either way: lower pressure inside, so the curtain gets
  shoved toward you. A weighted hem or a curtain that curves outward fixes it.</p>
</div>

<div class="feature">
  <h3>🌈 Why the sky is blue (and sunsets are red)</h3>
  <p>Sunlight is a mix of all colors, and air molecules scatter it — but not evenly. This is
  <strong>Rayleigh scattering</strong>, which is dramatically stronger for shorter wavelengths
  (scattering ∝ 1/λ⁴). Blue and violet get bounced around the sky far more than red, so the whole
  daytime sky glows blue (we see blue more than violet partly because the Sun emits less violet and
  our eyes are less sensitive to it). At sunset the light skims through <em>much</em> more atmosphere,
  so nearly all the blue is scattered away before it reaches you — what's left arriving straight from
  the Sun is the leftover red and orange.</p>
  <figure class="diagram">
    <svg viewBox="0 0 560 210" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Rayleigh scattering: blue scatters across the sky, red passes through at sunset">
      <defs><marker id="skyblue" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#00A6D6"/></marker>
      <marker id="skyred" markerWidth="9" markerHeight="9" refX="6" refY="3" orient="auto"><path d="M0,0 L7,3 L0,6 Z" fill="#c0392b"/></marker></defs>
      <!-- atmosphere band -->
      <rect x="40" y="40" width="480" height="130" rx="10" fill="#00A6D6" fill-opacity="0.08" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4"/>
      <text x="55" y="60" font-size="10" fill="currentColor" opacity="0.7">atmosphere (air molecules)</text>
      <!-- incoming sunlight -->
      <line x1="60" y1="80" x2="250" y2="120" stroke="#FFB81C" stroke-width="3"/>
      <text x="70" y="76" font-size="10" fill="currentColor">white sunlight</text>
      <!-- scatter point -->
      <circle cx="250" cy="120" r="4" fill="currentColor"/>
      <!-- blue scattered in many directions -->
      <line x1="250" y1="120" x2="290" y2="70" stroke="#00A6D6" stroke-width="2" marker-end="url(#skyblue)"/>
      <line x1="250" y1="120" x2="210" y2="70" stroke="#00A6D6" stroke-width="2" marker-end="url(#skyblue)"/>
      <line x1="250" y1="120" x2="300" y2="150" stroke="#00A6D6" stroke-width="2" marker-end="url(#skyblue)"/>
      <text x="300" y="60" font-size="10" fill="#00A6D6" font-weight="700">blue scatters everywhere → blue sky</text>
      <!-- red continues -->
      <line x1="250" y1="120" x2="480" y2="150" stroke="#c0392b" stroke-width="3" marker-end="url(#skyred)"/>
      <text x="360" y="180" font-size="10" fill="#c0392b" font-weight="700">red passes through → red sunset</text>
    </svg>
    <figcaption>Short-wavelength blue light scatters strongly in every direction (blue sky); the red
    that survives the long slant through the atmosphere at dusk gives us sunsets.</figcaption>
  </figure>
</div>

<h2 class="section-title">Gallery</h2>

{% include gallery.html folder="/Photos/life-physics" %}

<div class="callout">
  <p>💬 Have an everyday mystery you'd like me to tackle?
  <a href="mailto:wesleywey0717@g.ucla.edu">Send it my way</a> and it might become the next entry.
  Any photos I add to <code>Photos/life-physics/</code> will show up above automatically.</p>
</div>
