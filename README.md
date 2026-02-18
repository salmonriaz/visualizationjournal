# Visualization Journal — Week 01 Package (v1.0.0)

## What this package does
- Creates a Quarto WEBSITE that looks like the common class "Course Notebook" layout:
  - Left sidebar navigation
  - "Weeks", "Labs", "Group Work" sections
  - Search box
- Builds output to /docs (GitHub Pages friendly)

## Files included
- _quarto.yml
- index.qmd
- week-01.qmd (implemented)
- week-02.qmd ... week-09.qmd (placeholders)
- lab-06.qmd (placeholder)
- group-weekly-plan.qmd (placeholder)
- group-week-04.qmd (placeholder)

## How to use
1) Copy these files into the ROOT of your Quarto project (same folder as your current index.qmd).
2) Render:
   - In Positron: "Render" / "Preview"
   - Or terminal: quarto render
3) Publish (GitHub Pages):
   - Commit + push, make sure GitHub Pages is configured to serve from /docs on the main branch.

## Mixing R + Python later
If a single .qmd contains both R and Python chunks, Quarto runs via knitr and Python goes through reticulate.
In those files you MUST add a first R chunk that calls reticulate::use_python(...).
