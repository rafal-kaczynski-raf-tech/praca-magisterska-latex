# Master's Thesis

*[POLSKI](README.md)*

---

**Title:** *Modeling and control of a power electronic converter using artificial intelligence methods in the Python environment*

**Author:** Rafał Kaczyński &nbsp;·&nbsp; student ID **342208**
**Supervisor:** prof. dr hab. inż. Grzegorz Iwański
**University:** Warsaw University of Technology, Faculty of Electrical Engineering
**Institute:** Institute of Control and Industrial Electronics
**Field:** Applied Informatics &nbsp;·&nbsp; **Specialization:** Informatics in Business
**Defense year:** 2026

---

## About the thesis

This thesis presents the design and implementation of a custom **Digital Twin** of a bidirectional Buck-Boost DC-DC power converter, written in **Python**. The simulation environment is integrated with a metaheuristic **Particle Swarm Optimization (PSO)** algorithm, used for automated tuning of a model-free **Bang-Bang (MF-BB)** controller. The work is software-engineering and optimization oriented, culminating in empirical validation against commercial **PSIM** software.

**Keywords:** Digital Twin · Python · Particle Swarm Optimization (PSO) · Buck-Boost converter · model-free control · software engineering.

## Related repository

Source code of the Digital Twin (physics engine + MF-BB controller + PSO):
👉 [github.com/rafal-kaczynski-raf-tech/praca-magisterska](https://github.com/rafal-kaczynski-raf-tech/praca-magisterska)

## Repository structure

| File / directory | Contents |
|---|---|
| `EE-dyplom.tex` | Main file — title page, abstract, document structure |
| `EE-dyplom.bib` | Bibliography (BibTeX) |
| `EE-dyplom.cls` | Template LaTeX class (do not modify) |
| `tekst/` | Chapter content (`wstep.tex`, `analiza.tex`, `realizacja.tex`, `ai.tex`, `podsumowanie.tex`) |
| `rysunki/` | Figures, plots, and schematics used in the thesis |
| `gfx/` | Template graphics (WUT logos, headers) — do not modify |
| `Makefile` | Manual compilation script (XeLaTeX + Biber) |

## How to compile

### Overleaf (recommended)

1. Import the project from GitHub: *New Project → Import from GitHub*.
2. Open **Menu → Settings → Compiler** and select **XeLaTeX** (pdfLaTeX will not compile correctly).
3. Click **Recompile**.

### Locally (macOS / Linux with TeX Live)

```bash
make            # XeLaTeX → Biber → XeLaTeX → XeLaTeX
make clean      # removes auxiliary files
```

## Thesis status

Work in progress. Per-chapter progress is reflected in the commit history.

## License and copyright

Thesis content (files in `tekst/`, `rysunki/` and `EE-dyplom.tex`, `EE-dyplom.bib`) — © Rafał Kaczyński, 2026. All rights reserved.

## Template attribution

This thesis uses the **EE-dyplom** template for the Faculty of Electrical Engineering at Warsaw University of Technology.

* Template author: *Łukasz Makowski* &lt;lukasz.makowski.ee@pw.edu.pl&gt;
* Template repository: [github.com/SP5LMA/EE-dyplom](https://github.com/SP5LMA/EE-dyplom)
* Template license: [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)
* The template conforms to the [WUT Rector Directive 4/2022](https://www.bip.pw.edu.pl/Wewnetrzne-akty-prawne/Dokumenty-Rektora-PW/Zarzadzenia-Rektora/2022/Zarzadzenie-nr-4-2022-Rektora-PW-z-dnia-27-01-2022) (in Polish) on the formatting of diploma theses.
