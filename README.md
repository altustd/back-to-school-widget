# Thornton Melon's Economics Lesson
### *As a Linear Programming Optimization Problem*

> *"The Japanese will kill us on the labor costs!"*
> — Thornton Melon, Back to School (1986)

[![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![PuLP](https://img.shields.io/badge/PuLP-Linear%20Programming-green)](https://coin-or.github.io/pulp/)

---

## The Setup

In the 1986 comedy *Back to School*, Rodney Dangerfield plays Thornton Melon — a self-made
millionaire who enrolls in college alongside his son. In one iconic classroom scene, a professor
walks through a sterile textbook model for building a factory to produce widgets. Thornton
promptly demolishes it with a barrage of real-world friction costs: bribing politicians for
zoning, kickbacks to carpenters, payoffs to building inspectors, dealing with the teamsters,
and mob-handled waste disposal.

Then the coup de grace: *"The Japanese will kill us on labor costs!"*

This notebook translates that rant into a rigorous **Linear Programming** cost-minimization
problem — and uses Python to prove Thornton right.

---

## What's in the Notebook

### Problem Formulation

A classic LP cost-minimization model with two decision variables:

- **x** — factory size (units of 10,000 sq ft)
- **p** — units produced (tape recorders, or widgets... whatever)

**Objective:** minimize total cost
**Constraints:** minimum production demand, factory capacity, non-negativity

The objective function deliberately inflates fixed costs to reflect Thornton's overhead
realities (politicians, carpenters, teamsters, inspectors, the mob).

### Two Scenarios

| Scenario | Description | Result |
|---|---|---|
| **Base Model** | U.S. factory with real-world friction costs | Optimal — $149/unit |
| **Japanese Competition** | Adds a competitive cost-ceiling constraint | Infeasible |

The competition constraint (`average cost <= $15/unit`) produces an inequality that is
mathematically impossible to satisfy given the base costs — which is exactly Thornton's point.

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
```

### Run the Notebook
```bash
git clone https://github.com/altustd/back-to-school-widget.git
cd back-to-school-widget
jupyter notebook "back-to-school-lp.ipynb"
```

---

## Concepts Demonstrated

- **Linear Programming** problem formulation (objective function + constraints)
- **Feasibility analysis** — recognizing when a system of constraints is unsatisfiable
- Translating a real-world scenario into a mathematical model
- Using **PuLP** to define, solve, and interpret LP problems in Python
- Interpreting solver status codes (`Optimal`, `Infeasible`)

---

## Repository Structure
```
back-to-school-widget/
│
├── back-to-school-lp.ipynb   # Main notebook
└── README.md
```

---

## Disclaimer

This notebook is a comedic and educational exercise. Cost figures and international comparisons
are drawn from the satirical context of a 1986 film and are not intended as modern economic
analysis.

*Footnote: Coding, formatting, and stylistic enhancements developed with assistance from Grok
(xAI). Optimization results independently verified using ChatGPT. All modeling decisions and
interpretations are the author's own.*

---

## Author

**Troy Altus** — March 2026

---

*"...No respect!"*
