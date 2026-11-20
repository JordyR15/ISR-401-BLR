## Cómo compilar GA-SUM-02

Diapositivas de la exposición sobre técnicas de elicitación y herramientas automatizadas de apoyo a la IR.

- Carpeta: `GA-SUM-02/`
- Archivo principal: `GA-SUM-02/main.tex` (incluye `bloqueA.tex`, `bloqueB.tex` y `bloqueCD.tex`; referencias en `GA-SUM-02/referencias.bib`)
- Compilador: pdfLaTeX con BibTeX (TeX Live, el predeterminado de Overleaf)
- Comandos, en orden (dentro de `GA-SUM-02/`):
  1. `pdflatex main.tex`
  2. `bibtex main`
  3. `pdflatex main.tex`
  4. `pdflatex main.tex`
- Dependencias (paquetes LaTeX): beamer, inputenc, fontenc, babel (spanish), tikz, booktabs, xcolor, IEEEtran (estilo bibliográfico)
