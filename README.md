# Back to School Economics — A Real-World Linear Programming Lesson

**Repository:** https://github.com/altustd/back-to-school-widget  
**Notebook:** `back-to-school-lp.ipynb`

---

## What Is This?

This repository contains a **single, self-contained Jupyter notebook** that turns a famous movie scene into a **real, mathematically correct economics and optimization example**.

It is based on the iconic classroom scene from *Back to School*, starring Rodney Dangerfield, where his character (Thornton Melon) interrupts an economics lecture and points out all the real-world costs missing from the professor’s clean textbook model.

Instead of just laughing at the scene, this notebook asks:

> *What happens if we actually put Thornton Melon’s objections into the math?*

---

## Who Is This For?

This project is intentionally written so that **anyone can read it**, including:

- Students learning economics, operations research, or optimization  
- Data science and analytics hiring managers  
- Engineers and professionals who deal with “theory vs reality”  
- Movie fans curious whether Thornton Melon was actually right  

You **do not need to know Python**, linear programming, or optimization solvers to follow the story.

---

## What Does the Notebook Show?

The notebook walks through:

### 1. A Simple Textbook Model  
A professor proposes building a factory to make “widgets” (or tape recorders — it doesn’t matter).

The goal:
- Produce at least **1,000 units**
- Minimize total cost

### 2. Thornton Melon Crashes the Model  
Thornton adds the costs textbooks ignore:
- Political grease  
- Kickbacks  
- Union issues  
- Inspections  
- Waste disposal (handled by the mob)

These are added **explicitly into the math**.

### 3. The Model Still Works… But It’s Expensive  
With realistic U.S. costs included:
- The problem is **mathematically feasible**
- The result is **very expensive**
- Average cost comes out to **$149 per unit**

### 4. Japanese Competition Is Introduced  
Thornton’s killer line:

> “The Japanese will kill us on the labor costs!”

This is modeled as a constraint requiring the factory to match a lower average cost.

**Result:**  
The optimization problem becomes **mathematically infeasible**.

That means:
- Not “unprofitable”
- Not “hard”
- But **literally impossible** given the assumptions

This is the key lesson.

---

## Why This Is Interesting

- It demonstrates how **real-world constraints break idealized theory**
- It shows that **infeasibility is sometimes the correct answer**
- It connects economics, optimization, and common sense
- It turns a movie joke into a rigorous modeling example

Thornton Melon wasn’t just funny — **the math proves he was right**.

---

## What’s in This Repository?

| File | Description |
|----|----|
| `back-to-school-lp.ipynb` | The complete, readable notebook with explanations, math, and results |
| `README.md` | This file |

There are **no dependencies you need to install** unless you want to run the notebook yourself.

---

## How to View This (No Programming Required)

### Option 1 — View Directly on GitHub (Recommended)
1. Click **`back-to-school-lp.ipynb`** in the file list  
2. GitHub will render it as a readable document  
3. Scroll and read — no setup required  

### Option 2 — Download and Open Locally
If you are familiar with Jupyter notebooks, you can download and run it locally, but this is **not required** to understand the content.

---

## Technical Notes (Optional Reading)

- The optimization model is implemented using **:contentReference[oaicite:2]{index=2}**
- A standard open-source solver is used
- All results are deterministic and reproducible
- Numerical calculations were independently reviewed and verified using **:contentReference[oaicite:3]{index=3}**

---

## Disclaimer

This project is:
- Educational  
- Satirical  
- Historically contextual (1986 manufacturing economics)

It is **not** intended as modern economic analysis or policy guidance.

---

## Author

**Troy Altus**  
Created for education, illustration, and fun — with full respect to both economics and Rodney Dangerfield.

> “It doesn’t matter? It matters to me!”

---

## If You Enjoyed This

Feel free to:
- Star the repository  
- Share it with students or colleagues  
- Use it as a teaching or interview discussion piece  

Feedback and discussion are always welcome.
