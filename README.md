<div align="center">

<!-- ═══ HEADER SVG ═══ -->
<svg width="900" height="320" viewBox="0 0 900 320" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="hdrGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#000000"/>
      <stop offset="35%" style="stop-color:#000d1a"/>
      <stop offset="65%" style="stop-color:#001433"/>
      <stop offset="100%" style="stop-color:#000000"/>
    </linearGradient>
    <filter id="neonGlow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes waveAnim {
        0%,100% { d: path("M0,260 Q225,230 450,260 Q675,290 900,260 L900,320 L0,320 Z"); }
        50%      { d: path("M0,260 Q225,290 450,260 Q675,230 900,260 L900,320 L0,320 Z"); }
      }
      @keyframes fadeInUp {
        from { opacity:0; transform:translateY(20px); }
        to   { opacity:1; transform:translateY(0); }
      }
      @keyframes neonPulse {
        0%,100% { filter:drop-shadow(0 0 6px #4FC3F7) drop-shadow(0 0 12px #00E5FF); }
        50%     { filter:drop-shadow(0 0 14px #4FC3F7) drop-shadow(0 0 28px #00E5FF); }
      }
      @keyframes scanline {
        0%   { transform:translateY(-100%); }
        100% { transform:translateY(900%); }
      }
      .title { animation: fadeInUp 1.2s ease forwards, neonPulse 3s ease-in-out infinite; }
      .wave  { animation: waveAnim 4s ease-in-out infinite; }
      .scan  { animation: scanline 6s linear infinite; opacity:0.04; }
    </style>
  </defs>
  <rect width="900" height="320" fill="url(#hdrGrad)"/>
  <!-- scanline effect -->
  <rect class="scan" x="0" y="0" width="900" height="18" fill="#4FC3F7"/>
  <!-- grid lines -->
  <g stroke="#4FC3F7" stroke-width="0.3" opacity="0.07">
    <line x1="0" y1="40"  x2="900" y2="40"/>
    <line x1="0" y1="80"  x2="900" y2="80"/>
    <line x1="0" y1="120" x2="900" y2="120"/>
    <line x1="0" y1="160" x2="900" y2="160"/>
    <line x1="0" y1="200" x2="900" y2="200"/>
    <line x1="0" y1="240" x2="900" y2="240"/>
    <line x1="150" y1="0" x2="150" y2="320"/>
    <line x1="300" y1="0" x2="300" y2="320"/>
    <line x1="450" y1="0" x2="450" y2="320"/>
    <line x1="600" y1="0" x2="600" y2="320"/>
    <line x1="750" y1="0" x2="750" y2="320"/>
  </g>
  <!-- corner brackets -->
  <g stroke="#00E5FF" stroke-width="2" fill="none" opacity="0.8">
    <polyline points="10,30 10,10 30,10"/>
    <polyline points="870,10 890,10 890,30"/>
    <polyline points="10,290 10,310 30,310"/>
    <polyline points="870,310 890,310 890,290"/>
  </g>
  <!-- wave bottom -->
  <path class="wave" d="M0,260 Q225,230 450,260 Q675,290 900,260 L900,320 L0,320 Z" fill="#000d1a" opacity="0.6"/>
  <!-- main title -->
  <text class="title" x="450" y="130" text-anchor="middle" font-family="monospace" font-size="68" font-weight="bold" fill="#4FC3F7" filter="url(#neonGlow)">HIMANSHU OS</text>
  <!-- subtitle -->
  <text x="450" y="168" text-anchor="middle" font-family="monospace" font-size="13" fill="#00E5FF" opacity="0.9" filter="url(#softGlow)">◈  HYPEROS v5.0  —  NEXT GEN DEVELOPER ENVIRONMENT  ◈</text>
  <!-- bottom label -->
  <text x="450" y="300" text-anchor="middle" font-family="monospace" font-size="10" fill="#4FC3F7" opacity="0.6">[ SYSTEM ARMED · NODE: EARTH-01 · CLEARANCE: LEVEL 5 ]</text>
</svg>

<br/>

<!-- ═══ BOOT SEQUENCE SVG ═══ -->
<svg width="900" height="230" viewBox="0 0 900 230" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes bootLine {
        0%   { opacity:0; transform:translateX(-10px); }
        100% { opacity:1; transform:translateX(0); }
      }
      @keyframes barFill { from { width:0; } to { width:var(--w); } }
      @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }
      .bl1  { animation: bootLine .4s .1s both; }
      .bl2  { animation: bootLine .4s .5s both; }
      .bl3  { animation: bootLine .4s .9s both; }
      .bl4  { animation: bootLine .4s 1.3s both; }
      .bl5  { animation: bootLine .4s 1.7s both; }
      .bl6  { animation: bootLine .4s 2.1s both; }
      .bl7  { animation: bootLine .4s 2.5s both; }
      .bl8  { animation: bootLine .4s 2.9s both; }
      .bl9  { animation: bootLine .4s 3.3s both; }
      .bl10 { animation: bootLine .4s 3.7s both; }
      .cursor { animation: blink 1s infinite; }
    </style>
  </defs>
  <rect width="900" height="230" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="898" height="228" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.4"/>
  <!-- title bar -->
  <rect x="0" y="0" width="900" height="24" fill="#001433" rx="8"/>
  <circle cx="16" cy="12" r="5" fill="#ff5f57"/>
  <circle cx="32" cy="12" r="5" fill="#febc2e"/>
  <circle cx="48" cy="12" r="5" fill="#28c840"/>
  <text x="450" y="16" text-anchor="middle" font-family="monospace" font-size="10" fill="#4FC3F7">HYPEROS v5.0 — BOOT TERMINAL</text>
  <!-- boot lines -->
  <g font-family="monospace" font-size="12" fill="#4FC3F7">
    <text class="bl1"  x="20" y="50">  <tspan fill="#00E5FF">███</tspan> HYPEROS BOOT SEQUENCE INITIATED <tspan fill="#00E5FF">███</tspan></text>
    <text class="bl2"  x="20" y="68">  [BIOS]   Checking hardware integrity.............. <tspan fill="#00E676">OK ✓</tspan></text>
    <text class="bl3"  x="20" y="86">  [KERNEL] Loading core modules... <tspan fill="#00E676">██████████</tspan> 100%</text>
    <text class="bl4"  x="20" y="104"> [SYSTEM] Mounting developer profile............... <tspan fill="#00E676">DONE ✓</tspan></text>
    <text class="bl5"  x="20" y="122"> [NET]    Uplink established — Signal 100%......... <tspan fill="#00E676">✓</tspan></text>
    <text class="bl6"  x="20" y="140"> [SEC]    Clearance Level 5 — ACCESS GRANTED........ <tspan fill="#FFD700">🔓</tspan></text>
    <text class="bl7"  x="20" y="158"> [AI]     Neural interface......................... <tspan fill="#7C4DFF">SYNCHRONIZED</tspan></text>
    <text class="bl8"  x="20" y="176"> [ENV]    Full Stack environment................... <tspan fill="#FF6D00">ARMED 🚀</tspan></text>
    <text class="bl9"  x="20" y="194"> [SYS]    All systems nominal — LIFTOFF READY...... <tspan fill="#00E676">✓</tspan></text>
    <text class="bl10" x="20" y="212"> <tspan fill="#00E5FF">&gt;&gt;&gt;</tspan> WELCOME TO HIMANSHU OS — HYPEROS v5.0 <tspan class="cursor" fill="#4FC3F7">█</tspan></text>
  </g>
</svg>

<br/>

<!-- ═══ STATUS BADGES SVG ═══ -->
<svg width="860" height="44" viewBox="0 0 860 44" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes badgePulse {
        0%,100% { filter:drop-shadow(0 0 3px currentColor); }
        50%     { filter:drop-shadow(0 0 10px currentColor); }
      }
      .badge { animation: badgePulse 2.5s ease-in-out infinite; }
    </style>
  </defs>
  <!-- SYSTEM ONLINE -->
  <g class="badge" color="#00E5FF">
    <rect x="0"   y="4" width="148" height="36" rx="6" fill="#000d1a" stroke="#00E5FF" stroke-width="1.2"/>
    <circle cx="18" cy="22" r="5" fill="#00E5FF"><animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/></circle>
    <text x="30" y="18" font-family="monospace" font-size="9" fill="#888">SYSTEM</text>
    <text x="30" y="32" font-family="monospace" font-size="11" font-weight="bold" fill="#00E5FF">ONLINE</text>
  </g>
  <!-- KERNEL -->
  <g class="badge" color="#4FC3F7">
    <rect x="158" y="4" width="130" height="36" rx="6" fill="#000d1a" stroke="#4FC3F7" stroke-width="1.2"/>
    <text x="172" y="18" font-family="monospace" font-size="9" fill="#888">KERNEL</text>
    <text x="172" y="32" font-family="monospace" font-size="11" font-weight="bold" fill="#4FC3F7">v5.0</text>
  </g>
  <!-- UPTIME -->
  <g class="badge" color="#00E676">
    <rect x="298" y="4" width="148" height="36" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
    <text x="312" y="18" font-family="monospace" font-size="9" fill="#888">⚡ UPTIME</text>
    <text x="312" y="32" font-family="monospace" font-size="11" font-weight="bold" fill="#00E676">4+ YEARS</text>
  </g>
  <!-- TELEMETRY -->
  <g class="badge" color="#7C4DFF">
    <rect x="456" y="4" width="168" height="36" rx="6" fill="#000d1a" stroke="#7C4DFF" stroke-width="1.2"/>
    <text x="470" y="18" font-family="monospace" font-size="9" fill="#888">🛰 TELEMETRY</text>
    <text x="470" y="32" font-family="monospace" font-size="11" font-weight="bold" fill="#7C4DFF">NOMINAL</text>
  </g>
  <!-- OPEN TO WORK -->
  <g class="badge" color="#00E676">
    <rect x="634" y="4" width="186" height="36" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
    <circle cx="652" cy="22" r="5" fill="#00E676"><animate attributeName="r" values="5;7;5" dur="1.8s" repeatCount="indefinite"/><animate attributeName="opacity" values="1;0.4;1" dur="1.8s" repeatCount="indefinite"/></circle>
    <text x="664" y="18" font-family="monospace" font-size="9" fill="#888">🚀 STATUS</text>
    <text x="664" y="32" font-family="monospace" font-size="10" font-weight="bold" fill="#00E676">OPEN TO WORK</text>
  </g>
</svg>

<br/><br/>

<!-- ═══ TELEMETRY TICKER SVG ═══ -->
<svg width="900" height="32" viewBox="0 0 900 32" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes ticker {
        0%   { transform: translateX(900px); }
        100% { transform: translateX(-1800px); }
      }
      .tick { animation: ticker 18s linear infinite; }
    </style>
  </defs>
  <rect width="900" height="32" fill="#000d1a" rx="4"/>
  <rect x="0" y="0" width="900" height="32" fill="none" stroke="#4FC3F7" stroke-width="0.5" rx="4" opacity="0.3"/>
  <clipPath id="tickClip"><rect width="900" height="32"/></clipPath>
  <g clip-path="url(#tickClip)">
    <text class="tick" y="21" font-family="monospace" font-size="12" fill="#00E5FF">
      [HYPEROS] ▰▰▰▰▰  Signal 100%  •  3 Active Missions  •  0 Failed  •  Uptime 4+ Years  •  Node: Earth-01  •  Stack: PHP | JS | SQL | C++ | HTML | CSS  ▰▰▰▰▰  [HYPEROS]
    </text>
  </g>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    IDENTITY MODULE                             -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes lineExpand { from{width:0} to{width:280px} }
      .lline { animation: lineExpand 1.5s ease forwards; }
    </style>
  </defs>
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <rect class="lline" x="10" y="15" height="1" fill="#00E5FF" opacity="0.5"/>
  <rect class="lline" x="410" y="15" height="1" fill="#00E5FF" opacity="0.5"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ HYPEROS ▶ IDENTITY.exe — DECRYPTING... CLEARANCE LEVEL 5 ]</text>
</svg>

<br/>

<!-- ═══ ASCII NAME BANNER SVG ═══ -->
<svg width="860" height="130" viewBox="0 0 860 130" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <filter id="nameGlow">
      <feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes nameReveal { from{opacity:0;letter-spacing:20px} to{opacity:1;letter-spacing:0} }
      @keyframes borderAnim {
        0%,100%{stroke:#4FC3F7} 33%{stroke:#00E5FF} 66%{stroke:#7C4DFF}
      }
      .namebox { animation: borderAnim 4s linear infinite; }
      .nametxt { animation: nameReveal 1.5s ease forwards; }
    </style>
  </defs>
  <rect width="860" height="130" fill="#000d1a" rx="6"/>
  <rect class="namebox" x="2" y="2" width="856" height="126" fill="none" stroke="#4FC3F7" stroke-width="1.5" rx="6"/>
  <g font-family="monospace" font-size="11" fill="#4FC3F7" filter="url(#nameGlow)">
    <text class="nametxt" x="50" y="28">██╗  ██╗██╗███╗   ███╗ █████╗ ███╗  ██╗███████╗██╗  ██╗██╗   ██╗</text>
    <text class="nametxt" x="50" y="44">██║  ██║██║████╗ ████║██╔══██╗████╗ ██║██╔════╝██║  ██║██║   ██║</text>
    <text class="nametxt" x="50" y="60">███████║██║██╔████╔██║███████║██╔██╗██║███████╗███████║██║   ██║</text>
    <text class="nametxt" x="50" y="76">██╔══██║██║██║╚██╔╝██║██╔══██║██║╚████║╚════██║██╔══██║██║   ██║</text>
    <text class="nametxt" x="50" y="92">██║  ██║██║██║ ╚═╝ ██║██║  ██║██║ ╚███║███████║██║  ██║╚██████╔╝</text>
    <text class="nametxt" x="50" y="108">╚═╝  ╚═╝╚═╝╚═╝     ╚═╝╚═╝  ╚═╝╚═╝  ╚══╝╚══════╝╚═╝  ╚═╝ ╚═════╝</text>
  </g>
  <text x="430" y="124" text-anchor="middle" font-family="monospace" font-size="10" fill="#00E5FF" opacity="0.8">◈  CALLSIGN: himanshu9682  ◈  NODE: EARTH-01  ◈  STATUS: ONLINE  ◈</text>
</svg>

<br/>

<!-- ═══ PROFILE CARDS SVG ═══ -->
<svg width="860" height="90" viewBox="0 0 860 90" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes cardGlow {
        0%,100%{opacity:0.6} 50%{opacity:1}
      }
      @keyframes pulseCircle {
        0%{r:5;opacity:1} 100%{r:12;opacity:0}
      }
      .card { animation: cardGlow 3s ease-in-out infinite; }
    </style>
  </defs>
  <!-- Card 1: Profile -->
  <rect x="0"   y="0" width="200" height="88" rx="8" fill="#000d1a" stroke="#4FC3F7" stroke-width="1.2"/>
  <text x="100" y="22" text-anchor="middle" font-family="monospace" font-size="10" fill="#4FC3F7">🖥️ PROFILE</text>
  <text x="100" y="42" text-anchor="middle" font-family="monospace" font-size="12" font-weight="bold" fill="#4FC3F7">HIMANSHU VERMA</text>
  <text x="100" y="60" text-anchor="middle" font-family="monospace" font-size="10" fill="#90caf9">Full Stack Dev</text>
  <text x="100" y="76" text-anchor="middle" font-family="monospace" font-size="9" fill="#4FC3F7" opacity="0.5">himanshu9682</text>
  <!-- Card 2: Status -->
  <rect x="220" y="0" width="200" height="88" rx="8" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
  <circle cx="270" cy="22" r="5" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="1.4s" repeatCount="indefinite"/></circle>
  <circle cx="270" cy="22" r="5" fill="none" stroke="#00E676"><animate attributeName="r" values="5;14;5" dur="1.4s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0;0.8" dur="1.4s" repeatCount="indefinite"/></circle>
  <text x="320" y="26" text-anchor="middle" font-family="monospace" font-size="10" fill="#00E676">🟢 STATUS</text>
  <text x="320" y="48" text-anchor="middle" font-family="monospace" font-size="13" font-weight="bold" fill="#00E676">● ONLINE</text>
  <text x="320" y="66" text-anchor="middle" font-family="monospace" font-size="10" fill="#00E676">OPEN TO WORK</text>
  <text x="320" y="80" text-anchor="middle" font-family="monospace" font-size="9" fill="#00E676" opacity="0.5">DEPLOY READY 🚀</text>
  <!-- Card 3: Memory -->
  <rect x="440" y="0" width="200" height="88" rx="8" fill="#000d1a" stroke="#7C4DFF" stroke-width="1.2"/>
  <text x="540" y="22" text-anchor="middle" font-family="monospace" font-size="10" fill="#7C4DFF">🧠 MEMORY</text>
  <text x="540" y="48" text-anchor="middle" font-family="monospace" font-size="22" font-weight="bold" fill="#7C4DFF">~4 YRS</text>
  <text x="540" y="66" text-anchor="middle" font-family="monospace" font-size="10" fill="#90caf9">EXPERIENCE</text>
  <text x="540" y="80" text-anchor="middle" font-family="monospace" font-size="9" fill="#7C4DFF" opacity="0.5">UPTIME: 100%</text>
  <!-- Card 4: Node -->
  <rect x="660" y="0" width="200" height="88" rx="8" fill="#000d1a" stroke="#FF6D00" stroke-width="1.2"/>
  <text x="760" y="22" text-anchor="middle" font-family="monospace" font-size="10" fill="#FF6D00">🌐 NODE</text>
  <text x="760" y="46" text-anchor="middle" font-family="monospace" font-size="13" font-weight="bold" fill="#FF6D00">NOIDA, INDIA</text>
  <text x="760" y="64" text-anchor="middle" font-family="monospace" font-size="11" fill="#FF6D00">EARTH-01</text>
  <text x="760" y="80" text-anchor="middle" font-family="monospace" font-size="9" fill="#FF6D00" opacity="0.5">UTC+5:30</text>
</svg>

<br/>

<!-- ═══ TELEMETRY ANIMATED SVG ═══ -->
<svg width="860" height="52" viewBox="0 0 860 52" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes typeRow {
        0%  {opacity:0} 33% {opacity:1} 66% {opacity:1} 100%{opacity:0}
      }
      .tr1{animation:typeRow 6s 0s infinite}
      .tr2{animation:typeRow 6s 2s infinite}
      .tr3{animation:typeRow 6s 4s infinite}
    </style>
  </defs>
  <rect width="860" height="52" fill="#000d1a" rx="4"/>
  <text class="tr1" x="430" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#4FC3F7">[TELEMETRY] Stack: PHP | JS | SQL | C++ | HTML5 | CSS3  ✓</text>
  <text class="tr2" x="430" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#4FC3F7">[TELEMETRY] Platforms: 3 LIVE / 0 DOWN  •  Mission Duration: ~4 Years  ✓</text>
  <text class="tr3" x="430" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#4FC3F7">[TELEMETRY] Objective: OPEN TO WORK ▶  Awaiting Transmission...</text>
  <text x="430" y="42" text-anchor="middle" font-family="monospace" font-size="10" fill="#00E5FF" opacity="0.5">[ SIGNAL: 100% · PACKET LOSS: 0% · LATENCY: 1ms ]</text>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    MISSION PROFILE                             -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ FLIGHT COMPUTER — DECRYPTING ASTRONAUT FILE v5.0... ]</text>
</svg>

</div>

<br/>

```js
// ╔══════════════════════════════════════════════════════════════════════╗
// ║   HYPEROS v5.0  ◈  MISSION CONTROL — ASTRONAUT FILE                 ║
// ║   CLEARANCE : LEVEL 5 — FULL ACCESS GRANTED  🔓                     ║
// ╚══════════════════════════════════════════════════════════════════════╝

const HIMANSHU_OS = {
  callsign    : "himanshu9682",
  name        : "Himanshu Verma",
  role        : "Full Stack Web Developer",
  base        : "Noida, India 🌍",
  uptime      : "~4 years",

  stack : {
    languages  : ["PHP", "JavaScript", "C++", "HTML5", "CSS3", "Oracle SQL"],
    tools      : ["VS Code", "GitHub", "Figma", "JIRA"],
    objectives : ["Scalable Web Apps", "Back-End Architecture", "DB Design"],
  },

  activeMissions : ["prepHQ ◉ LIVE", "The IoT Academy ◉ LIVE", "upSkill Campus ◉ LIVE"],
  deployStatus   : "OPEN_TO_DEPLOY → true 🚀",

  boot : () => {
    console.log("◈ ══════════ HYPEROS v5.0 ONLINE ══════════ ◈");
    console.log("▶  ALL SYSTEMS NOMINAL — INITIATING LAUNCH...");
    console.log("🚀 T-MINUS ZERO — LIFTOFF CONFIRMED.");
  }
};

HIMANSHU_OS.boot();
// ◈ ══════════ HYPEROS v5.0 ONLINE ══════════ ◈
// ▶  ALL SYSTEMS NOMINAL — INITIATING LAUNCH...
// 🚀 T-MINUS ZERO — LIFTOFF CONFIRMED.
```

<br/>

<div align="center">

<!-- ═══ ANIMATED TERMINAL SVG ═══ -->
<svg width="860" height="240" viewBox="0 0 860 240" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes termLine {
        0%  {opacity:0;transform:translateX(-8px)}
        100%{opacity:1;transform:translateX(0)}
      }
      @keyframes curBlink{0%,100%{opacity:1}50%{opacity:0}}
      .tl1 {animation:termLine .35s .2s both}
      .tl2 {animation:termLine .35s .7s both}
      .tl3 {animation:termLine .35s 1.0s both}
      .tl4 {animation:termLine .35s 1.3s both}
      .tl5 {animation:termLine .35s 1.6s both}
      .tl6 {animation:termLine .35s 1.9s both}
      .tl7 {animation:termLine .35s 2.2s both}
      .tl8 {animation:termLine .35s 2.5s both}
      .tl9 {animation:termLine .35s 2.8s both}
      .tl10{animation:termLine .35s 3.1s both}
      .tl11{animation:termLine .35s 3.4s both}
      .tcur{animation:curBlink 1s infinite}
    </style>
  </defs>
  <rect width="860" height="240" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="858" height="238" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.5"/>
  <!-- title bar -->
  <rect x="0" y="0" width="860" height="26" fill="#001433" rx="8"/>
  <circle cx="16" cy="13" r="5" fill="#ff5f57"/>
  <circle cx="32" cy="13" r="5" fill="#febc2e"/>
  <circle cx="48" cy="13" r="5" fill="#28c840"/>
  <text x="430" y="17" text-anchor="middle" font-family="monospace" font-size="10" fill="#4FC3F7">HIMANSHU OS — HYPEROS v5.0 TERMINAL</text>
  <!-- terminal content -->
  <g font-family="monospace" font-size="12" fill="#4FC3F7">
    <text class="tl1"  x="20" y="52"> <tspan fill="#00E5FF">himanshu@hyperos</tspan><tspan fill="#fff">:</tspan><tspan fill="#7C4DFF">~</tspan><tspan fill="#fff">$</tspan> whoami</text>
    <text class="tl2"  x="20" y="68"> ► Himanshu Verma — Full Stack Web Developer</text>
    <text class="tl3"  x="20" y="90"> <tspan fill="#00E5FF">himanshu@hyperos</tspan><tspan fill="#fff">:</tspan><tspan fill="#7C4DFF">~</tspan><tspan fill="#fff">$</tspan> systemctl status --all</text>
    <text class="tl4"  x="20" y="106"><tspan fill="#28c840">◉</tspan> developer.service  — ACTIVE   [████████████] 100%</text>
    <text class="tl5"  x="20" y="120"><tspan fill="#28c840">◉</tspan> backend.service    — RUNNING  [████████████] 100%</text>
    <text class="tl6"  x="20" y="134"><tspan fill="#28c840">◉</tspan> frontend.service   — RUNNING  [████████████] 100%</text>
    <text class="tl7"  x="20" y="148"><tspan fill="#28c840">◉</tspan> database.service   — ONLINE   [████████████] 100%</text>
    <text class="tl8"  x="20" y="162"><tspan fill="#28c840">◉</tspan> mission.service    — ARMED    [████████████] 100%</text>
    <text class="tl9"  x="20" y="176"><tspan fill="#28c840">◉</tspan> telemetry.service  — NOMINAL  [████████████] 100%</text>
    <text class="tl10" x="20" y="198"> <tspan fill="#00E5FF">himanshu@hyperos</tspan><tspan fill="#fff">:</tspan><tspan fill="#7C4DFF">~</tspan><tspan fill="#fff">$</tspan> uptime --verbose</text>
    <text class="tl11" x="20" y="214"> ► 4+ years active  |  3 missions live  |  0 failures  |  100% uptime</text>
    <text class="tl11" x="20" y="230"> <tspan fill="#00E5FF">himanshu@hyperos</tspan><tspan fill="#fff">:</tspan><tspan fill="#7C4DFF">~</tspan><tspan fill="#fff">$</tspan> <tspan class="tcur" fill="#4FC3F7">█</tspan></text>
  </g>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    SYSTEMS CHECK / TECH STACK                  -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ RUNNING SYSTEMS CHECK — ALL MODULES ]</text>
</svg>

<br/><br/>

<img src="https://skillicons.dev/icons?i=php,js,cpp,html,css,mysql&theme=dark&perline=6"/>

<br/><br/>

<img src="https://skillicons.dev/icons?i=vscode,github,figma,linux&theme=dark&perline=6"/>

<br/><br/>

<!-- ═══ ANIMATED SKILL BARS SVG ═══ -->
<svg width="860" height="260" viewBox="0 0 860 260" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes barGrow95 { from{width:0} to{width:570px} }
      @keyframes barGrow90 { from{width:0} to{width:540px} }
      @keyframes barGrow88 { from{width:0} to{width:528px} }
      @keyframes barGrow75 { from{width:0} to{width:450px} }
      @keyframes labelFade { from{opacity:0} to{opacity:1} }
      .bar95 { animation: barGrow95 1.8s 0.3s ease-out both; }
      .bar90 { animation: barGrow90 1.8s 0.6s ease-out both; }
      .bar88 { animation: barGrow88 1.8s 0.9s ease-out both; }
      .bar90b{ animation: barGrow90 1.8s 1.2s ease-out both; }
      .bar75 { animation: barGrow75 1.8s 1.5s ease-out both; }
      .lbl   { animation: labelFade 0.5s 2.2s both; }
    </style>
    <linearGradient id="barHtml" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#E34F26"/>
      <stop offset="100%" style="stop-color:#FF6D00"/>
    </linearGradient>
    <linearGradient id="barJs" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#F7DF1E"/>
      <stop offset="100%" style="stop-color:#FFD700"/>
    </linearGradient>
    <linearGradient id="barPhp" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#4FC3F7"/>
      <stop offset="100%" style="stop-color:#00E5FF"/>
    </linearGradient>
    <linearGradient id="barSql" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#F80000"/>
      <stop offset="100%" style="stop-color:#FF6D00"/>
    </linearGradient>
    <linearGradient id="barCpp" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00599C"/>
      <stop offset="100%" style="stop-color:#7C4DFF"/>
    </linearGradient>
  </defs>
  <rect width="860" height="260" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="858" height="258" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.4"/>
  <!-- header -->
  <text x="20" y="24" font-family="monospace" font-size="11" fill="#00E5FF">HYPEROS  ▸  root@himanshu:~$ run --systems-check --verbose --realtime</text>
  <line x1="10" y1="32" x2="850" y2="32" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <!-- HTML/CSS -->
  <text x="20"  y="58"  font-family="monospace" font-size="12" fill="#4FC3F7">◈  HTML5 / CSS3</text>
  <rect x="200" y="46" width="600" height="14" rx="3" fill="#001433"/>
  <rect class="bar95" x="200" y="46" height="14" rx="3" fill="url(#barHtml)"/>
  <text class="lbl" x="810" y="58" font-family="monospace" font-size="11" fill="#E34F26">95% EXPERT</text>
  <!-- JS -->
  <text x="20"  y="90"  font-family="monospace" font-size="12" fill="#4FC3F7">◈  JavaScript</text>
  <rect x="200" y="78" width="600" height="14" rx="3" fill="#001433"/>
  <rect class="bar90 " x="200" y="78" height="14" rx="3" fill="url(#barJs)"/>
  <text class="lbl" x="810" y="90" font-family="monospace" font-size="11" fill="#F7DF1E">90% ADV</text>
  <!-- PHP -->
  <text x="20"  y="122" font-family="monospace" font-size="12" fill="#4FC3F7">◈  PHP</text>
  <rect x="200" y="110" width="600" height="14" rx="3" fill="#001433"/>
  <rect class="bar90b" x="200" y="110" height="14" rx="3" fill="url(#barPhp)"/>
  <text class="lbl" x="810" y="122" font-family="monospace" font-size="11" fill="#4FC3F7">90% ADV</text>
  <!-- Oracle SQL -->
  <text x="20"  y="154" font-family="monospace" font-size="12" fill="#4FC3F7">◈  Oracle SQL</text>
  <rect x="200" y="142" width="600" height="14" rx="3" fill="#001433"/>
  <rect class="bar88" x="200" y="142" height="14" rx="3" fill="url(#barSql)"/>
  <text class="lbl" x="810" y="154" font-family="monospace" font-size="11" fill="#F80000">88% ADV</text>
  <!-- C++ -->
  <text x="20"  y="186" font-family="monospace" font-size="12" fill="#4FC3F7">◈  C++</text>
  <rect x="200" y="174" width="600" height="14" rx="3" fill="#001433"/>
  <rect class="bar75" x="200" y="174" height="14" rx="3" fill="url(#barCpp)"/>
  <text class="lbl" x="810" y="186" font-family="monospace" font-size="11" fill="#00599C">75% INT</text>
  <!-- support systems -->
  <line x1="10" y1="200" x2="850" y2="200" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <text x="20"  y="218" font-family="monospace" font-size="11" fill="#90caf9">SUPPORT SYSTEMS ──  ◎ VS Code   ◎ GitHub   ◎ Figma   ◎ JIRA   ◎ Linux</text>
  <line x1="10" y1="228" x2="850" y2="228" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <text x="20"  y="248" font-family="monospace" font-size="11" fill="#00E676">RESULT ──────────────────────── [ ALL SYSTEMS NOMINAL ✓  ARMED 🚀 ]</text>
</svg>

<br/><br/>

<!-- ═══ TECH BADGE ROW SVG ═══ -->
<svg width="860" height="44" viewBox="0 0 860 44" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes techBadge{0%,100%{filter:drop-shadow(0 0 3px #4FC3F7)}50%{filter:drop-shadow(0 0 10px #00E5FF)}}
      .tb{animation:techBadge 2.5s ease-in-out infinite}
    </style>
  </defs>
  <g class="tb">
    <rect x="0"   y="4" width="130" height="36" rx="6" fill="#000d1a" stroke="#4FC3F7" stroke-width="1.2"/>
    <text x="65"  y="18" text-anchor="middle" font-family="monospace" font-size="9"  fill="#888">PHP</text>
    <text x="65"  y="32" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#4FC3F7">90%</text>
  </g>
  <g class="tb">
    <rect x="140" y="4" width="130" height="36" rx="6" fill="#000d1a" stroke="#F7DF1E" stroke-width="1.2"/>
    <text x="205" y="18" text-anchor="middle" font-family="monospace" font-size="9"  fill="#888">JavaScript</text>
    <text x="205" y="32" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#F7DF1E">90%</text>
  </g>
  <g class="tb">
    <rect x="280" y="4" width="160" height="36" rx="6" fill="#000d1a" stroke="#E34F26" stroke-width="1.2"/>
    <text x="360" y="18" text-anchor="middle" font-family="monospace" font-size="9"  fill="#888">HTML5 / CSS3</text>
    <text x="360" y="32" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#E34F26">95%</text>
  </g>
  <g class="tb">
    <rect x="450" y="4" width="160" height="36" rx="6" fill="#000d1a" stroke="#F80000" stroke-width="1.2"/>
    <text x="530" y="18" text-anchor="middle" font-family="monospace" font-size="9"  fill="#888">Oracle SQL</text>
    <text x="530" y="32" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#F80000">88%</text>
  </g>
  <g class="tb">
    <rect x="620" y="4" width="130" height="36" rx="6" fill="#000d1a" stroke="#00599C" stroke-width="1.2"/>
    <text x="685" y="18" text-anchor="middle" font-family="monospace" font-size="9"  fill="#888">C++</text>
    <text x="685" y="32" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#00599C">75%</text>
  </g>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    ACTIVE MISSIONS                             -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ ACTIVE MISSIONS — LIVE STATUS FEED ]</text>
</svg>

<br/><br/>

<!-- ═══ MISSION CARDS SVG ═══ -->
<svg width="860" height="340" viewBox="0 0 860 340" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes missionCard{0%,100%{stroke-opacity:0.5}50%{stroke-opacity:1}}
      @keyframes livePulse{0%{r:5;opacity:1}100%{r:14;opacity:0}}
      @keyframes telBar{from{width:0}to{width:var(--tw)}}
      .mc{animation:missionCard 3s ease-in-out infinite}
      .mc1{animation-delay:0s}
      .mc2{animation-delay:1s}
      .mc3{animation-delay:2s}
      .tb1{animation:telBar 2s 0.5s ease-out both;--tw:380px}
      .tb2{animation:telBar 2s 1.0s ease-out both;--tw:380px}
      .tb3{animation:telBar 2s 1.5s ease-out both;--tw:380px}
    </style>
    <linearGradient id="mGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#00E676;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#4FC3F7;stop-opacity:0.8"/>
    </linearGradient>
  </defs>
  <rect width="860" height="340" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="858" height="338" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.3"/>
  <text x="20" y="24" font-family="monospace" font-size="11" fill="#00E5FF">root@himanshu:~$ mission --list --filter=active --telemetry --realtime</text>
  <line x1="10" y1="32" x2="850" y2="32" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>

  <!-- MISSION 01 -->
  <rect class="mc mc1" x="10" y="40" width="840" height="84" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
  <circle cx="30" cy="60" r="6" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite"/></circle>
  <circle cx="30" cy="60" r="6" fill="none" stroke="#00E676"><animate attributeName="r" values="6;16;6" dur="1.5s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0;0.8" dur="1.5s" repeatCount="indefinite"/></circle>
  <text x="48" y="56" font-family="monospace" font-size="13" font-weight="bold" fill="#00E676">MISSION-01 : prepHQ</text>
  <text x="700" y="56" font-family="monospace" font-size="11" fill="#00E676">[ LIVE 🟢 ]</text>
  <text x="30" y="72" font-family="monospace" font-size="10" fill="#90caf9">├── OBJECTIVE : Tech Interview &amp; Career-Prep Platform  |  SYSTEMS : Full-Stack | LMS Integration</text>
  <text x="30" y="86" font-family="monospace" font-size="10" fill="#90caf9">├── LAUNCH : Feb 2026  |  CREW : UniConverge Technologies</text>
  <text x="30" y="100" font-family="monospace" font-size="10" fill="#4FC3F7">└── TELEMETRY : </text>
  <rect x="140" y="91" width="400" height="10" rx="3" fill="#001433"/>
  <rect class="tb1" x="140" y="91" height="10" rx="3" fill="url(#mGrad)"/>
  <text x="548" y="100" font-family="monospace" font-size="10" fill="#00E676"> NOMINAL ✓</text>

  <!-- MISSION 02 -->
  <rect class="mc mc2" x="10" y="134" width="840" height="84" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
  <circle cx="30" cy="154" r="6" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="1.8s" repeatCount="indefinite"/></circle>
  <circle cx="30" cy="154" r="6" fill="none" stroke="#00E676"><animate attributeName="r" values="6;16;6" dur="1.8s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0;0.8" dur="1.8s" repeatCount="indefinite"/></circle>
  <text x="48" y="150" font-family="monospace" font-size="13" font-weight="bold" fill="#00E676">MISSION-02 : The IoT Academy</text>
  <text x="700" y="150" font-family="monospace" font-size="11" fill="#00E676">[ LIVE 🟢 ]</text>
  <text x="30" y="166" font-family="monospace" font-size="10" fill="#90caf9">├── OBJECTIVE : Ed-Tech | IoT / AI / Embedded Systems  |  SYSTEMS : Full-Stack | Curriculum + LMS + QA</text>
  <text x="30" y="180" font-family="monospace" font-size="10" fill="#90caf9">├── LAUNCH : Nov 2024  |  CREW : UniConverge Technologies</text>
  <text x="30" y="194" font-family="monospace" font-size="10" fill="#4FC3F7">└── TELEMETRY : </text>
  <rect x="140" y="185" width="400" height="10" rx="3" fill="#001433"/>
  <rect class="tb2" x="140" y="185" height="10" rx="3" fill="url(#mGrad)"/>
  <text x="548" y="194" font-family="monospace" font-size="10" fill="#00E676"> NOMINAL ✓</text>

  <!-- MISSION 03 -->
  <rect class="mc mc3" x="10" y="228" width="840" height="84" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
  <circle cx="30" cy="248" r="6" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="2.1s" repeatCount="indefinite"/></circle>
  <circle cx="30" cy="248" r="6" fill="none" stroke="#00E676"><animate attributeName="r" values="6;16;6" dur="2.1s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.8;0;0.8" dur="2.1s" repeatCount="indefinite"/></circle>
  <text x="48" y="244" font-family="monospace" font-size="13" font-weight="bold" fill="#00E676">MISSION-03 : upSkill Campus</text>
  <text x="700" y="244" font-family="monospace" font-size="11" fill="#00E676">[ LIVE 🟢 ]</text>
  <text x="30" y="260" font-family="monospace" font-size="10" fill="#90caf9">├── OBJECTIVE : Career Upskilling | 20+ Courses  |  SYSTEMS : Full-Stack | Internship + Placement Content</text>
  <text x="30" y="274" font-family="monospace" font-size="10" fill="#90caf9">├── LAUNCH : Nov 2024  |  CREW : UniConverge Technologies</text>
  <text x="30" y="288" font-family="monospace" font-size="10" fill="#4FC3F7">└── TELEMETRY : </text>
  <rect x="140" y="279" width="400" height="10" rx="3" fill="#001433"/>
  <rect class="tb3" x="140" y="279" height="10" rx="3" fill="url(#mGrad)"/>
  <text x="548" y="288" font-family="monospace" font-size="10" fill="#00E676"> NOMINAL ✓</text>

  <!-- footer row -->
  <line x1="10" y1="320" x2="850" y2="320" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <text x="430" y="334" text-anchor="middle" font-family="monospace" font-size="11" fill="#00E676">TOTAL : 3 ACTIVE  |  0 ABORTED  |  0 FAILED  |  SUCCESS RATE : 100% 🚀</text>
</svg>

<br/><br/>

<!-- ═══ LIVE BADGE ROW SVG ═══ -->
<svg width="600" height="44" viewBox="0 0 600 44" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes liveBadge{0%,100%{filter:drop-shadow(0 0 4px #00E676)}50%{filter:drop-shadow(0 0 12px #00E676)}}
      .lb{animation:liveBadge 2s ease-in-out infinite}
    </style>
  </defs>
  <g class="lb">
    <rect x="0"   y="4" width="180" height="36" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
    <circle cx="18" cy="22" r="5" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite"/></circle>
    <text x="100" y="26" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#00E676">◉ prepHQ — LIVE</text>
  </g>
  <g class="lb">
    <rect x="200" y="4" width="200" height="36" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
    <circle cx="218" cy="22" r="5" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="1.8s" repeatCount="indefinite"/></circle>
    <text x="310" y="26" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#00E676">◉ IoT Academy — LIVE</text>
  </g>
  <g class="lb">
    <rect x="420" y="4" width="180" height="36" rx="6" fill="#000d1a" stroke="#00E676" stroke-width="1.2"/>
    <circle cx="438" cy="22" r="5" fill="#00E676"><animate attributeName="opacity" values="1;0.2;1" dur="2.1s" repeatCount="indefinite"/></circle>
    <text x="510" y="26" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#00E676">◉ upSkill — LIVE</text>
  </g>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    MISSION LOG / EXPERIENCE                    -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ MISSION LOG — DECRYPTING FLIGHT HISTORY... ]</text>
</svg>

<br/><br/>

<!-- ═══ EXPERIENCE TIMELINE SVG ═══ -->
<svg width="860" height="310" viewBox="0 0 860 310" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes logReveal{from{opacity:0;transform:translateX(-12px)}to{opacity:1;transform:translateX(0)}}
      @keyframes dotPulse{0%,100%{r:5}50%{r:8}}
      .lr1{animation:logReveal .5s .2s both}
      .lr2{animation:logReveal .5s .7s both}
      .lr3{animation:logReveal .5s 1.2s both}
      .lr4{animation:logReveal .5s 1.7s both}
      .dp{animation:dotPulse 2s ease-in-out infinite}
    </style>
  </defs>
  <rect width="860" height="310" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="858" height="308" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.3"/>
  <text x="20" y="24" font-family="monospace" font-size="11" fill="#00E5FF">root@himanshu:~$ cat /var/log/mission-history.log --decrypt --verbose</text>
  <line x1="10" y1="32" x2="850" y2="32" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <!-- timeline line -->
  <line x1="36" y1="44" x2="36" y2="296" stroke="#4FC3F7" stroke-width="1" opacity="0.3"/>

  <!-- Entry 1 - Active -->
  <circle class="dp" cx="36" cy="56" r="5" fill="#00E676"/>
  <g class="lr1">
    <text x="56" y="52" font-family="monospace" font-size="11" font-weight="bold" fill="#00E676">[T+ 2023-11 → PRESENT ]  UniConverge Technologies · Noida</text>
    <text x="56" y="66" font-family="monospace" font-size="10" fill="#90caf9">╰─ ROLE    : Research, Content &amp; Cross-Functional Lead</text>
    <text x="56" y="78" font-family="monospace" font-size="10" fill="#90caf9">╰─ MISSION : 3 platforms end-to-end (LMS + Web + QA)</text>
    <text x="56" y="90" font-family="monospace" font-size="10" fill="#90caf9">╰─ STACK   : PHP | JavaScript | Oracle SQL</text>
    <text x="56" y="102" font-family="monospace" font-size="10" fill="#00E676">╰─ SIGNAL  : ████████████████████████████ ◉ ACTIVE 🟢</text>
  </g>
  <line x1="10" y1="112" x2="850" y2="112" stroke="#4FC3F7" stroke-width="0.5" opacity="0.2"/>

  <!-- Entry 2 -->
  <circle cx="36" cy="124" r="5" fill="#4FC3F7"/>
  <g class="lr2">
    <text x="56" y="120" font-family="monospace" font-size="11" font-weight="bold" fill="#4FC3F7">[T+ 2023-02 → 2023-10 ]  EPIS Pvt. Ltd.</text>
    <text x="56" y="134" font-family="monospace" font-size="10" fill="#90caf9">╰─ ROLE    : Full-Stack Web Developer</text>
    <text x="56" y="146" font-family="monospace" font-size="10" fill="#90caf9">╰─ MISSION : Scalable back-end systems  |  CREW : 4-member dev squad</text>
    <text x="56" y="158" font-family="monospace" font-size="10" fill="#4FC3F7">╰─ SIGNAL  : ████████████████████████████ ◎ COMPLETED ✓</text>
  </g>
  <line x1="10" y1="168" x2="850" y2="168" stroke="#4FC3F7" stroke-width="0.5" opacity="0.2"/>

  <!-- Entry 3 -->
  <circle cx="36" cy="180" r="5" fill="#4FC3F7"/>
  <g class="lr3">
    <text x="56" y="176" font-family="monospace" font-size="11" font-weight="bold" fill="#4FC3F7">[T+ 2022-10 → 2023-01 ]  Velocity India</text>
    <text x="56" y="190" font-family="monospace" font-size="10" fill="#90caf9">╰─ ROLE    : Web Developer Intern</text>
    <text x="56" y="202" font-family="monospace" font-size="10" fill="#90caf9">╰─ MISSION : Employee Feedback System — Front-End Lead  |  CREW : 8-developer team</text>
    <text x="56" y="214" font-family="monospace" font-size="10" fill="#4FC3F7">╰─ SIGNAL  : ████████████████████████████ ◎ COMPLETED ✓</text>
  </g>
  <line x1="10" y1="224" x2="850" y2="224" stroke="#4FC3F7" stroke-width="0.5" opacity="0.2"/>

  <!-- Entry 4 -->
  <circle cx="36" cy="236" r="5" fill="#4FC3F7"/>
  <g class="lr4">
    <text x="56" y="232" font-family="monospace" font-size="11" font-weight="bold" fill="#4FC3F7">[T+ 2022-07 → 2022-10 ]  Zuxus Business Solution</text>
    <text x="56" y="246" font-family="monospace" font-size="10" fill="#90caf9">╰─ ROLE    : Database Administrator Intern</text>
    <text x="56" y="258" font-family="monospace" font-size="10" fill="#90caf9">╰─ MISSION : DB management &amp; query optimization</text>
    <text x="56" y="270" font-family="monospace" font-size="10" fill="#4FC3F7">╰─ SIGNAL  : ████████████████████████████ ◎ COMPLETED ✓</text>
  </g>
  <line x1="10" y1="282" x2="850" y2="282" stroke="#4FC3F7" stroke-width="0.5" opacity="0.2"/>
  <text x="430" y="298" text-anchor="middle" font-family="monospace" font-size="10" fill="#00E676">TOTAL MISSIONS : 4  |  ACTIVE : 1  |  COMPLETED : 3  |  FAILED : 0  ✓</text>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    FLIGHT DIAGNOSTICS / STATS                  -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ RUNNING FLIGHT DIAGNOSTICS — LIVE DATA FEED ]</text>
</svg>

<br/><br/>

<img src="https://github-readme-stats.vercel.app/api?username=himanshu9682&show_icons=true&hide_border=true&bg_color=000d1a&title_color=00E5FF&icon_color=4FC3F7&text_color=90caf9&ring_color=00E5FF&include_all_commits=true&count_private=true&border_radius=10" height="175"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=himanshu9682&layout=compact&hide_border=true&bg_color=000d1a&title_color=00E5FF&text_color=90caf9&langs_count=8&border_radius=10" height="175"/>

<br/><br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=himanshu9682&hide_border=true&background=000d1a&ring=00E5FF&fire=4FC3F7&currStreakLabel=00E5FF&sideLabels=90caf9&dates=90caf9&currStreakNum=00E5FF&sideNums=4FC3F7&stroke=00E5FF&border_radius=10" width="65%"/>

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=himanshu9682&theme=algolia&no-frame=true&no-bg=true&margin-w=6&column=7"/>

<br/><br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=himanshu9682&bg_color=000d1a&color=00E5FF&line=4FC3F7&point=ffffff&area=true&area_color=001433&hide_border=true&radius=8" width="96%"/>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    CREDENTIALS                                 -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ VERIFYING MISSION CREDENTIALS... CLEARANCE CHECK ]</text>
</svg>

<br/><br/>

<!-- ═══ CREDENTIALS SVG ═══ -->
<svg width="860" height="200" viewBox="0 0 860 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes credReveal{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:translateY(0)}}
      @keyframes verifiedGlow{0%,100%{filter:drop-shadow(0 0 3px #00E676)}50%{filter:drop-shadow(0 0 10px #00E676)}}
      .cr1{animation:credReveal .4s .2s both}
      .cr2{animation:credReveal .4s .5s both}
      .cr3{animation:credReveal .4s .8s both}
      .cr4{animation:credReveal .4s 1.1s both}
      .vg{animation:verifiedGlow 2.5s ease-in-out infinite}
    </style>
  </defs>
  <rect width="860" height="200" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="858" height="198" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.3"/>
  <text x="20" y="24" font-family="monospace" font-size="11" fill="#00E5FF">root@himanshu:~$ cat credentials.json | verify --all --decrypt</text>
  <line x1="10" y1="32" x2="850" y2="32" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>

  <g class="cr1">
    <rect x="10" y="40" width="840" height="30" rx="4" fill="#001433"/>
    <text x="24" y="60" font-family="monospace" font-size="11" fill="#90caf9">"Oracle_DB_11g_RAC"</text>
    <text x="240" y="60" font-family="monospace" font-size="11" fill="#888">: issuer: "Skillsoft"</text>
    <text class="vg" x="680" y="60" font-family="monospace" font-size="11" fill="#00E676">◉ VERIFIED ✓  ACTIVE</text>
  </g>
  <g class="cr2">
    <rect x="10" y="76" width="840" height="30" rx="4" fill="#000d1a"/>
    <text x="24" y="96" font-family="monospace" font-size="11" fill="#90caf9">"JIRA_Project_Mgmt"</text>
    <text x="240" y="96" font-family="monospace" font-size="11" fill="#888">: issuer: "Great Learning"</text>
    <text class="vg" x="680" y="96" font-family="monospace" font-size="11" fill="#00E676">◉ VERIFIED ✓  ACTIVE</text>
  </g>
  <g class="cr3">
    <rect x="10" y="112" width="840" height="30" rx="4" fill="#001433"/>
    <text x="24" y="132" font-family="monospace" font-size="11" fill="#90caf9">"NET_OOPs"</text>
    <text x="240" y="132" font-family="monospace" font-size="11" fill="#888">: issuer: "Great Learning"</text>
    <text class="vg" x="680" y="132" font-family="monospace" font-size="11" fill="#00E676">◉ VERIFIED ✓  ACTIVE</text>
  </g>
  <g class="cr4">
    <rect x="10" y="148" width="840" height="30" rx="4" fill="#000d1a"/>
    <text x="24" y="168" font-family="monospace" font-size="11" fill="#90caf9">"Prompt_Engineering"</text>
    <text x="240" y="168" font-family="monospace" font-size="11" fill="#888">: issuer: "Certified"</text>
    <text class="vg" x="680" y="168" font-family="monospace" font-size="11" fill="#00E676">◉ VERIFIED ✓  ACTIVE</text>
  </g>
  <line x1="10" y1="184" x2="850" y2="184" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <text x="430" y="196" text-anchor="middle" font-family="monospace" font-size="10" fill="#FFD700">▶▶  IDENTITY CONFIRMED — CLEARANCE LEVEL 5 — ALL ACCESS GRANTED 🔓</text>
</svg>

</div>

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!--                    UPLINK / CONTACT                            -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ═══ SECTION HEADER SVG ═══ -->
<svg width="700" height="34" viewBox="0 0 700 34" xmlns="http://www.w3.org/2000/svg">
  <rect width="700" height="34" fill="#000d1a" rx="4"/>
  <text x="350" y="22" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">[ UPLINK ESTABLISHED — TRANSMITTING SIGNAL... ]</text>
</svg>

<br/><br/>

<!-- ═══ CONTACT BUTTONS SVG ═══ -->
<svg width="700" height="56" viewBox="0 0 700 56" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes contactBtn{0%,100%{filter:drop-shadow(0 0 4px #4FC3F7)}50%{filter:drop-shadow(0 0 14px #00E5FF)}}
      .cb{animation:contactBtn 2.5s ease-in-out infinite}
      .cb2{animation:contactBtn 2.5s 0.8s ease-in-out infinite}
      .cb3{animation:contactBtn 2.5s 1.6s ease-in-out infinite}
    </style>
  </defs>
  <a href="mailto:himanshu.hv3992@gmail.com">
    <g class="cb">
      <rect x="0" y="8" width="210" height="40" rx="8" fill="#000d1a" stroke="#EA4335" stroke-width="1.5"/>
      <text x="105" y="24" text-anchor="middle" font-family="monospace" font-size="9" fill="#888">📧 GMAIL</text>
      <text x="105" y="40" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#EA4335">himanshu.hv3992@gmail.com</text>
    </g>
  </a>
  <a href="https://github.com/himanshu9682">
    <g class="cb2">
      <rect x="230" y="8" width="210" height="40" rx="8" fill="#000d1a" stroke="#4FC3F7" stroke-width="1.5"/>
      <text x="335" y="24" text-anchor="middle" font-family="monospace" font-size="9" fill="#888">🐙 GITHUB</text>
      <text x="335" y="40" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#4FC3F7">himanshu9682</text>
    </g>
  </a>
  <a href="https://linkedin.com/in/himanshu9682">
    <g class="cb3">
      <rect x="460" y="8" width="210" height="40" rx="8" fill="#000d1a" stroke="#0A66C2" stroke-width="1.5"/>
      <text x="565" y="24" text-anchor="middle" font-family="monospace" font-size="9" fill="#888">💼 LINKEDIN</text>
      <text x="565" y="40" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#0A66C2">Connect</text>
    </g>
  </a>
</svg>

<br/><br/>

<!-- ═══ UPLINK STATUS SVG ═══ -->
<svg width="700" height="100" viewBox="0 0 700 100" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      @keyframes signalWave{
        0%  {opacity:0;transform:scaleX(0)}
        50% {opacity:1;transform:scaleX(1)}
        100%{opacity:0;transform:scaleX(1)}
      }
      .sw1{animation:signalWave 2s 0.0s ease-in-out infinite}
      .sw2{animation:signalWave 2s 0.4s ease-in-out infinite}
      .sw3{animation:signalWave 2s 0.8s ease-in-out infinite}
    </style>
  </defs>
  <rect width="700" height="100" fill="#000d1a" rx="8"/>
  <rect x="1" y="1" width="698" height="98" fill="none" stroke="#4FC3F7" stroke-width="1" rx="8" opacity="0.3"/>
  <text x="350" y="24" text-anchor="middle" font-family="monospace" font-size="12" fill="#00E5FF">UPLINK : ESTABLISHED ✓</text>
  <text x="350" y="44" text-anchor="middle" font-family="monospace" font-size="11" fill="#4FC3F7">FREQUENCY : himanshu.hv3992@gmail.com</text>
  <text x="350" y="62" text-anchor="middle" font-family="monospace" font-size="11" fill="#90caf9">LATENCY : 1ms  |  PACKET LOSS : 0%  |  SIGNAL : 100%</text>
  <!-- signal bars -->
  <rect class="sw1" x="260" y="74" width="40" height="16" rx="2" fill="#00E676" transform-origin="260 82"/>
  <rect class="sw2" x="320" y="74" width="40" height="16" rx="2" fill="#00E676" transform-origin="320 82"/>
  <rect class="sw3" x="380" y="74" width="40" height="16" rx="2" fill="#00E676" transform-origin="380 82"/>
  <text x="350" y="88" text-anchor="middle" font-family="monospace" font-size="10" fill="#00E676">STATUS : READY TO COLLABORATE — AWAITING TRANSMISSION ▶</text>
</svg>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=himanshu9682&style=for-the-badge&color=00E5FF&labelColor=000d1a&label=PROFILE+VIEWS"/>

<br/><br/>

<!-- ═══ FOOTER SVG ═══ -->
<svg width="900" height="180" viewBox="0 0 900 180" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="footGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#000000"/>
      <stop offset="40%" style="stop-color:#000d1a"/>
      <stop offset="70%" style="stop-color:#001433"/>
      <stop offset="100%" style="stop-color:#000000"/>
    </linearGradient>
    <filter id="footGlow">
      <feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      @keyframes footWave {
        0%,100% { d: path("M0,60 Q225,30 450,60 Q675,90 900,60 L900,0 L0,0 Z"); }
        50%      { d: path("M0,60 Q225,90 450,60 Q675,30 900,60 L900,0 L0,0 Z"); }
      }
      @keyframes footFade{from{opacity:0}to{opacity:1}}
      .fw{animation:footWave 4s ease-in-out infinite}
      .ff{animation:footFade 2s ease forwards}
    </style>
  </defs>
  <rect width="900" height="180" fill="url(#footGrad)"/>
  <path class="fw" d="M0,60 Q225,30 450,60 Q675,90 900,60 L900,0 L0,0 Z" fill="#000d1a" opacity="0.5"/>
  <!-- corner brackets -->
  <g stroke="#00E5FF" stroke-width="1.5" fill="none" opacity="0.6">
    <polyline points="10,20 10,10 20,10"/>
    <polyline points="880,10 890,10 890,20"/>
    <polyline points="10,160 10,170 20,170"/>
    <polyline points="880,170 890,170 890,160"/>
  </g>
  <text class="ff" x="450" y="90" text-anchor="middle" font-family="monospace" font-size="16" font-weight="bold" fill="#00E5FF" filter="url(#footGlow)">◈  MISSION COMPLETE — ALL SYSTEMS NOMINAL  ◈</text>
  <text class="ff" x="450" y="114" text-anchor="middle" font-family="monospace" font-size="12" fill="#4FC3F7">T-PLUS INFINITY — STILL BUILDING 🚀</text>
  <line x1="100" y1="128" x2="800" y2="128" stroke="#4FC3F7" stroke-width="0.5" opacity="0.3"/>
  <text x="450" y="148" text-anchor="middle" font-family="monospace" font-size="10" fill="#4FC3F7" opacity="0.6">HYPEROS v5.0  ·  SESSION TERMINATED  ·  READY FOR NEXT SESSION</text>
</svg>

</div>
