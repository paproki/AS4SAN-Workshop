# Big Data in Neuroimaging - Hands-on Workshop

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/paproki/AS4SAN-Workshop/blob/main/big_data_neuroimaging_workshop.ipynb)

**A visual tour of the things that get *harder*, not easier, when your dataset gets huge.**

This repository holds the materials for the AS4SAN hands-on workshop on working with large-scale
neuroimaging datasets. The centrepiece is a single self-contained Jupyter notebook built for a
**neuroscience audience** and not aimed at programers or statisticians: you don't need to be a programmer to follow along. Every
code cell is already written and runs as-is - your job is to **read the picture**, then in the
*Your turn* cells **change one highlighted value and re-run** to watch the picture change.

---

## Quick start

### Run it in the browser (recommended - nothing to install)

Click the **Open in Colab** badge above. Once the notebook opens, run the first
**Setup** cell (it installs nothing beyond the standard scientific Python stack that Colab already
ships) and work through the exercises top to bottom.

There are no external data downloads - the notebook builds its own **simulated** dataset in the
first cell.

---

## Why simulated data?

The notebook uses a fabricated brain dataset (10,000 participants) with **engineered ground truth**,
so every exercise has a *known* right answer to check your reasoning against. The structure mirrors
the real big-data resources you'll actually meet - UK Biobank, ABCD, HCP, ENIGMA - where each of
these pitfalls is a *daily* reality: systematic missingness, confounding, tiny-but-significant
effects, multiple comparisons, and scanner/site effects.

---

## What's covered

| # | Exercise | The lesson |
|---|----------|------------|
| 1 | **Loading & inspecting** | Look at your data before you analyse it - summarise and plot when you can't read 10,000 rows by hand |
| 2 | **Missingness** | In big data, missing values are usually *not* random (MCAR / MAR / MNAR) |
| 2.5 | **Handling missingness** | Imputation vs simply dropping the blanks - and what each costs you |
| 3 | **Confounding** | How a relationship can be an illusion created by a third variable (with a DAG walk-through of confounders, colliders, and mediators) |
| 4 | **Prediction vs explanation** | Why a "significant" model can still predict badly |
| 5 | **Effect size vs significance** | Why almost everything becomes "significant" at scale |
| 6 | **Multiple comparisons** | Why testing many things guarantees false alarms |
| 7 | **Site & scanner effects** | The multi-scanner harmonisation headache |
| 8 | **Analysis choices** | How a chain of defensible decisions ("the garden of forking paths") changes the result |

---

## What's in this repo

- **`big_data_neuroimaging_workshop.ipynb`** - the hands-on notebook (the thing you run).

---

The notebook is designed to be worked through live. Each exercise ends with a *Your turn* cell that
changes exactly one value, so participants can see cause and effect immediately.
