# Taming Undefined Behavior in LLVM

This repository contains a Beamer slide deck about the PLDI 2017 paper **“Taming Undefined Behavior in LLVM.”**

## Repository structure

- `main.tex`: entry point for the presentation
- `beamers/`: individual slide sections
- `images/`: images and figures used in slides
- `beamerthemeSNSPisa.sty`: custom Beamer theme
- `llvmlisting.sty`: LLVM-IR listing style
- `bibliography.bib`: bibliography source

## Requirements

- A TeX distribution with LuaLaTeX or XeLaTeX support (LuaLaTeX is configured by default)
- `latexmk`
- `inkscape` (for `svg` support)
- `JetBrains Mono` font (used for code listings)

## Build

From the repository root:

```bash
latexmk -lualatex -shell-escape main.tex
```

The generated PDF will be `main.pdf`.

## Clean build artifacts

```bash
latexmk -C
```
