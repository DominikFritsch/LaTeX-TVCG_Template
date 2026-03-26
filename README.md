# LaTeX_TVCG_Template

A structured LaTeX template for submissions to the
**IEEE Transactions on Visualization and Computer Graphics (TVCG)**.

---

## Requirements

- LaTeX distribution: [TeX Live](https://www.tug.org/texlive/) or [MiKTeX](https://miktex.org/)
- Editor: [Overleaf](https://www.overleaf.com/) (recommended) or VS Code with LaTeX Workshop
- BibTeX for bibliography management

---

## Project Structure
```
├── main.tex                  # Entry point – only \input{} calls
├── packages.tex              # All \usepackage{} declarations
├── settings.tex              # Package configurations & language toggle
├── metadata.tex              # Title, authors, abstract, keywords
├── references.bib            # Bibliography database
├── figures/                  # Place all figures here
└── sections/
    ├── 01_introduction.tex
    ├── 02_related_work.tex
    ├── 03_method.tex
    ├── 04_results.tex
    ├── 05_discussion.tex
    └── 06_conclusion.tex
```

---

## Language Toggle

This template supports switching between **German** and **English**
by changing a single line in `settings.tex`:
```latex
\germantrue     % German
\germanfalse    % English
```

This single switch controls both the Babel language settings and
all section content simultaneously.

---

## Compilation
```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

---

## References

- [TVCG Official Website](https://www.computer.org/csdl/journal/tg)
- [TVCG Author Guidelines](https://www.computer.org/digital-library/journals/tg/cfp-ieee-transactions-on-visualization-computer-graphics)
- [IEEEtran LaTeX Template](https://template-selector.ieee.org/)