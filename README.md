# CausalDataScience LaTeX Template

This repository is the reusable LaTeX paper template for CausalDataScience.
The manuscript content files are intentionally empty. Add project-specific
text only after creating a new repository from this template.

## Start a paper

1. Set the title, author, and date in `manuscript/main.tex`.
2. Write the abstract in `manuscript/abstract.tex`.
3. Write the paper in `manuscript/main/1.tex` through
   `manuscript/main/7.tex`.
4. Write supplementary material in `manuscript/appendix/`.
5. After adding the first citation, uncomment the two bibliography commands
   near the end of `manuscript/main.tex`.

## Build

Run the following commands from the repository root:

```sh
cd manuscript
latexmk -r ../latexmkrc -C
latexmk -r ../latexmkrc -pdf -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

The PDF and intermediate files are written to `build/`.

## Bibliography snapshot

`manuscript/reference.bib` is a frozen canonical union of 15 source-paper
bibliographies. It contains 645 unique citation keys.

SHA-256:

```text
64f0f250c9c699d89c15d3382f037f3a783ab9f955d090779fd9423b13199e3f
```
