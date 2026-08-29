# SafeHerAI — Unified AI Women's Safety Platform

> **MSME Idea Hackathon 6.0 | POC Demo**
> A unified, context-aware journey safety architecture powered by a five-stream AI Safety Brain.

---

## Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                    AI SAFETY BRAIN                          │
│         Context-Aware Multi-Agent Decision Engine           │
│                                                             │
│  Environmental │ Journey/Ride │ Physiological │ Community   │
│  Intelligence  │ Intelligence │ Intelligence  │ Intelligence│
│                                                             │
│  ► Risk Prediction  ► Counterfactual Analysis              │
│  ► Explainable AI   ► Adaptive Safety Policies             │
│  ► Guardian Intelligence  ► Intervention Routing           │
└──────────────────────────┬──────────────────────────────────┘
                           │
          ┌────────────────┼────────────────┐
          ▼                ▼                ▼
   Flutter App      Streamlit          FastAPI
   (Mobile)         (Dashboard)        (Backend)
```

## Five Intelligence Tracks

| Track | Capability |
|-------|-----------|
| 🗺️ **AI Safety Map** | Dynamic safety heatmap, exposure-aware routing, counterfactual route analysis, safe-haven recommendation |
| 🚗 **Smart Ride Intelligence** | Journey safety twin, multi-agent ride monitoring, driver deviation detection, escalation |
| 💓 **Wearable Safety Intelligence** | Physiological data (HR, SpO2, stress), fear/distress probability estimation |
| 👥 **Community Safety Intelligence** | AI-verified crowd-sourced reports, trust scoring, dynamic map updates |
| 🤖 **AI Safety Companion** | Gemini-powered guidance, grievance summarisation, complaint routing |

---

## Project Structure

```
SafeHerAI/
├── backend/           # FastAPI — central intelligence backend
├── streamlit_app/     # Streamlit — demo dashboard (5 pages)
├── flutter_app/       # Flutter — mobile safety app
├── README.md
└── .gitignore
```

---

## Quick Start

### 1. Backend
```bash
cd backend
pip install -r requirements.txt
cp .env.example .env          # add your GEMINI_API_KEY
uvicorn main:app --reload
# → http://localhost:8000
# → Docs: http://localhost:8000/docs
```

### 2. Streamlit Dashboard
```bash
cd streamlit_app
pip install -r requirements.txt
streamlit run app.py
# → http://localhost:8501
```

### 3. Flutter App
```bash
cd flutter_app
flutter pub get
flutter run                   # connect device or emulator
```

---

## Demo Scenarios

| Scenario | Description | Triggers |
|----------|-------------|---------|
| `NORMAL` | Safe journey, all signals green | Default |
| `DEVIATION` | Ride deviates from planned route | Smart Ride Intelligence alert |
| `DISTRESS` | Physiological distress detected | Wearable + AI Brain escalation |
| `COMMUNITY_ALERT` | Community report near user | Community Intelligence + reroute |

Switch scenarios via the Streamlit dashboard or query param `?scenario=DEVIATION`.

---

## Innovation

SafeHerAI is not a single-feature safety app. It is a **unified AI Safety Brain** that:

- Fuses **5 heterogeneous intelligence streams** simultaneously
- Maintains a **continuous, evolving journey-level safety state** (not point-in-time alerts)
- Performs **counterfactual decision analysis** ("what if she takes Route A?")
- Generates **explainable, adaptive interventions** to guardian, police, emergency services
- Provides **safe-arrival verification** and **AI-assisted grievance redressal**

---

## Team
VIT-AP University | MSME Idea Hackathon 6.0
Reference: 26INC06AP044404
