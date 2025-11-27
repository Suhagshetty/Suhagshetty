<!-- Donut Chart — Dark Theme (Paste this into your README.md) -->
<div align="center">
  <h3 style="color:#ffffff;margin-bottom:6px">📊 Most Used Languages</h3>
  <p style="color:#9f9f9f;margin-top:0;margin-bottom:12px">Based on public repositories — TypeScript, JavaScript, Java, SQL</p>

  <!-- SVG Donut -->
  <svg
    role="img"
    aria-label="Donut chart showing most used languages: TypeScript 70 percent, JavaScript 20 percent, Java 7 percent, SQL 3 percent"
    viewBox="0 0 420 260"
    width="420"
    height="260"
    style="background:#0D1117; border-radius:12px; padding:12px;"
  >
    <defs>
      <style>
        .label { font: 600 12px/1.2 'Segoe UI', Roboto, system-ui, -apple-system; fill:#bdbdbd; }
        .title { font: 700 14px/1.2 'Segoe UI', Roboto, system-ui, -apple-system; fill:#ffffff; }
        .legend { font: 600 12px/1 'Segoe UI', Roboto, system-ui, -apple-system; fill:#dcdcdc; }
        .percent { font: 700 12px/1 'Segoe UI', Roboto, system-ui, -apple-system; fill:#ffffff; }
        .small { font: 500 11px/1 'Segoe UI', Roboto, system-ui, -apple-system; fill:#9f9f9f; }
      </style>
      <!-- Colors -->
      <linearGradient id="gTs" x1="0" x2="1">
        <stop offset="0" stop-color="#60a5fa" />
        <stop offset="1" stop-color="#3178C6" />
      </linearGradient>
      <linearGradient id="gJs" x1="0" x2="1">
        <stop offset="0" stop-color="#f7df1e" />
        <stop offset="1" stop-color="#e6c220" />
      </linearGradient>
      <linearGradient id="gJava" x1="0" x2="1">
        <stop offset="0" stop-color="#f2994a" />
        <stop offset="1" stop-color="#ED8B00" />
      </linearGradient>
      <linearGradient id="gSql" x1="0" x2="1">
        <stop offset="0" stop-color="#7ee787" />
        <stop offset="1" stop-color="#4DB33D" />
      </linearGradient>
    </defs>

    <!-- Title -->
    <text x="220" y="28" class="title" text-anchor="middle">Most Used Languages — Donut</text>

    <!-- Donut center -->
    <g transform="translate(100,130) rotate(-90)">
      <!-- Circle base -->
      <circle r="72" cx="0" cy="0" fill="none" stroke="#0D1117" stroke-width="36" />

      <!-- Slices: percentages (stroke-dasharray: <part> <rest>) -->
      <!-- Calculation notes: circumference = 2πr ≈ 2 * 3.1416 * 72 ≈ 452.39 -->
      <!-- Values used: TS 70 -> 316.67 ; JS 20 -> 90.48 ; Java 7 -> 31.67 ; SQL 3 -> 13.57 -->

      <!-- TypeScript 70% -->
      <circle r="72" cx="0" cy="0" fill="none" stroke="url(#gTs)" stroke-width="36"
              stroke-dasharray="316.67 135.72" stroke-dashoffset="0" stroke-linecap="round" />

      <!-- JavaScript 20% (offset by 316.67) -->
      <circle r="72" cx="0" cy="0" fill="none" stroke="url(#gJs)" stroke-width="36"
              stroke-dasharray="90.48 361.91" stroke-dashoffset="-316.67" stroke-linecap="round" />

      <!-- Java 7% (offset by 316.67+90.48 = 407.15) -->
      <circle r="72" cx="0" cy="0" fill="none" stroke="url(#gJava)" stroke-width="36"
              stroke-dasharray="31.67 420.72" stroke-dashoffset="-407.15" stroke-linecap="round" />

      <!-- SQL 3% (offset by 407.15+31.67 = 438.82) -->
      <circle r="72" cx="0" cy="0" fill="none" stroke="url(#gSql)" stroke-width="36"
              stroke-dasharray="13.57 438.82" stroke-dashoffset="-438.82" stroke-linecap="round" />
    </g>

    <!-- Inner circle (hole) -->
    <circle cx="100" cy="130" r="44" fill="#0D1117" />

    <!-- Center text: main language -->
    <text x="100" y="125" class="label" text-anchor="middle">Top Language</text>
    <text x="100" y="145" class="percent" text-anchor="middle">TypeScript — 70%</text>

    <!-- Legend -->
    <g transform="translate(210,60)">
      <!-- TypeScript -->
      <rect x="0" y="0" width="16" height="16" rx="3" fill="url(#gTs)"></rect>
      <text x="22" y="13" class="legend">TypeScript</text>
      <text x="120" y="13" class="small">70%</text>

      <!-- JavaScript -->
      <rect x="0" y="28" width="16" height="16" rx="3" fill="url(#gJs)"></rect>
      <text x="22" y="41" class="legend">JavaScript</text>
      <text x="120" y="41" class="small">20%</text>

      <!-- Java -->
      <rect x="0" y="56" width="16" height="16" rx="3" fill="url(#gJava)"></rect>
      <text x="22" y="69" class="legend">Java</text>
      <text x="120" y="69" class="small">7%</text>

      <!-- SQL -->
      <rect x="0" y="84" width="16" height="16" rx="3" fill="url(#gSql)"></rect>
      <text x="22" y="97" class="legend">SQL</text>
      <text x="120" y="97" class="small">3%</text>
    </g>

    <!-- Footer note -->
    <text x="210" y="245" class="small" text-anchor="middle">Data: Public GitHub repositories — approximate distribution</text>
  </svg>
</div>
