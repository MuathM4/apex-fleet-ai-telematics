# 🚛 Naqil AI (ناقل الذكي) — Autonomous Fleet Telematics & Driver Copilot

[![Live Demo](https://img.shields.io/badge/LIVE_PLATFORM-ONLINE-10b981?style=for-the-badge&logo=vercel&logoColor=white)](https://ai-autonomous-truck-r7gn.bolt.host)
[![Hackathon Project](https://img.shields.io/badge/Competition-Taibah_Thon_2026-6366f1?style=for-the-badge)](#)
[![Stack](https://img.shields.io/badge/Frontend-React_%7C_Tailwind_%7C_Leaflet-38bdf8?style=for-the-badge&logo=react&logoColor=white)](#)
[![AI Engine](https://img.shields.io/badge/Cognitive_Core-Bi--Directional_LLM_Dispatcher-8b5cf6?style=for-the-badge)](#)

> **Live Application URL:** **[https://ai-autonomous-truck-r7gn.bolt.host](https://ai-autonomous-truck-r7gn.bolt.host)**

---

## 🏆 Project Overview & Vision

**Naqil AI** is an intelligent telematics dispatch platform and autonomous driver copilot engineered to modernize freight logistics for commercial fleets and independent truck drivers (*الأفراد*) across Saudi Arabia's primary freight corridors (Madinah, Jeddah Islamic Port, Yanbu, Riyadh, and Dammam).

Developed as an innovative competition solution for **Taibah Thon**, the platform directly aligns with the objectives of the **Saudi Vision 2030 National Transport and Logistics Strategy**:
1. **Eliminating Deadheading:** Helping drivers secure profitable return-leg loads (*رجوع*) to cut empty miles and highway carbon emissions.
2. **Heavy-Vehicle Dynamic Safety:** Providing real-time telemetry monitoring, steep mountain pass elevation warnings (e.g., Aqabat routes), and simulated J1939 fault response protocols.
3. **Bilingual AI Voice/Text Dispatch:** An in-cab conversational copilot operating in Saudi Arabic and English that turns human dispatch directives into real-time vehicle kinematics modifications.

---

## 🌟 Key Features

### 1. 🗺️ Heavy Freight Map & Route Telematics
- Interactive geospatial tracking showing vehicle progress along real Saudi highway corridors.
- Route polylines with real-time ETA calculations, distance counters, and highway speed limit tracking.
- Heavy-vehicle route optimization factoring in truck curfews, weigh stations, and certified SASCO rest plazas.

### 2. 📊 Live Vehicle HUD ("The Metry")
- Sub-second telemetry gauges: **Ground Speed ($\text{km/h}$)**, **Engine RPM**, **Automated Gear Selection**, **Fuel SoC / Burn Rate ($\text{L/h}$)**, and **Engine Coolant Temperature ($^\circ\text{C}$)**.
- Driver safety scorecard and regulatory **Hours of Service (HOS)** fatigue monitoring.

### 3. 💬 Bi-Directional AI Driver Copilot
- Conversational dispatch bridge capable of understanding operational directives in Arabic (*"هدي السرعة إلى 60"* / *"وقف على جنب"*) and English.
- Real-time physics mutation: Directives to pull over or change speeds dynamically alter the moving truck's speed and status indicators on the map.

### 4. ⚡ Fault & Drama Injection (Chaos Engineering)
- Testable operational emergency modes:
  - **🔥 Engine Overheat:** Simulates thermal coolant spikes ($115^\circ\text{C}$), triggers ECU limp mode ($35\text{ km/h}$), and radios a priority mayday.
  - **🛑 Harsh Braking:** Simulates sudden hazard avoidance ($-7.4\text{ m/s}^2$ ABS deceleration).
  - **⚡ Overspeed Violation:** Alerts the control room when a unit exceeds the legal corridor limit.

---

## 🏗️ System Architecture

+-------------------------------------------------------------------------+
|                   PRESENTATION LAYER (Mobile & Web)                     |
|  - Real-Time Dark Geospatial Map (Polyline Routes & Heading Vectors)    |
|  - Live Telemetry HUD (Speed, RPM, Fuel SoC, Coolant Temp, Safety KPI)  |
|  - 2-Way AI Dispatch Radio + Chaos/Fault Injection Controls             |
+------------------------------------+------------------------------------+
| Event Loop / WebSockets (10Hz)
v
+-------------------------------------------------------------------------+
|                STOCHASTIC SIMULATION & COGNITIVE CORE                   |
|  - Kinematic Loop: Longitudinal Accel, AMT Gear/RPM & Thermal Drift     |
|  - AI Agent Router: Persona Context Hydrator + JSON Tool Execution      |
|  - Spontaneous Hazard Generator: Unscripted Traffic & Weather Events    |
+-------------------------------------------------------------------------+


---

## 🛠️ Tech Stack Matrix

| Layer | Technologies |
| :--- | :--- |
| **Frontend Framework** | React 18, TypeScript, Tailwind CSS |
| **Geospatial Engine** | Leaflet.js, Carto Dark Matter Tiles, Custom SVG Heading Markers |
| **UI Components** | Lucide Icons, Custom Animated Radial Gauges, Responsive HUD Drawer |
| **AI Cognitive Bridge** | Natural Language Processing / LLM Tool Calling (English & Saudi Arabic) |
| **Deployment Platform** | Cloud PWA Infrastructure ([Bolt.host](https://ai-autonomous-truck-r7gn.bolt.host)) |

---

## 🚀 Getting Started

### Live Demo (No Installation Required)
Access the fully functioning cloud deployment directly in your desktop or mobile browser:  
👉 **[Launch Naqil AI Platform](https://ai-autonomous-truck-r7gn.bolt.host)**

### Local Setup
```bash
# 1. Clone this repository
git clone [https://github.com/YOUR_USERNAME/naqil-ai-telematics.git](https://github.com/YOUR_USERNAME/naqil-ai-telematics.git)
cd naqil-ai-telematics

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
👨‍💻 Project Lead
Muath Makhlouf

Autonomous Systems, Full-Stack Telematics & AI Automation

Developed for Taibah Thon 2026
