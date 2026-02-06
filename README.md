# 🌊 Subsea Cable Vulnerability Index (SCVI) 3.0
> **Modeling Physical, Operational, and Geopolitical Resilience in Global Fiber-Optics**

![Version](https://img.shields.io/badge/version-3.0.0-blue.svg)
![Field](https://img.shields.io/badge/Field-Geopolitics%20%26%20Network%20Science-orange)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📌 Project Abstract
Submarine cables carry **99%** of global transoceanic data. However, existing resilience models often ignore the "Grey Zone" between physical infrastructure and geopolitical friction. This project constructs the **SCVI 3.0**, a unified framework to quantify national digital sovereignty.

---

## 🛠️ The 4-Pillar Framework
The index is calculated as a weighted average (25% each) of the following pillars:

### 🔵 Pillar I: Physical Network Robustness
*Focus: Topological stability and geometric diversity.*
- **Route Diversity ($HHI_{route}$):** Calculated using the Herfindahl-Hirschman Index to detect "Single Points of Failure."
- **Node Betweenness Centrality:** Identifies "hub" nations whose disruption causes global cascading failures.
- **Algebraic Connectivity:** Uses the **Fiedler Value** of the network graph to measure how easily a network can be partitioned.

### 🟢 Pillar II: Geographic & Environmental Exposure
*Focus: Physical hazards and "Aggression Zones."*
- **Chokepoint Dependency:** Vulnerability to narrow passages (e.g., Malacca Strait, Red Sea).
- **Shallow Water Risk:** Exposure to depths $<200$m where 70% of accidental cable cuts occur.
- **Strategic Insight:** CSIS notes that cables are prime targets for **"Grey Zone" attacks**—sabotage that is difficult to attribute to a state actor.



### 🟡 Pillar III: Operational Sovereignty
*Focus: The ability to maintain and repair infrastructure independently.*
- **Sovereign Repair Vessels:** Tracking domestic-flagged ships vs. foreign-owned fleets.
- **Cable Protection Zones (CPZs):** Legal frameworks that penalize ships for anchoring near critical lines.
- **Strategic Insight:** Resiliency is a function of **Repair Speed**. In conflict zones, repair permits can be weaponized to keep a country offline.

### 🔴 Pillar IV: Geopolitical & Ownership Security
*Focus: Influence of foreign states and "Hyperscalers."*
- **Transit State Alignment:** Measuring the political "friction" of cables passing through foreign EEZs using UN Voting Data.
- **Ownership Diversity:** Analyzing the shift from telecom consortiums to **Hyperscalers** (Google, Meta, Amazon).
- **Strategic Insight:** Hyperscalers now own over two-thirds of international bandwidth, shifting control from public regulators to private tech giants.

---

## 📅 Semester Implementation Plan

| Phase | Duration | Key Activities |
| :--- | :--- | :--- |
| **Phase 1: Data Mining** | Weeks 1-4 | Scrape **TeleGeography**; Integrate UN Voting Data & AIS ship locations. |
| **Phase 2: Coding** | Weeks 5-8 | Build Graph via `NetworkX`; Map EEZs via `GeoPandas`. |
| **Phase 3: Analysis** | Weeks 9-12 | Calculate SCVI scores for G20; Case Study: India's "Pakistan vs. Singapore" routes. |
| **Phase 4: Reporting** | Weeks 13-14 | Build **Streamlit Dashboard** and final presentation. |

---

## 💻 Tech Stack
- **Languages:** ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
- **Data Science:** `GeoPandas`, `NetworkX`, `NumPy`, `Pandas`
- **Visualization:** `Streamlit`, `Plotly`, `Folium`
- **Data Sources:** TeleGeography, PCH, MarineRegions.org

---

## ⚠️ Disclaimer
> [!IMPORTANT]
> This project is for academic purposes at **IIIT Bengaluru**. It utilizes proprietary data from **TeleGeography**; users must ensure they have a valid subscription to access the raw `.json` datasets.

---
**References:**
- *Center for Strategic and International Studies (CSIS): "Securing Subsea Cable Infrastructure"*
- *SCVI 3.0 Project Elective Proposal (PE_PRESENTATION.pdf)*
