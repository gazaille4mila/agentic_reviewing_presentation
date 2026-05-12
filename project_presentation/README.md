# LaTeX Project Presentation Template
This directory contains a LaTeX Beamer template for AMLRT project presentations.

The template ships with a custom Mila Beamer theme (`beamerthemeMila.sty`) and reusable slide macros (`slide_templates.tex`) for title, section, QA, and closing slides.

## Local Setup

1. **Install LaTeX Distribution**
    - **macOS**: Install [MacTeX](https://tug.org/mactex/):
      ```sh
      brew install --cask mactex
      ```
    - **Windows**: Install [MiKTeX](https://miktex.org/download).
    - **Linux**: Install TeX Live:
      ```sh
      sudo apt-get install texlive-full
      ```
2. **Install Work Sans (recommended)**
   **Work Sans** is the font used in Google Slides Mila templates. It is not always installed by default in your LaTeX distribution.
    - The theme uses `fontspec` and targets **Work Sans** when available.
    - If Work Sans is not installed, the theme falls back to Helvetica Neue.
    - **macOS**:
      ```sh
      brew install --cask font-work-sans
      ```
3. **Build and Preview**
    - Build with the provided Makefile targets (see below).
    - Use XeLaTeX-compatible recipes because the theme uses `fontspec`.

## Build Commands

From `project_presentation/`:

```sh
make help
make install
make build-presentation
make build-all
make clean
```
