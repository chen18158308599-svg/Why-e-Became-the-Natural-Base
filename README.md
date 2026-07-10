# The Number Nobody Was Looking For

**Why *e* Became the Natural Base**

An interactive Quarto document telling the history of Euler's number $e$ — from astronomers drowning in arithmetic, through Napier's logarithms and Bernoulli's compound-interest limit, to Euler's calculus unifying them all, and why $e$ keeps reappearing across science.

**Group:** BAAG
**Authors:** Chen Chen, Gao Shuo, Irene Bong Sze Ting

---

## What's inside

| Section | Idea |
|---|---|
| Introduction | Why $e$ shows up everywhere despite nobody looking for it |
| Astronomers Were Drowning in Arithmetic | The computational problem logarithms were invented to solve |
| John Napier's Shortcut | Turning multiplication into addition; Briggs's decimal tables |
| Bernoulli's Question | The compound-interest limit that first produced $e$ |
| Euler Connects the Dots | How calculus ties the logarithm and the limit to the same constant |
| Why $e$ Turns Up Everywhere | Population growth, radioactive decay, the 37% rule, logarithmic spirals |
| Conclusion | The number that was never invented, only discovered |

Includes several interactive Plotly demos built directly into the document:
- Napier's two-particle race (geometric decay vs. arithmetic growth)
- The tangent-slope slider on $a^x$ (hunting for the base with derivative slope 1)
- The area-splitting demo showing $\int \frac1t\,dt$ behaves like a logarithm

## Built with

- [Quarto](https://quarto.org/) — document rendering
- Python 3 (via Quarto's Jupyter engine)
- [Plotly](https://plotly.com/python/) — interactive figures
- [NumPy](https://numpy.org/)

## Getting started

**Prerequisites**
- [Quarto CLI](https://quarto.org/docs/get-started/) installed
- Python 3.9+
- `pip install numpy plotly`

**Render locally**

```bash
git clone <this-repo-url>
cd <repo-folder>
quarto render natural_base.qmd
```

This produces a self-contained HTML file with all interactive figures embedded. Open it in any browser — no server required.

> If you edit a code chunk and the rendered output doesn't seem to update, clear any `_freeze/` cache folder and re-render; Quarto can otherwise reuse stale widget output from a previous run.

## Project structure

```
.
├── natural_base.qmd      # main document
├── BAAG_images/          # figures and photos used in the document
└── README.md
```

## License

Course project — no license specified. Reuse with attribution.
