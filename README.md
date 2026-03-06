# Thornton Melon's Economics Lesson
### *As a Linear Programming Optimization Problem*

> *"The Japanese will kill us on the labor costs!"*  
> — Thornton Melon, Back to School (1986)

[![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![PuLP](https://img.shields.io/badge/PuLP-Linear%20Programming-green)](https://coin-or.github.io/pulp/)

---

## The Setup

In the 1986 comedy *Back to School*, Rodney Dangerfield plays Thornton Melon — a self-made millionaire who enrolls in college alongside his son. In one iconic classroom scene, a professor walks through a sterile textbook model for building a factory to produce widgets. Thornton promptly demolishes it with a barrage of real-world friction costs: bribing politicians for zoning, kickbacks to carpenters, payoffs to building inspectors, dealing with the teamsters, and mob-handled waste disposal.

Then the coup de grâce: *"The Japanese will kill us on labor costs!"*

This repository translates that rant into a rigorous **Linear Programming** cost-minimization problem — and uses Python to prove Thornton right.

---

## Notebooks

| Notebook                          | Description                                                                 | Version / Focus                          |
|-----------------------------------|-----------------------------------------------------------------------------|------------------------------------------|
| `back-to-school-lp.ipynb`         | Original factory production cost model + Japanese competition infeasibility | v1.0 – core production cost analysis     |
| `back-to-school-lp-v2.0.ipynb`    | Enhanced version: production costs + full logistics / transportation layer  | v2.0 – production + distribution         |

**v2.0 highlights:**
- Classic **Transportation Problem** — minimizing shipping costs from 2 factories to 4 warehouses
- Realistic distance-based + "Thornton surcharge" costs (tolls, unions, fuel…)
- Optimal shipment plan (Memphis dominates long-haul, NY serves local)
- What-if commentary (fuel price spikes, demand surges, adding a Texas factory)

---

## Technical Stack

- **Python 3.13**
- **[PuLP](https://coin-or.github.io/pulp/)** — linear programming modeling and solving
- **CBC Solver** (bundled with PuLP) — open-source LP/MIP solver
- **Jupyter Notebook**

---

## Getting Started

### Prerequisites
```bash

pip install pulp jupyter