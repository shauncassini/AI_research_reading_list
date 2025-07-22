# Research Paper Reading List (LaTeX Template)

Author: Shaun Cassini  
Date: 2025-07-22

This project is a **LaTeX-based reading list template** for researchers.  
It allows you to keep track of papers with structured notes, all tied to your `.bib` file.

## Features
- Auto-pulls **title, authors, year, and URL** from your BibTeX database.
- Structured fields for **status, summary, contributions, methods, datasets, etc.**
- Missing fields are automatically marked `(Missing)`.
- IEEE-style references automatically generated.

## How to Use
1. Clone this repo.
2. Edit `papers.bib` to include your papers.
3. Add `\paperentry[...]` blocks to `main.tex` for each paper.
4. Compile with **`pdflatex` + `biber`** (or just use Overleaf).

Example usage:
```latex
\paperentry[
  status={Read, TODO: Replication},
  summary={Introduced the Transformer, replacing RNNs.},
  datasets={WMT 2014 English–German},
]{vaswani2017attention}
```

## Licence
This project is licensed under the MIT License (see LICENSE).