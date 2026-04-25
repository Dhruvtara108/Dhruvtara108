<!--
═══════════════════════════════════════════════════════════
  DHRUV — GitHub Profile README
  Fast-loading CSS animation header + full 2026 achievements
═══════════════════════════════════════════════════════════
-->

<div align="center">

<!-- FAST-LOADING CSS ANIMATION HEADER via SVG -->
<img width="100%" height="200" src="https://raw.githubusercontent.com/Dhruvtara108/Dhruvtara108/main/header.svg" alt="header" onerror="this.style.display='none'"/>

<!-- FALLBACK ANIMATED SVG — renders instantly, no external deps -->
<svg width="100%" height="180" viewBox="0 0 900 180" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0a0a0a"/>
      <stop offset="100%" style="stop-color:#111827"/>
    </linearGradient>
    <!-- Grid line animation -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#1a2a1a" stroke-width="0.5"/>
    </pattern>
    <!-- Glow filter -->
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glow2">
      <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="180" fill="url(#bg)"/>
  <rect width="900" height="180" fill="url(#grid)" opacity="0.4"/>

  <!-- Animated scan line -->
  <rect width="900" height="1" fill="#00ff41" opacity="0.15">
    <animate attributeName="y" from="0" to="180" dur="3s" repeatCount="indefinite"/>
  </rect>

  <!-- Corner brackets — TL -->
  <path d="M 20 20 L 20 50 M 20 20 L 50 20" stroke="#00ff41" stroke-width="2" fill="none" filter="url(#glow)">
    <animate attributeName="opacity" values="1;0.5;1" dur="2s" repeatCount="indefinite"/>
  </path>
  <!-- TR -->
  <path d="M 880 20 L 880 50 M 880 20 L 850 20" stroke="#00ff41" stroke-width="2" fill="none" filter="url(#glow)">
    <animate attributeName="opacity" values="1;0.5;1" dur="2s" begin="0.5s" repeatCount="indefinite"/>
  </path>
  <!-- BL -->
  <path d="M 20 160 L 20 130 M 20 160 L 50 160" stroke="#00ff41" stroke-width="2" fill="none" filter="url(#glow)">
    <animate attributeName="opacity" values="1;0.5;1" dur="2s" begin="1s" repeatCount="indefinite"/>
  </path>
  <!-- BR -->
  <path d="M 880 160 L 880 130 M 880 160 L 850 160" stroke="#00ff41" stroke-width="2" fill="none" filter="url(#glow)">
    <animate attributeName="opacity" values="1;0.5;1" dur="2s" begin="1.5s" repeatCount="indefinite"/>
  </path>

  <!-- Floating dots — robot/circuit aesthetic -->
  <circle cx="100" cy="90" r="2" fill="#00ff41" opacity="0.6">
    <animate attributeName="cy" values="90;80;90" dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;1;0.6" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="800" cy="90" r="2" fill="#00ff41" opacity="0.6">
    <animate attributeName="cy" values="90;100;90" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="150" cy="50" r="1.5" fill="#00ff41" opacity="0.4">
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="1.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="750" cy="130" r="1.5" fill="#00ff41" opacity="0.4">
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="2.2s" repeatCount="indefinite"/>
  </circle>

  <!-- Circuit lines -->
  <path d="M 80 90 L 120 90 L 120 60 L 160 60" stroke="#00ff41" stroke-width="0.8" fill="none" opacity="0.3">
    <animate attributeName="opacity" values="0.3;0.7;0.3" dur="3s" repeatCount="indefinite"/>
  </path>
  <path d="M 820 90 L 780 90 L 780 120 L 740 120" stroke="#00ff41" stroke-width="0.8" fill="none" opacity="0.3">
    <animate attributeName="opacity" values="0.3;0.7;0.3" dur="3s" begin="1.5s" repeatCount="indefinite"/>
  </path>

  <!-- Main name — with letter-by-letter reveal feel via opacity -->
  <text x="450" y="85" text-anchor="middle" font-family="'Courier New', monospace" font-size="42" font-weight="bold" fill="#ffffff" filter="url(#glow2)" letter-spacing="8">
    DHRUV
    <animate attributeName="opacity" values="0;1" dur="0.8s" fill="freeze"/>
  </text>

  <!-- Green accent line under name -->
  <rect x="320" y="95" width="0" height="2" fill="#00ff41" filter="url(#glow)">
    <animate attributeName="width" from="0" to="260" dur="0.8s" begin="0.8s" fill="freeze"/>
    <animate attributeName="x" from="450" to="320" dur="0.8s" begin="0.8s" fill="freeze"/>
  </rect>

  <!-- Role text -->
  <text x="450" y="125" text-anchor="middle" font-family="'Courier New', monospace" font-size="13" fill="#00ff41" letter-spacing="3" opacity="0">
    SWE · AI SYSTEMS · ROBOTICS RESEARCHER
    <animate attributeName="opacity" values="0;0.9" dur="0.5s" begin="1.2s" fill="freeze"/>
  </text>

  <!-- Status indicator -->
  <circle cx="290" cy="148" r="4" fill="#00ff41" filter="url(#glow)">
    <animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>
  <text x="302" y="152" font-family="'Courier New', monospace" font-size="11" fill="#00ff41" opacity="0">
    OPEN TO OPPORTUNITIES
    <animate attributeName="opacity" values="0;0.8" dur="0.5s" begin="1.6s" fill="freeze"/>
  </text>

  <!-- Duckietown badge top right -->
  <rect x="720" y="20" width="160" height="24" rx="4" fill="#00ff41" opacity="0.1" stroke="#00ff41" stroke-width="0.5"/>
  <text x="800" y="36" text-anchor="middle" font-family="'Courier New', monospace" font-size="10" fill="#00ff41" opacity="0">
    @ DUCKIETOWN · MIT ECOSYSTEM
    <animate attributeName="opacity" values="0;0.9" dur="0.5s" begin="1.4s" fill="freeze"/>
  </text>
</svg>

<br/>

<!-- BADGES -->
![Profile Views](https://komarev.com/ghpvc/?username=Dhruvtara108&color=00ff41&style=for-the-badge&label=PROFILE+VIEWS&labelColor=0a0a0a)
[![LinkedIn](https://img.shields.io/badge/5K%2B_FOLLOWERS-LinkedIn-00ff41?style=for-the-badge&logo=linkedin&logoColor=0a0a0a&labelColor=0a0a0a)](https://www.linkedin.com/in/dhruv-01352a279/)
[![GitHub](https://img.shields.io/badge/GITHUB-Dhruvtara108-00ff41?style=for-the-badge&logo=github&logoColor=0a0a0a&labelColor=0a0a0a)](https://github.com/Dhruvtara108)
[![Email](https://img.shields.io/badge/EMAIL-Contact-00ff41?style=for-the-badge&logo=gmail&logoColor=0a0a0a&labelColor=0a0a0a)](mailto:mishradhruv257@gmail.com)

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
![Python](https://img.shields.io/badge/Python-0a0a0a?style=for-the-badge&logo=python&logoColor=00ff41)
![C++](https://img.shields.io/badge/C++-0a0a0a?style=for-the-badge&logo=cplusplus&logoColor=00ff41)
![JavaScript](https://img.shields.io/badge/JS-0a0a0a?style=for-the-badge&logo=javascript&logoColor=00ff41)
![C#](https://img.shields.io/badge/C%23-0a0a0a?style=for-the-badge&logo=csharp&logoColor=00ff41)
![C](https://img.shields.io/badge/C-0a0a0a?style=for-the-badge&logo=c&logoColor=00ff41)
![Dart](https://img.shields.io/badge/Dart-0a0a0a?style=for-the-badge&logo=dart&logoColor=00ff41)

</td>
<td align="center" width="180">

### ⚙️ Backend
![FastAPI](https://img.shields.io/badge/FastAPI-0a0a0a?style=for-the-badge&logo=fastapi&logoColor=00ff41)
![Node.js](https://img.shields.io/badge/Node.js-0a0a0a?style=for-the-badge&logo=nodedotjs&logoColor=00ff41)
![ASP.NET](https://img.shields.io/badge/ASP.NET-0a0a0a?style=for-the-badge&logo=dotnet&logoColor=00ff41)
![REST](https://img.shields.io/badge/REST_APIs-0a0a0a?style=for-the-badge&logo=fastapi&logoColor=00ff41)

</td>
<td align="center" width="180">

### 🌐 Frontend
![React](https://img.shields.io/badge/React_19-0a0a0a?style=for-the-badge&logo=react&logoColor=00ff41)
![Flutter](https://img.shields.io/badge/Flutter-0a0a0a?style=for-the-badge&logo=flutter&logoColor=00ff41)
![HTML5](https://img.shields.io/badge/HTML5-0a0a0a?style=for-the-badge&logo=html5&logoColor=00ff41)
![Shadcn](https://img.shields.io/badge/Shadcn_UI-0a0a0a?style=for-the-badge&logo=shadcnui&logoColor=00ff41)

</td>
</tr>
<tr>
<td align="center" width="180">

### 🤖 AI & CV
![YOLOv8](https://img.shields.io/badge/YOLOv8-0a0a0a?style=for-the-badge&logo=python&logoColor=00ff41)
![OpenCV](https://img.shields.io/badge/OpenCV-0a0a0a?style=for-the-badge&logo=opencv&logoColor=00ff41)
![TFLite](https://img.shields.io/badge/TF_Lite-0a0a0a?style=for-the-badge&logo=tensorflow&logoColor=00ff41)
![PyTorch](https://img.shields.io/badge/PyTorch-0a0a0a?style=for-the-badge&logo=pytorch&logoColor=00ff41)
![UiPath](https://img.shields.io/badge/UiPath-0a0a0a?style=for-the-badge&logo=uipath&logoColor=00ff41)

</td>
<td align="center" width="180">

### 🦾 Robotics
![ROS](https://img.shields.io/badge/ROS-0a0a0a?style=for-the-badge&logo=ros&logoColor=00ff41)
![Arduino](https://img.shields.io/badge/Arduino-0a0a0a?style=for-the-badge&logo=arduino&logoColor=00ff41)
![RPi](https://img.shields.io/badge/Raspberry_Pi-0a0a0a?style=for-the-badge&logo=raspberrypi&logoColor=00ff41)
![Fusion360](https://img.shields.io/badge/Fusion_360-0a0a0a?style=for-the-badge&logo=autodesk&logoColor=00ff41)
![Docker](https://img.shields.io/badge/Docker-0a0a0a?style=for-the-badge&logo=docker&logoColor=00ff41)

</td>
<td align="center" width="180">

### ☁️ Cloud & Data
![GCP](https://img.shields.io/badge/GCP-0a0a0a?style=for-the-badge&logo=googlecloud&logoColor=00ff41)
![BigQuery](https://img.shields.io/badge/BigQuery-0a0a0a?style=for-the-badge&logo=googlebigquery&logoColor=00ff41)
![MongoDB](https://img.shields.io/badge/MongoDB-0a0a0a?style=for-the-badge&logo=mongodb&logoColor=00ff41)
![SQL](https://img.shields.io/badge/SQL_Server-0a0a0a?style=for-the-badge&logo=microsoftsqlserver&logoColor=00ff41)
![Linux](https://img.shields.io/badge/Linux-0a0a0a?style=for-the-badge&logo=linux&logoColor=00ff41)

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

[![Email](https://img.shields.io/badge/mishradhruv257%40gmail.com-0a0a0a?style=for-the-badge&logo=gmail&logoColor=00ff41)](mailto:mishradhruv257@gmail.com)
[![LinkedIn](https://img.shields.io/badge/5K%2B_Followers_·_LinkedIn-0a0a0a?style=for-the-badge&logo=linkedin&logoColor=00ff41)](https://www.linkedin.com/in/dhruv-01352a279/)
[![GitHub](https://img.shields.io/badge/Dhruvtara108_·_GitHub-0a0a0a?style=for-the-badge&logo=github&logoColor=00ff41)](https://github.com/Dhruvtara108)

<br/>

```
> Shipping AI + Robotics from India 🇮🇳
> Building at the intersection of Software · AI · Robotics · ML
> Open to: SWE roles · Robotics Engineering · Research collaborations
```

</div>
