# Project-Elective_Sem6
This project, the Subsea Cable Vulnerability Index (SCVI) 3.0, is a sophisticated attempt to quantify how "safe" a country's internet connection is from a physical, political, and operational standpoint. While most people think of "the cloud" as something in the sky, 99% of global data actually travels through hair-thin glass fibers at the bottom of the ocean.

## 🛡️ 1. Understanding the Four Pillars of Vulnerability

The project quantifies risk by breaking down infrastructure health into four equal "Pillars," each contributing **25%** to the final vulnerability score.

---

### Pillar I: Physical Network Robustness
*Focus: The geometry and structural resilience of physical cable layouts.*

This pillar analyzes how geography and network design influence the likelihood of a total system failure.

#### 📍 Route Diversity ($HHI_{route}$)
If a country’s cables are concentrated in one narrow gap (like the Red Sea), a single anchor drag can take out the entire country. We mathematically identify this "concentration" using the **Herfindahl-Hirschman Index**:

$$HHI_{route} = \sum_{i=1}^{N} s_i^2$$

> **Note:** A higher $HHI$ score indicates a dangerous lack of diversity, signaling a "single point of failure."

#### 🔗 Node Betweenness Centrality
This metric identifies countries that act as **"Bridges."** * **The Risk:** If a country is a major hub, it becomes a high-value target during a conflict. 
* **The Impact:** Cutting cables at a high-centrality node disrupts not just the host nation, but many other dependent nations.

#### 📐 Algebraic Connectivity
We use the **"Fiedler value"** of the network graph to measure its structural integrity.
* This identifies how easily a network can be split into two "disconnected islands."
* It provides a mathematical snapshot of the network's overall cohesion and its ability to withstand multiple simultaneous cuts.

---
