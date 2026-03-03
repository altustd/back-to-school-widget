# Thornton Melon's Economics Lesson  
**As a Linear Programming Optimization Problem**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)](https://www.python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![nbviewer](https://img.shields.io/badge/render-nbviewer-orange?logo=Jupyter)](https://nbviewer.org/github/altust/Thornton-Melon-Economics-LP) <!-- replace with your actual repo path -->

**From *Back to School* (1986)**  
Turning Rodney Dangerfield's iconic "no respect" classroom rant into a **PuLP** linear program — because theory is great… until real-world costs (and Japanese competition) show up.

> "The Japs will kill us on the labor costs!"  
> — Thornton Melon

<p align="center">
  <img src="https://i.ytimg.com/vi/lKBbFHMEvDc/maxresdefault.jpg" alt="Rodney Dangerfield as Thornton Melon passionately explaining real-world costs" width="65%"/>
  <br><em>Thornton crashes Economics 101 and ruins the professor's clean model… with math.</em>
</p>

## What This Is

A humorous take on **cost-minimization linear programming** inspired by the famous factory-building scene in *Back to School*.

- Professor's idealized model → feasible, but expensive (~$149/unit after Thornton's "friction" costs)
- Add realistic 1986-era Japanese labor competition → **infeasible** (the math says "no respect!")

Uses **PuLP** to show:
1. Base U.S. factory (with kickbacks, mob waste disposal, etc.) → optimal solution
2. With added constraint (avg cost ≤ $15/unit) → provably impossible

Great for anyone who likes operations research, optimization, Python, or 80s comedy.

## Key Results

- **U.S. only (realistic overhead)**: $149,000 total cost → 1,000 units at $149 each
- **With Japanese benchmark** → **Infeasible** (Thornton wins again)

```text
Status:            Optimal
Total Cost ($1k):  149.0
Factory size:      1.0 (×10,000 sq ft)
Produced:          1000 units
Avg cost / unit:   $149.00
