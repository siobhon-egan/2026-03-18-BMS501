# BMS501 Workshop 4 — Case Mapping

2026‑03‑18

**Unit:** BMS501  
**Topic:** Case Mapping (Workshop 4)  
**Date:** 2026‑03‑18  

This repository contains all materials for the **Case Mapping** practical in BMS501.  
You’ll work in a Quarto document to map and interpret case data, following step‑by‑step instructions hosted on the unit website and LMS.

---

## 🚀 Quick Start (Recommended: Posit Cloud)

### Steps
1. **Open Posit Cloud** and your BMS501 project.
2. Open **`case-mapping.qmd`** in the editor.
3. Open these references in a second window:
    - [Workshop 4 (LMS)](https://moodleprod.murdoch.edu.au/mod/book/view.php?id=2972457&chapterid=87420#mod_book-chapter)
    - [Case Mapping Tutorial](https://siobhonlegan.com/2026-03-18-BMS501/case-mapping.html)
4. Follow the tutorial steps and run the chunks in `case-mapping.qmd`.
5. **Render** with Quarto:
   `quarto render case-mapping.qmd`

## 🎯 What We’ll Cover

By the end of this workshop you will be able to:

- Practice geocoding and working with case point data
- Explore different map types (dot maps and choropleths)
- Learn how to load, check, and align spatial data layers
- Understand how data type and map choice influence interpretation
- Begin building simple epidemiological maps to support infectious disease surveillance


## 📦 Repository Structure

Update paths if your structure differs.

```
.
├── data/                 # Input datasets (non-sensitive teaching data)
├── scripts/              # (Optional) Helper R scripts for plotting/mapping
├── results/              # Rendered outputs (figures, maps)
├── case-mapping.qmd      # Main Quarto document used in the practical
├── renv/                 # (Optional) Reproducible R environment
├── _quarto.yml           # (Optional) Quarto project config
└── README.md             # You are here
```

## 🧰 Requirements

Posit Cloud (recommended) or R ≥ 4.3 + Quarto ≥ 1.5 locally
If running locally, install Quarto: <https://quarto.org/docs/get-started/>

```r
# Example package install
#install.packages("pacman")
#install.packages("rmarkdown")
#use pacman to install/load packages
pacman::p_load(
  rio, # to import data
  tidyverse, # to clean, handle, and plot the data (includes ggplot2 package)
  sf, # to manage spatial data using a Simple Feature format
  tmap, # to produce simple maps, works for both interactive and static maps
  janitor # examining and cleaning data
)
```

## 📚 Workshop Links

- [Workshop 4 (LMS)](https://moodleprod.murdoch.edu.au/mod/book/view.php?id=2972457&chapterid=87420#mod_book-chapter)
- [Case Mapping Tutorial](https://siobhonlegan.com/2026-03-18-BMS501/case-mapping.html)


Keep both pages open while you work in `case-mapping.qmd`.


## 📝 How to Use This Repo During Class

Clone or open the project in Posit Cloud (preferred) or locally.
Open `case-mapping.qmd` and follow the tutorial steps (data import → cleaning → mapping → export).
Render to HTML/PDF when prompted.


## 🔄 Reproducibility (Optional)

If this repo includes an renv.lock, enable a reproducible R environment:
```r
install.packages("renv")
renv::restore()
```

Then render:
```bash
quarto render case-mapping.qmd
```

## 📤 Outputs

Interactive/printed maps saved to results/
A rendered HTML/PDF report from `case-mapping.qmd`


----

Egan, S. (2026). BMS501 Workshop 4: Case Mapping — Practical Materials (v2026-03-18).
GitHub repository: <https://github.com/siobhon-egan/2026-03-18-BMS501>