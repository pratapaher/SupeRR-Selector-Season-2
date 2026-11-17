# 🏆 Rajasthan Royals SupeRR Selector S2
### IPL 2027 Auction Intelligence Hub & High-Leverage Decision Engine

[![Netlify Status](https://img.shields.io/badge/Netlify-Live_Deploy-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://rr-supe-rr-selector.netlify.app/)
[![React 19](https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite_6-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-Proprietary_RR-EA1B84?style=for-the-badge)](#)

---

## 🌐 Live Platform Link

> ### 🔗 **[Explore the Live Hub → https://rr-supe-rr-selector.netlify.app/](https://rr-supe-rr-selector.netlify.app/)**
> *Fully interactive 3D tactical stadium, pressure scenario simulator, live purse allocation, and high-impact clutch telemetry.*

---

## 📌 Executive Summary

In T20 cricket, standard season averages are notoriously deceptive. A batter averaging 35 at a 130 strike rate across low-stress overs often falters when the asking rate touches 12.0 in the death overs. Similarly, an economy rate of 7.5 means little if a bowler hemorrhages 24 runs in the 19th over.

**SupeRR Selector S2** is an advanced, client-side auction intelligence war room engineered specifically for the **Rajasthan Royals** management and scouting setup ahead of the **IPL 2027 Auction**. 

Instead of baseline statistics, the engine filters and ranks players strictly by **$\Delta$-Lift** — measuring how much *better* a player performs when the match is on the line, cross-referenced with the exact ground geometry of the **Sawai Mansingh Stadium (SMS Jaipur)** (80m straight boundaries, 75m square arcs).

---

## 📊 Core Data & Analytics Methodology

### 1. The $\Delta$-Lift Metric
* **Clutch Batters ($\Delta\text{SR}$)**: $\text{HP Strike Rate} - \text{Baseline Strike Rate}$.
  Measures scoring acceleration specifically in high-pressure states (overs 16–20, required run rate $\ge 10.0$, or after 3+ early wickets).
* **Pressure Bowlers ($\Delta\text{Econ}$)**: $\text{HP Economy} - \text{Baseline Economy}$.
  Measures runs conceded per over under acute pressure compared to league-wide drift norms (+0.85 RPO baseline inflation).

### 2. Pressure Delivery Index (PDI %)
A composite reliability rating ($0-100\%$) synthesizing:
* Win-conversion rate in historical high-leverage deliveries (2022–2026 IPL dataset).
* Dot-ball avoidance / suppression under crisis.
* Boundary execution percentage in match-defining overs.

---

## 🚀 Key Feature Modules

```
┌────────────────────────────────────────────────────────────────────────┐
│                      SupeRR Selector S2 Architecture                   │
├────────────────────────────────────────────────────────────────────────┤
│  [1] 30-Sec FastScan HUD   ──▶ Headline Metrics & Judge Spotlights     │
│  [2] 3D Tactical Stadium   ──▶ SMS Jaipur Ground & Spatial Deployment  │
│  [3] Player Split Stage    ──▶ 45/55 Cutout & 5-Axis Telemetry Radar   │
│  [4] Scenario Simulator    ──▶ Real-time Chase & Target Engine         │
│  [5] War Room Purse Plan   ──▶ ₹32.5 Cr Auction & RTM Allocation       │
│  [6] Stadium Audio Deck    ──▶ IPL Anthem & Procedural Crowd Mix       │
└────────────────────────────────────────────────────────────────────────┘
```

### 1. 30-Second Franchise Brief & HUD
* **Instant KPI Cards**: Avg pressure lift (+34.3 ΔSR), economy hold, and average shortlist PDI.
* **Judge Spotlight Filters**: 1-click filtering for specific tactical scenarios:
  - 💥 **Crunch Chases**: RRR $\ge 11.0$ finishers (e.g., Rinku Singh, Shashank Singh).
  - 🛡️ **Top-Order Collapse**: Rebuilding anchors when 3+ wickets fall in powerplay.
  - 🏰 **Jaipur Fit**: Players with shot arcs calibrated for SMS Jaipur's unique 80m dimensions.

### 2. 3D Tactical Stadium Ground
* **Authentic Ground Geometry**: Built with CSS 3D perspective transforms (`rotateX(56°)`), featuring concentric emerald mowed lawn rings, boundary rope cushions, 30-yard fielding ring, and clay pitch strip.
* **Interactive Player Billboard Tokens**: 10 spring-animated jersey tokens per discipline (Batters / Bowlers) that adjust on toggle.
* **Instant Split-Stage Slide**: Clicking any player token or bottom selector button smoothly glides the viewport down directly to that player's comprehensive telemetry breakdown.

### 3. Cinematic Player Stage & Split Telemetry
* **Broadcast Cutout (Left)**: Custom vector jersey silhouettes featuring the official transparent Rajasthan Royals emblem, jersey numbers, and franchise target tags.
* **Data Card (Right)**:
  - **PDI Radial Gauge**: Circular SVG reliability gauge.
  - **5-Axis Radar Polygon**: Visualizing skills (Death Overs, Wicket Crisis, Tight Chase, Boundary Freq, Dot Avoidance) vs. IPL league average.
  - **Signature Pressure Moment**: Documented historical clutch match performance.
  - **SMS Jaipur Tactical Fit**: Precise role explanation for the Royals XI.

### 4. Real-Time Scenario Engine (Pressure Simulator)
* Real-time sliders for **Target Score** (140–240), **Balls Remaining** (6–36), and **Wickets Down** (2–8).
* Computes real-time **Required Run Rate (RRR)** and categorizes match state (`CONTROLLED`, `HIGH PRESSURE`, `EXTREME CRISIS`).
* Instant algorithm re-ranks all 20 players by empirical win probability for that exact match situation.

### 5. Mini-Auction War Room & Purse Optimizer
* Budget tracker for **₹32.5 Cr** projected mini-auction purse.
* Dynamic bid bracket toggles: **Conservative**, **Balanced**, and **Aggressive**.
* **₹4.0 Cr Safety Reserve**: Automated warning alerts if high ceiling bids violate minimum squad-fill floor requirements.
* Detailed target cards for Arshdeep Singh, Shashank Singh, and Mitchell Santner.

### 6. Immersive Stadium Audio Engine
* **IPL Anthem Feature**: Official trumpet theme plays automatically **5 seconds after entry**.
* **Smart 2-Play Cap**: Automatically plays exactly 2 times and terminates permanently without infinite annoyance.
* **Procedural Crowd Synthesis**: Dual-layer ambient crowd low-pass noise via Web Audio API.
* **1-Click Floating Control**: Minimal circular button to mute/unmute at any moment.

---

## 🛠️ Tech Stack & Architecture

| Layer | Technologies |
|---|---|
| **Framework** | [React 19](https://react.dev/) + [Vite 6](https://vitejs.dev/) |
| **Language** | [TypeScript](https://www.typescriptlang.org/) (Strict mode) |
| **Styling** | [Tailwind CSS v4](https://tailwindcss.com/) with custom franchise theme (`#EA1B84` Royal Pink, `#EAA822` Gold, `#001D48` Deep Navy) |
| **Animations** | [Motion](https://motion.dev/) (Framer Motion) + CSS 3D Transforms |
| **Data Visualization** | [Recharts](https://recharts.org/) (Radar & Polar charts) + Custom SVG Gauges |
| **Audio** | Web Audio API (procedural synthesis) + HTML5 Audio |
| **Hosting & CDN** | [Netlify Edge](https://www.netlify.com/) (Global CDN, Atomic Deploys, SPA Rewrite Rules) |

---

## 💻 Local Development Setup

### Prerequisites
* **Node.js** $\ge 18$
* **Yarn** (`npm install -g yarn`)

### 1. Clone the Repository
```bash
git clone https://github.com/pratapaher/RR_hackathon.git
cd RR_hackathon
```

### 2. Install Dependencies
```bash
cd frontend
yarn install
```

### 3. Run the Development Server
```bash
yarn dev
```
Open **`http://localhost:3000`** in your browser.

### 4. Build for Production
```bash
yarn build
```
Generates an optimized, tree-shaken static production bundle in `frontend/dist`.

### 5. Code Quality Checks
```bash
yarn lint
```

---

## 📁 Repository Directory Structure

```
RR_hackathon/
├── frontend/
│   ├── public/
│   │   ├── _redirects              # Netlify SPA redirect rules
│   │   ├── ipl-anthem.mp3          # Stadium entry theme
│   │   ├── rr-logo.png             # Official transparent RR emblem
│   │   └── RR-SupeRR-Selector...pdf# Official methodology whitepaper
│   ├── src/
│   │   ├── components/
│   │   │   ├── hub/
│   │   │   │   ├── Header.tsx      # Sticky brand bar & ticker
│   │   │   │   ├── FastScanHud.tsx # 30-sec KPI overview & judge filters
│   │   │   │   ├── StadiumField.tsx# 3D isometric field & player tokens
│   │   │   │   ├── PlayerCutout.tsx# Silhouette vector player bust
│   │   │   │   ├── PlayerStage.tsx # Split telemetry card & radar
│   │   │   │   ├── PressureSimulator.tsx # Dynamic chase engine
│   │   │   │   ├── AuctionRoom.tsx # Purse strategy & allocation
│   │   │   │   └── AudioDeck.tsx   # Audio toggle & delayed anthem
│   │   │   └── ui/                 # Reusable Radix & Tailwind components
│   │   ├── data/
│   │   │   └── players.ts          # Verified 20-player dataset & coordinates
│   │   ├── pages/
│   │   │   └── Home.tsx            # Single-page assembly & grand footer
│   │   └── index.css               # Franchise styles & animation keyframes
│   └── package.json
├── backend/                        # Bare starter skeleton & PDF generator
├── netlify.toml                    # Netlify deployment configuration
├── vercel.json                     # Vercel SPA routing configuration
└── README.md                       # Documentation & Project Guide
```

---

## 🎯 Rajasthan Royals Hackathon Submission Details

* **Project**: SupeRR Selector Season 2 — IPL 2027 Auction Intelligence Hub
* **Franchise Focus**: Rajasthan Royals (SMS Jaipur Home Venue Calibration)
* **Live Deployment**: **[https://rr-supe-rr-selector.netlify.app/](https://rr-supe-rr-selector.netlify.app/)**
* **Repository**: **[https://github.com/pratapaher/SupeRR-Selector-Season-2](https://github.com/pratapaher/SupeRR-Selector-Season-2)**
* **Author**: Pratap Aher ([@pratapaher](https://github.com/pratapaher))

---

<div align="center">
  <sub>Forged in Royal Pink & Navy Blue · Halla Bol ⚡</sub>
</div>
