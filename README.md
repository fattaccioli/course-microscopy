# Fluorescence Microscopy — Course Materials

Online course materials for **Microscopie de Fluorescence**, M2 Microscopies, Sorbonne Université / ENS.

**Jacques Fattaccioli** — Institut Pierre-Gilles de Gennes

## Structure

```
microscopy-course/
├── _quarto.yml                          # Site configuration
├── index.qmd                            # Course overview
├── lectures/                            # Lecture notes (from PPTX/PDF source)
│   ├── 01-introduction.qmd
│   ├── 02-fluorescence-principles.qmd
│   ├── 03-fluorophores.qmd
│   ├── 04-microscope-in-practice.qmd
│   ├── 05-digital-imaging.qmd
│   ├── 06-advanced-techniques.qmd
│   ├── 07-ricm.qmd
│   └── 08-two-photon.qmd
├── tutorials/                           # Problem sets with corrections
│   └── single-molecule-microscopy.qmd
├── images/                              # Figures extracted from slides
├── references.bib
└── .github/workflows/publish.yml        # Auto-deploy to GitHub Pages
```

## Building locally

```bash
quarto preview    # live preview
quarto render     # full build
```

## Deployment

Pushing to `main` triggers automatic deployment to GitHub Pages via GitHub Actions.

## Adding content

1. Edit or create `.qmd` files in `lectures/` or `tutorials/`
2. Add figures to `images/`
3. Reference figures in `.qmd` files: `![Caption](../images/figure.png)`
4. `git push` → site rebuilds automatically
