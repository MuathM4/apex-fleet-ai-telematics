# 🚛 APEX Fleet AI — Autonomous Telematics & Bi-Directional LLM Dispatch Platform

[![Live Demo](https://img.shields.io/badge/LIVE_DEMO-ONLINE-10b981?style=for-the-badge&logo=bolt&logoColor=white)](https://ai-autonomous-truck-r7gn.bolt.host)
[![Frontend](https://img.shields.io/badge/Frontend-React_%7C_Tailwind_CSS-38bdf8?style=for-the-badge&logo=react&logoColor=white)](#)
[![Geospatial](https://img.shields.io/badge/Mapping-Leaflet.js_%7C_Carto_Dark-10b981?style=for-the-badge&logo=leaflet&logoColor=white)](#)
[![AI Engine](https://img.shields.io/badge/AI_Core-Llama_3_%7C_Tool_Calling-8b5cf6?style=for-the-badge)](#)

> **Live Deployment:** **[Launch APEX Fleet AI Command Console](https://ai-autonomous-truck-r7gn.bolt.host)**

---

## 🏆 Project Overview & Engineering Achievement

**APEX Fleet AI** is an end-to-end **Autonomous Commercial Fleet Simulation & Real-Time Telematics Command Platform**, developed as an innovation project for **Taibah Thon**. Designed to model next-generation freight logistics operations across primary Saudi Arabian transport corridors (Madinah Logistics Hub, Jeddah Islamic Port, Yanbu Industrial City, Riyadh Dry Port, and Dammam), the platform bridges **high-frequency vehicle telemetry** with **conversational AI agent dispatching** in alignment with the **Saudi Vision 2030 National Transport and Logistics Strategy**.

Unlike static dashboard mockups, this system implements a **closed-loop physics and cognitive architecture**: natural language commands issued by a human dispatcher (in English or Saudi Arabic) are parsed into structured tool calls that directly mutate the real-time kinematics, speed governors, and hierarchical state machines of moving trucks on the map.

---

## ✨ Key Architectural Achievements

- **Stochastic Multi-Agent Physics Engine:** Simulates concurrent commercial semi-trucks with Gaussian throttle drift, 12-speed Automated Manual Transmission (AMT) gear/RPM synthesis, dynamic fuel burn rates ($\text{L/h}$), coolant thermodynamics, and Hours-of-Service (HOS) driver fatigue modeling.
- **Unscripted World Event Injection:** Agents autonomously encounter and report stochastic highway hazards (sandstorm visibility drops, stray livestock, lane closures, and thermal creep) without human scripting.
- **Closed-Loop AI Dispatch Radio (Tool Calling):** Bi-directional communication console powered by Llama-3 / Structured NLP. Dispatchers can negotiate with virtual drivers, request live ETA/telemetry readbacks, or issue operational directives (`SET_SPEED`, `PULL_OVER`, `RESUME_CRUISE`, `TAKE_DETOUR`) that physically alter vehicle telemetry in real time.
- **Interactive Fault & "Drama" Injection:** Built-in chaos-engineering controls allow operators to inject J1939 engine overheat faults (`115°C` ECU limp mode), harsh air-brake events (`-7.4 m/s²`), and overspeed violations to test automated safety workflows.

---

## 🏗️ System Architecture
