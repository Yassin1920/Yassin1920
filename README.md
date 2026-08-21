<svg width="1200" height="320" viewBox="0 0 1200 320" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0a0e14"/>
      <stop offset="55%" stop-color="#0d1b22"/>
      <stop offset="100%" stop-color="#0a0e14"/>
    </linearGradient>
    <linearGradient id="accent" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#8BC7CA" stop-opacity="0"/>
      <stop offset="50%" stop-color="#8BC7CA" stop-opacity="1"/>
      <stop offset="100%" stop-color="#8BC7CA" stop-opacity="0"/>
    </linearGradient>
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#8BC7CA" stroke-opacity="0.06" stroke-width="1"/>
    </pattern>
  </defs>

  <rect width="1200" height="320" fill="url(#bg)"/>
  <rect width="1200" height="320" fill="url(#grid)"/>

  <!-- corner brackets -->
  <g stroke="#8BC7CA" stroke-width="2" fill="none" opacity="0.65">
    <path d="M 30 20 L 30 50 M 30 20 L 60 20"/>
    <path d="M 1170 20 L 1170 50 M 1170 20 L 1140 20"/>
    <path d="M 30 300 L 30 270 M 30 300 L 60 300"/>
    <path d="M 1170 300 L 1170 270 M 1170 300 L 1140 300"/>
  </g>

  <!-- eyebrow -->
  <text x="600" y="88" font-family="'JetBrains Mono', 'Courier New', monospace" font-size="14" letter-spacing="6" fill="#8BC7CA" text-anchor="middle" opacity="0.85">FULL&#160;STACK&#160;DEVELOPER</text>

  <!-- name -->
  <text x="600" y="160" font-family="'Segoe UI', Arial, sans-serif" font-size="56" font-weight="700" fill="#eef4f4" text-anchor="middle" letter-spacing="1">Abed Mouhamed Yassin</text>

  <!-- accent rule -->
  <rect x="450" y="188" width="300" height="2" fill="url(#accent)"/>

  <!-- tagline -->
  <text x="600" y="224" font-family="'JetBrains Mono', 'Courier New', monospace" font-size="15" fill="#9fb4b6" text-anchor="middle" opacity="0.9">Laravel&#160;&#183;&#160;Symfony&#160;&#183;&#160;React&#160;&#183;&#160;PHP&#160;&#183;&#160;MySQL</text>

  <!-- stack pills -->
  <g font-family="'JetBrains Mono', 'Courier New', monospace" font-size="12" fill="#8BC7CA">
    <g transform="translate(600,258)">
      <g transform="translate(-330,0)">
        <rect x="-42" y="-16" width="84" height="26" rx="13" fill="none" stroke="#8BC7CA" stroke-opacity="0.4"/>
        <text x="0" y="2" text-anchor="middle">BACKEND</text>
      </g>
      <g transform="translate(-140,0)">
        <rect x="-46" y="-16" width="92" height="26" rx="13" fill="none" stroke="#8BC7CA" stroke-opacity="0.4"/>
        <text x="0" y="2" text-anchor="middle">FRONTEND</text>
      </g>
      <g transform="translate(60,0)">
        <rect x="-52" y="-16" width="104" height="26" rx="13" fill="none" stroke="#8BC7CA" stroke-opacity="0.4"/>
        <text x="0" y="2" text-anchor="middle">DATABASES</text>
      </g>
      <g transform="translate(280,0)">
        <rect x="-58" y="-16" width="116" height="26" rx="13" fill="none" stroke="#8BC7CA" stroke-opacity="0.4"/>
        <text x="0" y="2" text-anchor="middle">SYSTEM DESIGN</text>
      </g>
    </g>
  </g>
</svg>
