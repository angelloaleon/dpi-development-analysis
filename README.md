# Digital Public Infrastructure & Development Co-operation
## A Data-Driven Policy Analysis for Low- and Middle-Income Countries

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![OECD DAC](https://img.shields.io/badge/Data-OECD%20DAC%20%7C%20World%20Bank-green)](https://stats.oecd.org/)

---

### Overview

This project analyzes the landscape of **Digital Public Infrastructure (DPI)** adoption and donor financing in low- and middle-income countries (LMICs), with a focus on how international development co-operation can better support inclusive digital transformation.

The analysis draws on OECD Development Assistance Committee (DAC) data, World Bank open indicators, and ITU statistics to produce evidence-based policy insights relevant to the OECD DAC's emerging work stream on digital transformation.

> **Policy Question:** Are international donors aligning their digital ODA flows with the countries and sectors where DPI investment would have the greatest development impact?

---

### What is Digital Public Infrastructure?

DPI refers to shared digital systems that function like public goods — enabling broad participation in society and the economy. Core components include:

| Pillar | Examples |
|--------|----------|
| **Digital ID** | National ID systems, legal identity registries |
| **Payment Infrastructure** | Real-time payment rails, interoperable mobile money |
| **Data Exchange** | Health data platforms, civil registration systems |
| **Connectivity** | Broadband networks, universal service funds |

The G20 and OECD have increasingly recognized DPI as a foundation for achieving the SDGs, particularly in Africa, South Asia, and Latin America.

---

### Project Structure

```
dpi-development-analysis/
│
├── notebooks/
│   └── dpi_lmic_analysis.ipynb     # Main analysis notebook + policy brief
│
├── data/
│   └── raw/                         # Downloaded datasets (auto-fetched by notebook)
│
├── outputs/
│   └── figures/                     # Exported charts and visualizations
│
├── requirements.txt
└── README.md
```

---

### Data Sources

| Source | Dataset | Access |
|--------|---------|--------|
| **OECD.Stat / DAC** | CRS — ODA flows to ICT & digital sectors | [stats.oecd.org](https://stats.oecd.org/) |
| **World Bank** | WDI — Internet use, broadband, financial inclusion | `wbgapi` Python package |
| **ITU** | ICT Development Index, mobile broadband coverage | [itu.int/en/ITU-D/Statistics](https://www.itu.int/en/ITU-D/Statistics/) |
| **UNDP** | Human Development Index (HDI) | [hdr.undp.org](https://hdr.undp.org/) |

All data is fetched programmatically via official APIs. No proprietary datasets are used.

---

### Key Analyses

1. **DPI Adoption Trends (2010–2023)** — Internet penetration and mobile broadband coverage across LMIC regions, disaggregated by gender where data permits.

2. **ODA Flows to Digital Sectors** — OECD DAC CRS analysis of bilateral and multilateral donor commitments to ICT/digital, identifying funding gaps and leader/laggard donors.

3. **DPI × Development Outcomes** — Correlation analysis between digital infrastructure indicators and financial inclusion, poverty rates, and SDG progress proxies.

4. **Policy Brief** — An OECD-style policy brief with findings and recommendations for DAC members on how to strengthen digital development co-operation practices.

---

### Policy Relevance

This analysis is aligned with:
- The **OECD DAC Recommendation on Enabling Open and Innovative Government** (2017)
- The **G20 DPI Framework** (2023, India Presidency)
- **OECD Digital Government Policy Framework**
- **SDG 9** (Industry, Innovation and Infrastructure) and **SDG 17** (Partnerships for the Goals)

---

### How to Run

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/dpi-development-analysis.git
cd dpi-development-analysis

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook notebooks/dpi_lmic_analysis.ipynb
```

---

### Author

**Angello Leon** | MA International Affairs, Graduate Institute Geneva  
Research interests: digital governance, development co-operation, anti-corruption

---

*This project was produced as an independent policy research exercise. It is not affiliated with or endorsed by the OECD.*
