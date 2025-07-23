# Modeling Transformer Aging and Life Loss Using IEEE Clause 7 for BESS Planning

This repository contains the full implementation of a transformer thermal aging model built during my 2025 summer research at Clarkson University. The goal was to evaluate the insulation loss of life (LOL) of a 2.8 MVA transformer under real SCADA load and NASA ambient temperature data, and assess the benefit of BESS deployment to defer a $13.7M upgrade in Stillwater, NY.

---

## 🔧 Tools & Methods

- IEEE C57.91 Clause 7 thermal aging model (top-oil & hotspot temperature)
- FAA (Aging Acceleration Factor) and LOL (Loss of Life) calculations
- Python-based simulation using minute-resolution time steps
- BESS-capped load simulation for deferral analysis

---

## 📁 Repository Structure

| Folder        | Description                                      |
|---------------|--------------------------------------------------|
| `data/`       | Real SCADA load data and NASA ambient temperature |
| `code/`       | Python scripts implementing the thermal model     |
| `results/`    | Loss of life outputs and temperature plots        |
| `figures/`    | Diagrams and visual references for the poster     |

---

## 📊 Example Results (June 1st, 2023)

| Metric                        | Uncapped Load | BESS-Capped Load |
|------------------------------|---------------|------------------|
| Peak Hotspot Temperature     | 98.4 °C       | 91.7 °C          |
| Total Loss of Life (LOL)     | 0.0052 %      | 0.0026 %         |
| Aging Reduction via BESS     | —             | ~50%             |

---

## 💡 Key Takeaways

- Real-world modeling provides more accurate insights than synthetic assumptions
- BESS can significantly reduce thermal aging and help utilities defer expensive upgrades
- A minute-resolution Python model + SCADA data = more realistic planning support

---

## 🧠 Future Work

- Test BESS impact under hotter summer scenarios
- Automate simulation pipeline for other transformer assets
- Integrate NYSEG economic models into LOL-BCA feedback loop

---

## 🙏 Acknowledgments

Special thanks to **Dr. Leo Y. Jiang** for his mentorship and the **McNair Scholars Program** for supporting this research.

_This repository is maintained by Nas Nfaoui (Summer 2025)._

---

📎 **Poster + Simulation Code Access**  
Scan the QR code on the poster to visit this repository and explore the full simulation.
