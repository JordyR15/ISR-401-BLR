# Presentación: Técnicas de Elicitación y Herramientas Automatizadas (GA-SUM-02)

Presentación desarrollada en **LaTeX / Beamer** para la asignatura **Ingeniería de Requerimientos (ISR-401)** — Universidad Técnica Estatal de Quevedo (UTEQ).

---

## Compilador y Herramientas Utilizadas

* **Distribución LaTeX:** MiKTeX (`pdfTeX 3.141592653` / MiKTeX 25.12 o superior)
* **Motor de compilación:** `pdfLaTeX`
* **Gestor de bibliografía:** `BibTeX` (estilo `IEEEtran`)
* **Editor recomendado:** TeXworks / Visual Studio Code (LaTeX Workshop)

---

## Estructura del Proyecto

```text
GA-SUM-02/
├── main.tex                   # Archivo principal (preámbulo, portada, estructura y referencias)
├── bloqueA.tex                # Bloque A: Técnicas de elicitación
├── bloqueB.tex                # Bloque B: Comparación de herramientas
├── bloqueCD.tex               # Bloques C y D: Recomendación y demostración (Helix ALM)
├── evidencias/                # Capturas de Helix ALM (imagen02.png, imagen03.png)
├── figuras/                   # Diagramas y evidencias de los bloques A y B
└── referencias/
    └── referencias.bib        # Base de datos bibliográfica en formato BibTeX
```

---

## Compilación desde CMD (Windows)

Para que las citas bibliográficas (`\cite{...}`) y el listado final de referencias se generen correctamente, es indispensable ejecutar **pdfLaTeX**, seguido de **BibTeX**, y nuevamente **pdfLaTeX** dos veces sobre el archivo `main.tex`.

Ejecutar la secuencia completa de compilación:

```cmd
pdflatex -interaction=nonstopmode main.tex
bibtex main
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Una vez finalizado el proceso sin errores, se generará el archivo **`main.pdf`** listo para presentar.

---