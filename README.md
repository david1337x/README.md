<svg width="1100" height="520" viewBox="0 0 1100 520" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Engineering process diagram: idea leads to architecture, then build, which splits into secure and automate, converging on deploy.">
  <title>Engineering Process — Idea to Deploy</title>

  <defs>
    <linearGradient id="bg2" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#050505"/>
      <stop offset="100%" stop-color="#0A1118"/>
    </linearGradient>
    <pattern id="grid2" width="26" height="26" patternUnits="userSpaceOnUse">
      <path d="M 26 0 L 0 0 0 26" fill="none" stroke="#00E5FF" stroke-opacity="0.045" stroke-width="1"/>
    </pattern>
    <marker id="arrow" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
      <path d="M 0 0 L 10 5 L 0 10 z" fill="#00E5FF"/>
    </marker>
    <filter id="nodeGlow" x="-40%" y="-40%" width="180%" height="180%">
      <feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <rect width="1100" height="520" fill="url(#bg2)"/>
  <rect width="1100" height="520" fill="url(#grid2)"/>

  <text x="40" y="44" font-family="'JetBrains Mono', 'Courier New', monospace" font-size="13" letter-spacing="2" fill="#8B949E">11 // SYSTEM ARCHITECTURE</text>
  <line x1="40" y1="58" x2="1060" y2="58" stroke="#00E5FF" stroke-opacity="0.25"/>

  <!-- connective paths, drawn first so nodes sit on top -->
  <g fill="none" stroke="#00E5FF" stroke-width="1.6" stroke-opacity="0.55" marker-end="url(#arrow)">
    <path d="M 550 118 L 550 158" />
    <path d="M 550 216 L 550 256" />
    <path d="M 550 314 L 420 354" />
    <path d="M 550 314 L 680 354" />
    <path d="M 420 412 L 550 452" />
    <path d="M 680 412 L 550 452" />
  </g>

  <!-- animated pulse traveling the spine, decorative signal-flow motion -->
  <circle r="3.4" fill="#00E5FF" filter="url(#nodeGlow)">
    <animateMotion dur="4.2s" repeatCount="indefinite"
      path="M 550 118 L 550 158 L 550 216 L 550 256 L 550 314 L 420 354 L 420 412 L 550 452" />
  </circle>

  <!-- node template applied per stage -->
  <g font-family="'JetBrains Mono', 'Courier New', monospace" text-anchor="middle">

    <!-- IDEA -->
    <g transform="translate(550,88)">
      <rect x="-90" y="-24" width="180" height="48" rx="3" fill="#0A1118" stroke="#8B949E" stroke-opacity="0.6"/>
      <text y="6" font-size="14" letter-spacing="2" fill="#FFFFFF">IDEA</text>
    </g>

    <!-- ARCHITECT -->
    <g transform="translate(550,186)">
      <rect x="-110" y="-24" width="220" height="48" rx="3" fill="#0A1118" stroke="#00E5FF" stroke-opacity="0.7"/>
      <text y="6" font-size="14" letter-spacing="2" fill="#FFFFFF">ARCHITECT</text>
    </g>

    <!-- BUILD -->
    <g transform="translate(550,284)">
      <rect x="-130" y="-28" width="260" height="56" rx="3" fill="#0A1118" stroke="#00E5FF" stroke-opacity="0.9"/>
      <text y="7" font-size="16" letter-spacing="3" fill="#00E5FF">BUILD</text>
    </g>

    <!-- SECURE -->
    <g transform="translate(420,384)">
      <rect x="-100" y="-24" width="200" height="48" rx="3" fill="#0A1118" stroke="#7C3AED" stroke-opacity="0.75"/>
      <text y="6" font-size="14" letter-spacing="2" fill="#FFFFFF">SECURE</text>
    </g>

    <!-- AUTOMATE -->
    <g transform="translate(680,384)">
      <rect x="-100" y="-24" width="200" height="48" rx="3" fill="#0A1118" stroke="#7C3AED" stroke-opacity="0.75"/>
      <text y="6" font-size="14" letter-spacing="2" fill="#FFFFFF">AUTOMATE</text>
    </g>

    <!-- DEPLOY -->
    <g transform="translate(550,482)">
      <rect x="-120" y="-26" width="240" height="52" rx="3" fill="#0A1118" stroke="#00E5FF" stroke-opacity="0.9"/>
      <text y="6" font-size="15" letter-spacing="3" fill="#FFFFFF">DEPLOY</text>
    </g>
  </g>

  <text x="1060" y="510" text-anchor="end" font-family="'JetBrains Mono', 'Courier New', monospace" font-size="10" fill="#8B949E" fill-opacity="0.6">DIAGRAM IS A DESIGN ELEMENT, NOT LIVE TELEMETRY</text>
</svg>
