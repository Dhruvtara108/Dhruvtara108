<!--
═══════════════════════════════════════════════════════════
  DHRUV — GitHub Profile README
  Pixel Platformer Header · Navy / Black / White Palette
═══════════════════════════════════════════════════════════
-->

<div align="center">

<!-- PIXEL PLATFORMER ANIMATION — no external deps, renders instantly -->
<svg width="100%" viewBox="0 0 900 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="sky" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#000814"/>
      <stop offset="100%" stop-color="#001533"/>
    </linearGradient>
    <filter id="gw">
      <feGaussianBlur stdDeviation="5" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="gws">
      <feGaussianBlur stdDeviation="2" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      /* ── CHARACTER WALK + JUMP ── */
      .char{animation:cm 10s linear infinite;}
      @keyframes cm{
        0%  {transform:translate(-55px,150px);}
        13% {transform:translate(168px,150px);}
        15% {transform:translate(185px,116px);}
        17% {transform:translate(202px,123px);}
        38% {transform:translate(355px,123px);}
        40% {transform:translate(382px,80px);}
        42% {transform:translate(428px,90px);}
        60% {transform:translate(650px,90px);}
        63% {transform:translate(668px,150px);}
        100%{transform:translate(952px,150px);}
      }
      /* ── LEGS alternating step ── */
      .ll{animation:lw .28s steps(2,end) infinite;}
      .rl{animation:lw .28s steps(2,end) infinite .14s;}
      @keyframes lw{from{transform:translateY(0);}to{transform:translateY(4px);}}
      /* ── ENEMY 1 pacing on Platform 1 ── */
      .e1{animation:e1a 2.4s ease-in-out infinite;}
      @keyframes e1a{0%,100%{transform:translate(210px,136px);}50%{transform:translate(248px,136px);}}
      /* ── ENEMY 2 pacing on Platform 2 ── */
      .e2{animation:e2a 2.8s ease-in-out infinite;}
      @keyframes e2a{0%,100%{transform:translate(462px,103px);}50%{transform:translate(516px,103px);}}
      /* ── COIN float ── */
      .coins{animation:cf .9s ease-in-out infinite alternate;}
      @keyframes cf{0%{transform:translateY(0);}100%{transform:translateY(-5px);}}
      /* ── SCAN LINE ── */
      .sc{animation:sl 5s linear infinite;}
      @keyframes sl{from{transform:translateY(-5px);}to{transform:translateY(205px);}}
      /* ── STAR TWINKLE ── */
      .s0{animation:tw 2.1s ease-in-out infinite;}
      .s1{animation:tw 1.8s ease-in-out infinite .45s;}
      .s2{animation:tw 2.4s ease-in-out infinite .9s;}
      .s3{animation:tw 1.6s ease-in-out infinite 1.35s;}
      .s4{animation:tw 2.0s ease-in-out infinite .2s;}
      .s5{animation:tw 2.6s ease-in-out infinite .7s;}
      .s6{animation:tw 1.9s ease-in-out infinite 1.1s;}
      .s7{animation:tw 2.3s ease-in-out infinite 1.7s;}
      @keyframes tw{0%,100%{opacity:.85;}50%{opacity:.04;}}
      /* ── TEXT REVEALS ── */
      .nt{animation:fi .9s ease forwards;}
      .rt{animation:fi .5s ease 1s forwards;opacity:0;}
      .dt{animation:fi .5s ease 1.7s forwards;opacity:0;}
      @keyframes fi{to{opacity:1;}}
      /* ── STATUS PULSE ── */
      .pb{animation:pulse 1.8s ease-in-out infinite;}
      @keyframes pulse{0%,100%{opacity:.35;}50%{opacity:1;}}
      /* ── BRACKET FLICKER ── */
      .br1{animation:bf 2s ease-in-out infinite;}
      .br2{animation:bf 2s ease-in-out infinite 1s;}
      @keyframes bf{0%,100%{opacity:.55;}50%{opacity:.15;}}
      /* ── FLAG WAVE ── */
      .flag{animation:fw 1.2s ease-in-out infinite alternate;}
      @keyframes fw{0%{transform:skewX(0deg);}100%{transform:skewX(-6deg);}}
    </style>
  </defs>

  <!-- ═══ SKY ═══ -->
  <rect width="900" height="200" fill="url(#sky)"/>

  <!-- ═══ SUBTLE SCAN LINE ═══ -->
  <rect class="sc" width="900" height="1.5" y="0" fill="#3b82f6" opacity="0.06"/>

  <!-- ═══ CRESCENT MOON ═══ -->
  <circle cx="838" cy="32" r="16" fill="#dbeafe" opacity="0.88"/>
  <circle cx="845" cy="30" r="14" fill="#000f25" opacity="0.98"/>

  <!-- ═══ STARS ═══ -->
  <rect class="s0" x="42"  y="9"  width="2" height="2" fill="white"/>
  <rect class="s1" x="118" y="21" width="2" height="2" fill="white"/>
  <rect class="s2" x="196" y="8"  width="2" height="2" fill="white"/>
  <rect class="s3" x="342" y="18" width="2" height="2" fill="white"/>
  <rect class="s4" x="494" y="6"  width="2" height="2" fill="white"/>
  <rect class="s5" x="644" y="15" width="2" height="2" fill="white"/>
  <rect class="s6" x="752" y="10" width="2" height="2" fill="white"/>
  <rect class="s7" x="892" y="22" width="2" height="2" fill="white"/>
  <!-- dim 1×1 stars -->
  <rect x="76"  y="30" width="1" height="1" fill="white" opacity="0.4"/>
  <rect x="284" y="13" width="1" height="1" fill="white" opacity="0.35"/>
  <rect x="430" y="25" width="1" height="1" fill="white" opacity="0.45"/>
  <rect x="570" y="8"  width="1" height="1" fill="white" opacity="0.3"/>
  <rect x="714" y="38" width="1" height="1" fill="white" opacity="0.4"/>

  <!-- ═══ DISTANT MOUNTAINS ═══ -->
  <polygon points="0,172   88,96  176,172"  fill="#060e1d" opacity="0.95"/>
  <polygon points="48,172  158,84 268,172"  fill="#091520" opacity="0.9"/>
  <polygon points="376,172 442,120 508,172" fill="#060e1d" opacity="0.85"/>
  <polygon points="685,172 768,90 851,172"  fill="#091520" opacity="0.9"/>
  <polygon points="738,172 822,106 906,172" fill="#060e1d" opacity="0.85"/>

  <!-- ═══ GROUND (surface y=175) ═══ -->
  <rect x="0" y="175" width="900" height="25" fill="#0c1e3d"/>
  <rect x="0" y="175" width="900" height="5"  fill="#1a3575"/>
  <rect x="0" y="175" width="900" height="2"  fill="#2550a0"/>
  <!-- tile dividers every 30px -->
  <rect x="30"  y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="60"  y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="90"  y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="120" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="150" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="180" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="210" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="240" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="270" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="300" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="330" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="360" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="390" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="420" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="450" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="480" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="510" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="540" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="570" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="600" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="630" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="660" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="690" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="720" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="750" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="780" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="810" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="840" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>
  <rect x="870" y="175" width="1" height="9" fill="#081428" opacity="0.9"/>

  <!-- ═══ PLATFORM 1  x=200–370, surface y=148 ═══ -->
  <rect x="200" y="152" width="170" height="10" fill="#0c1e3d"/>
  <rect x="200" y="148" width="170" height="5"  fill="#1a3575"/>
  <rect x="200" y="148" width="170" height="2"  fill="#2550a0"/>
  <!-- bottom shadow -->
  <rect x="203" y="158" width="167" height="2" fill="#040c1a" opacity="0.7"/>
  <!-- tile marks -->
  <rect x="230" y="148" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="260" y="148" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="290" y="148" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="320" y="148" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="350" y="148" width="1" height="8" fill="#081428" opacity="0.9"/>
  <!-- left pillar -->
  <rect x="200" y="160" width="6" height="15" fill="#0e254a"/>
  <rect x="364" y="160" width="6" height="15" fill="#0e254a"/>

  <!-- ═══ PLATFORM 2  x=440–670, surface y=115 ═══ -->
  <rect x="440" y="119" width="230" height="10" fill="#0c1e3d"/>
  <rect x="440" y="115" width="230" height="5"  fill="#1a3575"/>
  <rect x="440" y="115" width="230" height="2"  fill="#2550a0"/>
  <rect x="443" y="125" width="227" height="2" fill="#040c1a" opacity="0.7"/>
  <!-- tile marks -->
  <rect x="470" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="500" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="530" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="560" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="590" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="620" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <rect x="650" y="115" width="1" height="8" fill="#081428" opacity="0.9"/>
  <!-- pillars -->
  <rect x="440" y="127" width="6" height="48" fill="#0e254a"/>
  <rect x="664" y="127" width="6" height="48" fill="#0e254a"/>

  <!-- ═══ ENEMY 1  — blue slime, paces Platform 1 ═══ -->
  <g class="e1">
    <!-- body -->
    <rect x="0" y="0" width="20" height="12" rx="4" fill="#1d4ed8"/>
    <rect x="0" y="0" width="20" height="3"  rx="2" fill="#2563eb" opacity="0.5"/>
    <!-- eyes -->
    <rect x="2" y="3" width="6" height="6" rx="1" fill="white"/>
    <rect x="12" y="3" width="6" height="6" rx="1" fill="white"/>
    <!-- pupils -->
    <rect x="3" y="4" width="3" height="4" fill="#1e3a8a"/>
    <rect x="13" y="4" width="3" height="4" fill="#1e3a8a"/>
    <!-- shine -->
    <rect x="4" y="4" width="1" height="1" fill="white" opacity="0.8"/>
    <rect x="14" y="4" width="1" height="1" fill="white" opacity="0.8"/>
    <!-- antenna -->
    <rect x="8" y="-6" width="3" height="6" fill="#3b82f6"/>
    <rect x="6" y="-9" width="7" height="4" rx="2" fill="#60a5fa"/>
    <rect x="8" y="-8" width="3" height="2" fill="white" opacity="0.5"/>
  </g>

  <!-- ═══ ENEMY 2  — purple slime, paces Platform 2 ═══ -->
  <g class="e2">
    <rect x="0" y="0" width="20" height="12" rx="4" fill="#4c1d95"/>
    <rect x="0" y="0" width="20" height="3"  rx="2" fill="#6d28d9" opacity="0.5"/>
    <rect x="2" y="3" width="6" height="6" rx="1" fill="white"/>
    <rect x="12" y="3" width="6" height="6" rx="1" fill="white"/>
    <rect x="3" y="4" width="3" height="4" fill="#2e1065"/>
    <rect x="13" y="4" width="3" height="4" fill="#2e1065"/>
    <rect x="4" y="4" width="1" height="1" fill="white" opacity="0.8"/>
    <rect x="14" y="4" width="1" height="1" fill="white" opacity="0.8"/>
    <rect x="8" y="-6" width="3" height="6" fill="#7c3aed"/>
    <rect x="6" y="-9" width="7" height="4" rx="2" fill="#a78bfa"/>
    <rect x="8" y="-8" width="3" height="2" fill="white" opacity="0.5"/>
  </g>

  <!-- ═══ COINS above Platform 2 ═══ -->
  <g transform="translate(546,97)">
    <g class="coins">
      <!-- coin 1 -->
      <rect x="0"  y="0" width="9" height="9" rx="2" fill="#93c5fd" stroke="#3b82f6" stroke-width="1.5"/>
      <rect x="3"  y="2" width="3" height="5" fill="#1d4ed8" opacity="0.5"/>
      <!-- coin 2 -->
      <rect x="16" y="0" width="9" height="9" rx="2" fill="#93c5fd" stroke="#3b82f6" stroke-width="1.5"/>
      <rect x="19" y="2" width="3" height="5" fill="#1d4ed8" opacity="0.5"/>
      <!-- coin 3 -->
      <rect x="32" y="0" width="9" height="9" rx="2" fill="#93c5fd" stroke="#3b82f6" stroke-width="1.5"/>
      <rect x="35" y="2" width="3" height="5" fill="#1d4ed8" opacity="0.5"/>
    </g>
  </g>

  <!-- ═══ GROUND PIXEL PROPS ═══ -->
  <!-- rock at x=145 -->
  <rect x="145" y="169" width="14" height="8" rx="1" fill="#0f2855"/>
  <rect x="147" y="167" width="10" height="4" rx="1" fill="#152f68"/>
  <!-- rock at x=730 -->
  <rect x="730" y="170" width="11" height="7" rx="1" fill="#0f2855"/>
  <rect x="732" y="168" width="7" height="3" rx="1" fill="#152f68"/>
  <!-- small gem at x=810 -->
  <polygon points="815,169 819,162 823,169" fill="#3b82f6" opacity="0.8"/>
  <polygon points="815,169 819,166 823,169" fill="#93c5fd" opacity="0.6"/>

  <!-- ═══ GOAL FLAG at x=870 ═══ -->
  <!-- pole -->
  <rect x="868" y="143" width="3" height="32" fill="#1e3a8a"/>
  <!-- flag shape -->
  <g class="flag" style="transform-origin: 871px 143px;">
    <polygon points="871,143 898,152 871,161" fill="#1d4ed8"/>
    <polygon points="871,143 898,152 871,161" fill="#93c5fd" opacity="0.35"/>
  </g>
  <!-- pole base -->
  <rect x="863" y="173" width="14" height="4" rx="1" fill="#1a3575"/>

  <!-- ═══ PLAYER CHARACTER (astronaut-bot, 16w × 25h) ═══ -->
  <g class="char">
    <!-- HELMET -->
    <rect x="1"  y="0"  width="15" height="9"  rx="2" fill="#60a5fa"/>
    <rect x="3"  y="0"  width="10" height="2"  fill="#93c5fd"/>
    <!-- visor -->
    <rect x="3"  y="3"  width="11" height="4"  fill="#1e3a8a"/>
    <!-- visor glare -->
    <rect x="4"  y="3"  width="4"  height="2"  fill="#bfdbfe" opacity="0.55"/>
    <!-- eyes inside visor -->
    <rect x="4"  y="5"  width="3"  height="2"  fill="#93c5fd"/>
    <rect x="10" y="5"  width="3"  height="2"  fill="#93c5fd"/>
    <!-- BODY -->
    <rect x="2"  y="9"  width="13" height="8"  fill="#1d4ed8"/>
    <!-- chest panel -->
    <rect x="5"  y="11" width="7"  height="4"  fill="#1e3a8a"/>
    <rect x="6"  y="12" width="1"  height="2"  fill="#3b82f6"/>
    <rect x="9"  y="12" width="1"  height="2"  fill="#3b82f6"/>
    <rect x="7"  y="11" width="3"  height="1"  fill="#3b82f6" opacity="0.4"/>
    <!-- LEFT ARM -->
    <rect x="0"  y="10" width="3"  height="5"  fill="#1d4ed8"/>
    <rect x="0"  y="14" width="3"  height="2"  fill="#93c5fd"/>
    <!-- RIGHT ARM + TOOL -->
    <rect x="14" y="10" width="3"  height="5"  fill="#1d4ed8"/>
    <rect x="14" y="14" width="4"  height="2"  fill="#60a5fa"/>
    <!-- LEFT LEG (stepped walk animation) -->
    <g class="ll">
      <rect x="2"  y="17" width="5"  height="6"  fill="#1e3a8a"/>
      <rect x="1"  y="21" width="6"  height="3"  fill="#1e40af"/>
    </g>
    <!-- RIGHT LEG -->
    <g class="rl">
      <rect x="10" y="17" width="5"  height="6"  fill="#1e3a8a"/>
      <rect x="9"  y="21" width="6"  height="3"  fill="#1e40af"/>
    </g>
  </g>

  <!-- ═══ DARK OVERLAY behind text area for legibility ═══ -->
  <rect x="0" y="0" width="900" height="92" fill="#000814" opacity="0.42"/>

  <!-- ═══ CORNER BRACKETS ═══ -->
  <path class="br1" d="M18,16 L18,40 M18,16 L42,16" stroke="#3b82f6" stroke-width="1.5" fill="none"/>
  <path class="br2" d="M882,16 L882,40 M882,16 L858,16" stroke="#3b82f6" stroke-width="1.5" fill="none"/>

  <!-- ═══ NAME TEXT ═══ -->
  <text class="nt"
    x="450" y="55"
    text-anchor="middle"
    font-family="'Courier New',Courier,monospace"
    font-size="40" font-weight="bold"
    fill="#ffffff"
    filter="url(#gw)"
    letter-spacing="8">DHRUV</text>

  <!-- Animated underline -->
  <rect x="450" y="62" width="0" height="2" fill="#3b82f6">
    <animate attributeName="width" from="0" to="248" dur="0.7s" begin="0.9s" fill="freeze"/>
    <animate attributeName="x"     from="450" to="326" dur="0.7s" begin="0.9s" fill="freeze"/>
  </rect>

  <!-- ═══ ROLE TEXT ═══ -->
  <text class="rt"
    x="450" y="80"
    text-anchor="middle"
    font-family="'Courier New',Courier,monospace"
    font-size="11" fill="#93c5fd" letter-spacing="2.5">
    SWE  ·  AI SYSTEMS  ·  ROBOTICS  ·  MIT ECOSYSTEM
  </text>

  <!-- ═══ STATUS ═══ -->
  <circle class="pb" cx="295" cy="93" r="4" fill="#3b82f6" filter="url(#gws)"/>
  <text class="dt"
    x="307" y="97"
    font-family="'Courier New',Courier,monospace"
    font-size="10" fill="#60a5fa">OPEN TO OPPORTUNITIES</text>

  <!-- ═══ DUCKIETOWN BADGE (top-right) ═══ -->
  <rect x="715" y="16" width="167" height="22" rx="3" fill="#1e3a8a" opacity="0.25" stroke="#3b82f6" stroke-width="0.6"/>
  <text class="rt"
    x="798" y="31"
    text-anchor="middle"
    font-family="'Courier New',Courier,monospace"
    font-size="9" fill="#93c5fd" letter-spacing="0.5">@ DUCKIETOWN · MIT ECOSYSTEM</text>
</svg>

<br/>

<!-- BADGES -->
![Profile Views](https://komarev.com/ghpvc/?username=Dhruvtara108&color=1d4ed8&style=for-the-badge&label=PROFILE+VIEWS&labelColor=0f172a)
[![LinkedIn](https://img.shields.io/badge/5K%2B_FOLLOWERS-LinkedIn-1d4ed8?style=for-the-badge&logo=linkedin&logoColor=93c5fd&labelColor=0f172a)](https://www.linkedin.com/in/dhruv-01352a279/)
[![GitHub](https://img.shields.io/badge/GITHUB-Dhruvtara108-1d4ed8?style=for-the-badge&logo=github&logoColor=93c5fd&labelColor=0f172a)](https://github.com/Dhruvtara108)
[![Email](https://img.shields.io/badge/EMAIL-Contact-1d4ed8?style=for-the-badge&logo=gmail&logoColor=93c5fd&labelColor=0f172a)](mailto:mishradhruv257@gmail.com)

</div>

---

<div align="center">

## ✦ ABOUT ME ✦

</div>

```python
class Dhruv:
    def __init__(self):
        self.name        = "Dhruv"
        self.role        = "Software Engineer · AI/Robotics Researcher · Builder"
        self.university  = "KIIT University — B.Tech CSE (2023–Present)"
        self.location    = "India 🇮🇳  →  Building Globally"
        self.email       = "mishradhruv257@gmail.com"
        self.linkedin    = "linkedin.com/in/dhruv-01352a279"
        self.github      = "github.com/Dhruvtara108"

    @property
    def currently(self):
        return [
            "🤖  SWE Intern @ Duckietown Robotics — MIT ecosystem, Cambridge MA",
            "🔬  ML Research Collaborator — LLM memorization & privacy-preserving systems",
            "📡  Building Professor Dashboard — live robot data, APIs, visualization",
            "🏆  Team Lead — RoboNexus World Championship (CTF Track) · KFUPM",
            "🚀  TinyFish Accelerator — accepted, building agentic AI systems",
        ]

    @property
    def research_interests(self):
        return [
            "🦾  Autonomous Robotics & Embedded Systems",
            "🧠  Agentic AI & Intelligent Automation",
            "⚡  AI-Driven Backend Architectures",
            "📊  ML Systems · LLM Research · Privacy-Preserving AI",
        ]

    @property
    def i_build_with(self):
        return {
            "hardware" : ["Arduino", "Raspberry Pi", "Sensors", "Fusion 360"],
            "ai_ml"    : ["YOLOv8", "OpenCV", "TensorFlow Lite", "PyTorch", "Agentic AI"],
            "backend"  : ["Python", "FastAPI", "ASP.NET Core", "Node.js", "REST APIs"],
            "frontend" : ["React 19", "Flutter", "HTML/CSS", "Shadcn UI"],
            "data"     : ["SQL Server", "MongoDB", "Google BigQuery"],
            "systems"  : ["ROS", "Linux/Ubuntu", "Docker", "GCP", "Git"],
        }
```

---

<div align="center">

## ✦ 2026 ACHIEVEMENTS ✦

</div>

```
╔══════════════════════════════════════════════════════════════════════════╗
║                                                                          ║
║   🤖  Duckietown Robotics (MIT ecosystem, Cambridge MA)                  ║
║       Software Engineering Intern · Mar 2026 – Present                  ║
║       ROS · Docker · Linux · Python · APIs · Real Robot Data            ║
║                                                                          ║
╠══════════════════════════════════════════════════════════════════════════╣
║                                                                          ║
║   🚀  TinyFish Accelerator — ACCEPTED                                    ║
║       16,500 credits + API access · Building agentic AI systems          ║
║       Los Altos, California · Feb 2026                                   ║
║                                                                          ║
╠══════════════════════════════════════════════════════════════════════════╣
║                                                                          ║
║   🔴  Red Bull Basement '26 — IDEA SELECTED & FUNDED                     ║
║       $1,000 Microsoft Azure Credits · Microsoft for Startups            ║
║       Hardware prototype idea selected · Mar 2026                        ║
║                                                                          ║
╠══════════════════════════════════════════════════════════════════════════╣
║                                                                          ║
║   🏆  RoboNexus World Championship — TEAM LEAD                           ║
║       CTF Track · KFUPM International Robotics · Conditionally Accepted  ║
║       Team: Karn · Competition delayed (regional conflict) · 2026        ║
║                                                                          ║
╠══════════════════════════════════════════════════════════════════════════╣
║                                                                          ║
║   🏥  HSIL Hackathon 2026 — SHORTLISTED                                  ║
║       Harvard T.H. Chan School of Public Health × KIIT-TEC              ║
║       Health Systems Innovation Lab · Apr 2026                           ║
║                                                                          ║
╠══════════════════════════════════════════════════════════════════════════╣
║                                                                          ║
║   🔬  RoSE @ ICSE 2026 — PAPER SUBMITTED & PEER REVIEWED                 ║
║       "Lessons Learned from Real-World Robotic System Deployment"        ║
║       Robot Software Engineering Workshop · Co-located with ICSE 2026   ║
║       3 peer reviews received from intl. robotics researchers            ║
║                                                                          ║
╠══════════════════════════════════════════════════════════════════════════╣
║                                                                          ║
║   🇮🇳  Smart India Hackathon 2025 — NATIONAL ROUND 2                     ║
║       Ministry of Education, Government of India · Oct 2025             ║
║       Top 50 of 250+ teams @ KIIT → Advanced to National Round 2        ║
║       Project: Arogyam — AI Emergency Healthcare Platform                ║
║                                                                          ║
╚══════════════════════════════════════════════════════════════════════════╝
```

---

<div align="center">

## ✦ FEATURED PROJECTS ✦

</div>

<table align="center">
<tr>
<td width="50%" valign="top">

### 🦯 NeuralNav AI — Assistive Navigation
> *Real-time AI navigation for visually impaired*

**Stack:** `YOLOv8` · `OpenCV` · `Arduino Nano` · `TensorFlow Lite` · `Flutter` · `Python`

| Layer | Tech |
|---|---|
| 👁️ Vision | YOLOv8 + OpenCV |
| 🔊 Hardware | Arduino + HC-SR04 |
| 🤖 Fusion | Sensor + AI logic |
| 📱 Mobile | Flutter + TFLite |

> Prototype completed · Real-time tested · Low-cost & scalable

</td>
<td width="50%" valign="top">

### 🧠 NexusHire — AI Hiring Copilot
> *Agentic AI-powered recruitment intelligence*

**Stack:** `FastAPI` · `Python` · `React` · `TinyFish` · `Agentic AI`

| Feature | Status |
|---|---|
| 🎯 Skill Extraction | ✅ Live |
| 📊 GitHub Analysis | ✅ Live |
| 🔐 Authenticity Score | ✅ Live |
| 📈 Analytics Dashboard | ✅ Live |

> Built using TinyFish Accelerator API credits

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏥 Arogyam — AI Healthcare Platform
> *Smart triage, emergency response & diagnosis*

**Stack:** `React` · `Node.js` · `WhatsApp Business API` · `AI/ML`

| Feature | Status |
|---|---|
| 💬 AI Symptom Analysis | ✅ Live |
| 🚨 Emergency Alert <1min | ✅ Live |
| 📷 Image Diagnosis | ✅ Live |
| 🏥 Auto Hospital Alert | ✅ Live |

> 🏆 SIH 2025 — National Round 2

</td>
<td width="50%" valign="top">

### 🤖 Robotics R&D — KIIT Research Centre
> *Hardware robotics built at KSRC lab*

**Stack:** `Arduino` · `Raspberry Pi` · `Python` · `MATLAB` · `Fusion 360`

| Robot | Purpose |
|---|---|
| 🚁 Delivery Bot | Hostel/society delivery |
| 📷 Surveillance Bot | Campus monitoring |
| 🏥 ICU Sanitation Bot | Contactless hospital cleaning |

> ~70% task automation in prototype simulations
> Led 5-person team · Full hardware-software cycle

</td>
</tr>
</table>

---

<div align="center">

## ✦ WORK EXPERIENCE TIMELINE ✦

</div>

```
 2024 ──────────────────────────────────────────────────────────── 2026 →

 [May'24]      [Sep'24]     [May'25]    [Jul'25]    [Jul'25]    [Mar'26]
     │              │            │           │           │           │
 🏭 TATA       🦾 KSRC      ⚡ ASME     🏭 TATA     💰 FAXIS   🤖 DUCK
 STEEL         Robotics     KIIT        STEEL       Fintech    IETOWN
 Data          R&D Lab      EV+Robot    Backend     Full       Robotics
 Analyst       Autonomous   Design &    ASP.NET     Stack      Infra
 Python        Robots       CAD         SQL+GCP     React 19   ROS+APIs
     │              │            │           │           │           │
 EDA &        ~70% Task    ~20% Faster  ~22% Less   ~25%       Professor
 Dashboards   Automation   Prototype    Manual      Faster     Dashboard
                           Cycle        Work        Render     (Live)
```

---

<div align="center">

## ✦ RESEARCH ✦

</div>

| 🔬 Project | 👤 Collaborator | 🏛️ Institution | 📅 Status |
|---|---|---|---|
| LLM Memorization & Privacy-Preserving ML | Postdoctoral ML Researcher | International | 🟢 Active — LOR + Paid Research Referral |
| AI Tool Adoption in Software Dev (Ethics) | Assoc. Prof. Adolfo Neto | UTFPR, Brazil | 🟢 Active — Paper in progress |
| Real-World Robotic System Deployment | Independent | RoSE @ ICSE 2026 | 🟡 Submitted — 3 peer reviews received |

---

<div align="center">

## ✦ TECH ARSENAL ✦

</div>

<table align="center">
<tr>
<td align="center" width="180">

### 💻 Languages
![Python](https://img.shields.io/badge/Python-0f172a?style=for-the-badge&logo=python&logoColor=93c5fd)
![C++](https://img.shields.io/badge/C++-0f172a?style=for-the-badge&logo=cplusplus&logoColor=93c5fd)
![JavaScript](https://img.shields.io/badge/JS-0f172a?style=for-the-badge&logo=javascript&logoColor=93c5fd)
![C#](https://img.shields.io/badge/C%23-0f172a?style=for-the-badge&logo=csharp&logoColor=93c5fd)
![C](https://img.shields.io/badge/C-0f172a?style=for-the-badge&logo=c&logoColor=93c5fd)
![Dart](https://img.shields.io/badge/Dart-0f172a?style=for-the-badge&logo=dart&logoColor=93c5fd)

</td>
<td align="center" width="180">

### ⚙️ Backend
![FastAPI](https://img.shields.io/badge/FastAPI-0f172a?style=for-the-badge&logo=fastapi&logoColor=93c5fd)
![Node.js](https://img.shields.io/badge/Node.js-0f172a?style=for-the-badge&logo=nodedotjs&logoColor=93c5fd)
![ASP.NET](https://img.shields.io/badge/ASP.NET-0f172a?style=for-the-badge&logo=dotnet&logoColor=93c5fd)
![REST](https://img.shields.io/badge/REST_APIs-0f172a?style=for-the-badge&logo=fastapi&logoColor=93c5fd)

</td>
<td align="center" width="180">

### 🌐 Frontend
![React](https://img.shields.io/badge/React_19-0f172a?style=for-the-badge&logo=react&logoColor=93c5fd)
![Flutter](https://img.shields.io/badge/Flutter-0f172a?style=for-the-badge&logo=flutter&logoColor=93c5fd)
![HTML5](https://img.shields.io/badge/HTML5-0f172a?style=for-the-badge&logo=html5&logoColor=93c5fd)
![Shadcn](https://img.shields.io/badge/Shadcn_UI-0f172a?style=for-the-badge&logo=shadcnui&logoColor=93c5fd)

</td>
</tr>
<tr>
<td align="center" width="180">

### 🤖 AI & CV
![YOLOv8](https://img.shields.io/badge/YOLOv8-0f172a?style=for-the-badge&logo=python&logoColor=93c5fd)
![OpenCV](https://img.shields.io/badge/OpenCV-0f172a?style=for-the-badge&logo=opencv&logoColor=93c5fd)
![TFLite](https://img.shields.io/badge/TF_Lite-0f172a?style=for-the-badge&logo=tensorflow&logoColor=93c5fd)
![PyTorch](https://img.shields.io/badge/PyTorch-0f172a?style=for-the-badge&logo=pytorch&logoColor=93c5fd)
![UiPath](https://img.shields.io/badge/UiPath-0f172a?style=for-the-badge&logo=uipath&logoColor=93c5fd)

</td>
<td align="center" width="180">

### 🦾 Robotics
![ROS](https://img.shields.io/badge/ROS-0f172a?style=for-the-badge&logo=ros&logoColor=93c5fd)
![Arduino](https://img.shields.io/badge/Arduino-0f172a?style=for-the-badge&logo=arduino&logoColor=93c5fd)
![RPi](https://img.shields.io/badge/Raspberry_Pi-0f172a?style=for-the-badge&logo=raspberrypi&logoColor=93c5fd)
![Fusion360](https://img.shields.io/badge/Fusion_360-0f172a?style=for-the-badge&logo=autodesk&logoColor=93c5fd)
![Docker](https://img.shields.io/badge/Docker-0f172a?style=for-the-badge&logo=docker&logoColor=93c5fd)

</td>
<td align="center" width="180">

### ☁️ Cloud & Data
![GCP](https://img.shields.io/badge/GCP-0f172a?style=for-the-badge&logo=googlecloud&logoColor=93c5fd)
![BigQuery](https://img.shields.io/badge/BigQuery-0f172a?style=for-the-badge&logo=googlebigquery&logoColor=93c5fd)
![MongoDB](https://img.shields.io/badge/MongoDB-0f172a?style=for-the-badge&logo=mongodb&logoColor=93c5fd)
![SQL](https://img.shields.io/badge/SQL_Server-0f172a?style=for-the-badge&logo=microsoftsqlserver&logoColor=93c5fd)
![Linux](https://img.shields.io/badge/Linux-0f172a?style=for-the-badge&logo=linux&logoColor=93c5fd)

</td>
</tr>
</table>

---

<div align="center">

## ✦ CS FOUNDATIONS ✦

`Data Structures & Algorithms` &nbsp;·&nbsp; `OOP` &nbsp;·&nbsp; `DBMS` &nbsp;·&nbsp; `Operating Systems` &nbsp;·&nbsp; `Computer Networks` &nbsp;·&nbsp; `System Design` &nbsp;·&nbsp; `Compiler Design` &nbsp;·&nbsp; `Computer Architecture`

</div>

---

<div align="center">

## ✦ CONNECT ✦

[![Email](https://img.shields.io/badge/mishradhruv257%40gmail.com-0f172a?style=for-the-badge&logo=gmail&logoColor=93c5fd)](mailto:mishradhruv257@gmail.com)
[![LinkedIn](https://img.shields.io/badge/5K%2B_Followers_·_LinkedIn-0f172a?style=for-the-badge&logo=linkedin&logoColor=93c5fd)](https://www.linkedin.com/in/dhruv-01352a279/)
[![GitHub](https://img.shields.io/badge/Dhruvtara108_·_GitHub-0f172a?style=for-the-badge&logo=github&logoColor=93c5fd)](https://github.com/Dhruvtara108)

<br/>

```
> Shipping AI + Robotics from India 🇮🇳
> Building at the intersection of Software · AI · Robotics · ML
> Open to: SWE roles · Robotics Engineering · Research collaborations
```

</div>
