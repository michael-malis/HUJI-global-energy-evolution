**Scope and purpose**  
This repository contains the full R Markdown workflow for a university assignment carried out **together with a study partner**. Our goal was to turn the raw **OWID Global Energy** panel (1965-2023) into an end-to-end analytical narrative that tracks:

* long-run trends in absolute fuel consumption and shifting fuel shares;  
* per-capita demand across income tiers and regions;  
* geographic patterns via choropleth maps;  
* empirical CDFs and box-plots that expose distributional outliers;  
* a simple “crisis detector” that flags years of extreme contraction in global and national energy use.

---

**Key features**

* **One-click R Markdown build** – knit the main `.Rmd` to reproduce every figure, map and table.  
* **Data pipeline** – scripted download, type-safe import and tidying of all CSV / Excel sources.  
* **Faceted visuals** – stacked area charts for six world regions plus side-by-side log/linear comparisons.  
* **Interactive maps** – `rworldmap` choropleths for nuclear share, energy per capita and user-chosen metrics.  
* **Crisis analysis module** – year-over-year change computation, moving-average smoothing and automatic ranking of the steepest collapses (e.g., Japan post-Fukushima).

Everything is written in plain R with tidyverse grammar, making the project easy to extend or adapt to newer OWID releases.
