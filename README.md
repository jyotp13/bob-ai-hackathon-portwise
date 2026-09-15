#  Portwise

---

##  Team

| Field | Value |
|---|---|
| **Team Name** | Kunj Patel |
| **Track** | AI |
| **Team Lead** | Kunj — 26cs080@charusat.edu.in  |
| **Members** | Dharmay Thakkar , Siddhi Modi , Jyot Patel , Kunj Patel |

---

##  Problem Statement

The 2021 LA/Long Beach port backlog left 100+ ships waiting offshore for weeks, costing global supply chains over $10B. Port operators still allocate berths, cranes, and yard space across hundreds of vessels manually in spreadsheets, so congestion hotspots are identified reactively — only after vessels are already queuing — leaving no time to act on alternate routing or scheduling decisions.
---

##  Solution

PortFlow predicts berth congestion hotspots up to 72 hours in advance by analyzing incoming vessel schedules against real-time berth availability, then recommends an optimized berth and crane assignment plan that prioritizes critical and time-sensitive cargo. The system outputs a clear, shift-ready operations plan instead of a reactive spreadsheet update.
---

##  Key Features

- **Feature 1:** 72-hour congestion hotspot prediction based on vessel ETA vs. berth availability
- **Feature 2:** Automated berth and crane assignment optimization, prioritized by cargo urgency
- **Feature 3:** Shift-ready operations plan report generated automatically from prediction data
- **Feature 4:** Flags at-risk vessels likely to face delays before they occur
---

##  Tech Stack

| Category | Technologies |
|---|---|
| **Languages** | Python |
| **Frameworks** | None — command-line scripts only |
| **IBM Technologies** | IBM Cloud |
| **Databases** | None — vessel and berth data stored as CSV files |
| **Other** | GitHub Actions (template validation) |

---

##  Repository Structure

```
├── src/ # All source code
│ ├── data/ # vessels.csv, berths.csv
│ ├── predict_congestion.py
│ ├── generate_ops_plan.py
│ └── output/ # berth_plan.json, ops_plan.md
├── docs/ # Written documentation
│ ├── problem-statement.md
│ ├── solution-overview.md
│ ├── architecture.md
│ └── setup-guide.md
├── demo/ # Demo artifacts
│ ├── screenshots/ # App screenshots
│ └── demo-video-link.txt # Link to demo video
├── presentation/ # Slide deck
└── submission.yaml # Structured submission metadata
```

---

##  How to Run

```bash
# 1. Clone the repo
git clone https://github.com/[friend-username]/bob-ai-hackathon-[team-name].git
cd bob-ai-hackathon-[team-name]

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the congestion prediction
python src/predict_congestion.py

# 4. Generate the operations plan report
python src/generate_ops_plan.py
```

---

##  Demo

| Artifact | Link |
|---|---|
|  Demo Video | [See demo/demo-video-link.txt](demo/demo-video-link.txt) |
|  Live Demo |[https://jyotp13.github.io/bob-ai-hackathon-portwise/t](https://jyotp13.github.io/bob-ai-hackathon-portwise/t) |
|  Screenshots | [See demo/screenshots/](demo/screenshots/) |
|  Presentation | [See presentation/slides.pdf](presentation/) |

---

##  Known Limitations

> Be honest — judges appreciate transparency over overclaiming.

- [Limitation 1: e.g., "Uses simulated vessel and berth data, not a live port operations feed"]
- [Limitation 2: e.g., "Fixed 72-hour prediction window; does not account for real-time weather or customs delays"]
- [Limitation 3: e.g., "No persistent database — plans are generated fresh per run, not stored historically
"]

---

## 🏅 What We're Most Proud Of

We're proud that PortFlow tackles a specific, high-cost operational failure — reactive congestion detection — with a targeted prediction-plus-optimization approach rather than a generic dashboard. We deliberately scoped the project around one clear workflow (vessel data in, actionable berth plan out) so that what we built is fully functional and understandable end-to-end, rather than a broader set of half-finished features.
---
