from textwrap import dedent

dark = dedent(r'''
<svg width="1180" height="610" viewBox="0 0 1180 610" fill="none" xmlns="http://www.w3.org/2000/svg">
<defs>
  <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#030712"/>
    <stop offset="100%" stop-color="#0B1220"/>
  </linearGradient>
  <linearGradient id="accent" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#7C3AED">
      <animate attributeName="stop-color" values="#7C3AED;#22D3EE;#10B981;#7C3AED" dur="12s" repeatCount="indefinite"/>
    </stop>
    <stop offset="50%" stop-color="#22D3EE">
      <animate attributeName="stop-color" values="#22D3EE;#10B981;#7C3AED;#22D3EE" dur="12s" repeatCount="indefinite"/>
    </stop>
    <stop offset="100%" stop-color="#10B981">
      <animate attributeName="stop-color" values="#10B981;#7C3AED;#22D3EE;#10B981" dur="12s" repeatCount="indefinite"/>
    </stop>
  </linearGradient>
  <filter id="blur"><feGaussianBlur stdDeviation="40"/></filter>
  <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
    <feGaussianBlur stdDeviation="6" result="b"/>
    <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>
</defs>

<rect width="1180" height="610" rx="34" fill="url(#bg)"/>
<circle cx="180" cy="120" r="120" fill="#7C3AED" opacity=".18" filter="url(#blur)"/>
<circle cx="920" cy="160" r="140" fill="#22D3EE" opacity=".12" filter="url(#blur)"/>
<circle cx="860" cy="500" r="120" fill="#10B981" opacity=".12" filter="url(#blur)"/>

<g opacity=".25">
  <circle cx="120" cy="80" r="2" fill="#fff"><animate attributeName="cy" values="80;70;80" dur="6s" repeatCount="indefinite"/></circle>
  <circle cx="340" cy="220" r="1.5" fill="#fff"><animate attributeName="cy" values="220;210;220" dur="5s" repeatCount="indefinite"/></circle>
  <circle cx="980" cy="120" r="2" fill="#fff"><animate attributeName="cy" values="120;110;120" dur="7s" repeatCount="indefinite"/></circle>
</g>

<g transform="translate(50 55)">
  <rect width="390" height="500" rx="28" fill="#0F172A" fill-opacity=".72" stroke="rgba(255,255,255,.08)"/>
  <g transform="translate(36 70)" filter="url(#glow)">
    <text x="0" y="0" font-family="monospace" font-size="20" fill="url(#accent)">
      <tspan x="0" dy="0" opacity="0">   _____
        <animate attributeName="opacity" from="0" to="1" begin="0s" dur=".3s" fill="freeze"/>
      </tspan>
      <tspan x="0" dy="28" opacity="0">  / ____|
        <animate attributeName="opacity" from="0" to="1" begin=".2s" dur=".3s" fill="freeze"/>
      </tspan>
      <tspan x="0" dy="28" opacity="0"> | (___
        <animate attributeName="opacity" from="0" to="1" begin=".4s" dur=".3s" fill="freeze"/>
      </tspan>
      <tspan x="0" dy="28" opacity="0">  \___ \
        <animate attributeName="opacity" from="0" to="1" begin=".6s" dur=".3s" fill="freeze"/>
      </tspan>
      <tspan x="0" dy="28" opacity="0">  ____) |
        <animate attributeName="opacity" from="0" to="1" begin=".8s" dur=".3s" fill="freeze"/>
      </tspan>
      <tspan x="0" dy="28" opacity="0"> |_____/
        <animate attributeName="opacity" from="0" to="1" begin="1.0s" dur=".3s" fill="freeze"/>
      </tspan>
    </text>
    <rect x="-8" y="-22" width="310" height="210" fill="none" stroke="url(#accent)" opacity=".18"/>
    <rect x="-8" y="-22" width="310" height="8" fill="url(#accent)" opacity=".08">
      <animate attributeName="y" values="-22;180;-22" dur="7s" repeatCount="indefinite"/>
    </rect>
  </g>
</g>

<g transform="translate(470 55)">
  <rect width="660" height="500" rx="28" fill="#0F172A" fill-opacity=".72" stroke="rgba(255,255,255,.08)"/>
  <circle cx="28" cy="28" r="6" fill="#F87171"/>
  <circle cx="48" cy="28" r="6" fill="#FBBF24"/>
  <circle cx="68" cy="28" r="6" fill="#34D399"/>

  <g transform="translate(34 70)">
    <text x="0" y="0" font-family="ui-monospace,monospace" font-size="18" fill="#94A3B8">$ whoami</text>
    <text x="0" y="44" font-family="Inter,Segoe UI,sans-serif" font-size="38" font-weight="700" fill="#F8FAFC">Hi, I'm Sunil Kumar</text>

    <text x="0" y="92" font-family="ui-monospace,monospace" font-size="24" fill="url(#accent)">▶ Full Stack Developer</text>
    <rect x="315" y="72" width="12" height="28" fill="#22D3EE">
      <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
    </rect>

    <g font-family="Inter,Segoe UI,sans-serif" font-size="17" fill="#CBD5E1">
      <text x="0" y="142" opacity="0">📍 Madurai, India<animate attributeName="opacity" from="0" to="1" begin="1.2s" dur=".5s" fill="freeze"/></text>
      <text x="0" y="174" opacity="0">🎓 B.E. CSE Student<animate attributeName="opacity" from="0" to="1" begin="1.5s" dur=".5s" fill="freeze"/></text>
      <text x="0" y="206" opacity="0">🚀 Building NOVA AI &amp; web apps<animate attributeName="opacity" from="0" to="1" begin="1.8s" dur=".5s" fill="freeze"/></text>
      <text x="0" y="238" opacity="0">🌐 Portfolio: invodes.dev<animate attributeName="opacity" from="0" to="1" begin="2.1s" dur=".5s" fill="freeze"/></text>
      <text x="0" y="270" opacity="0">✉️ sunil@example.com<animate attributeName="opacity" from="0" to="1" begin="2.4s" dur=".5s" fill="freeze"/></text>
    </g>

    <text x="0" y="332" font-family="Inter,Segoe UI,sans-serif" font-size="18" font-weight="700" fill="#F8FAFC">Skills</text>

    <g transform="translate(0 350)" font-family="Inter,Segoe UI,sans-serif" font-size="14">
      <g><rect width="88" height="34" rx="17" fill="#111827" stroke="url(#accent)"/><text x="44" y="22" text-anchor="middle" fill="#F8FAFC">React</text></g>
      <g transform="translate(100 0)"><rect width="98" height="34" rx="17" fill="#111827" stroke="url(#accent)"/><text x="49" y="22" text-anchor="middle" fill="#F8FAFC">Node.js</text></g>
      <g transform="translate(210 0)"><rect width="112" height="34" rx="17" fill="#111827" stroke="url(#accent)"/><text x="56" y="22" text-anchor="middle" fill="#F8FAFC">Tailwind</text></g>
      <g transform="translate(334 0)"><rect width="90" height="34" rx="17" fill="#111827" stroke="url(#accent)"/><text x="45" y="22" text-anchor="middle" fill="#F8FAFC">Python</text></g>
      <g transform="translate(436 0)"><rect width="88" height="34" rx="17" fill="#111827" stroke="url(#accent)"/><text x="44" y="22" text-anchor="middle" fill="#F8FAFC">Docker</text></g>
    </g>

    <g transform="translate(0 440)" fill="#94A3B8">
      <circle cx="20" cy="0" r="16" fill="none" stroke="url(#accent)"/>
      <circle cx="80" cy="0" r="16" fill="none" stroke="url(#accent)"/>
      <circle cx="140" cy="0" r="16" fill="none" stroke="url(#accent)"/>
      <circle cx="200" cy="0" r="16" fill="none" stroke="url(#accent)"/>
      <text x="20" y="5" text-anchor="middle" font-size="11">GH</text>
      <text x="80" y="5" text-anchor="middle" font-size="11">IN</text>
      <text x="140" y="5" text-anchor="middle" font-size="11">X</text>
      <text x="200" y="5" text-anchor="middle" font-size="11">WEB</text>
    </g>
  </g>
</g>
</svg>
''').strip()

light = dark.replace('#030712','#FFFFFF').replace('#0B1220','#F1F5F9').replace('#0F172A','#F8FAFC').replace('#F8FAFC','#0F172A',1)

open('/mnt/data/dark.svg','w').write(dark)
open('/mnt/data/light.svg','w').write(light)

print('created', '/mnt/data/dark.svg', '/mnt/data/light.svg')
