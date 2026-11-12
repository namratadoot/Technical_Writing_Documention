
# LaTeX Notes

## 1. Introduction

LaTeX is a document preparation system based on TeX.

### Advantages
- Portable and free.
- Professional document layouts.
- Convenient mathematical typesetting.
- Supports multiple output formats.
- Generates references, tables of contents and bibliographies.

### Tools
- Windows: MiKTeX, TeXstudio.
- Linux: TeX Live, Kile.
- Online: Overleaf, Papeeria, CoCalc.

### File Formats
- Input: `.tex`
- Output: PDF, DVI, PostScript, RTF.

## 2. Document Structure

```latex
\documentclass{article}
\begin{document}
Hello World!
\end{document}
```

### Document Classes
- article
- report
- book
- letter
- beamer
- exam

### Compilation
```bash
pdflatex filename.tex
```

## 3. Title and Abstract

```latex
\title{My Document}
\author{Author Name}
\date{\today}
\maketitle
```

Abstract:

```latex
\begin{abstract}
Abstract text.
\end{abstract}
```

## 4. Sections and Formatting

```latex
\section{Introduction}
\subsection{Background}
\subsubsection{Details}
```

Common formatting commands:

- `\textbf{}` – Bold
- `\emph{}` – Emphasized
- `\tiny` – Tiny text
- `\large` – Large text
- `\Huge` – Largest text

Text alignment:
- `flushleft`
- `center`
- `flushright`

## 5. Mathematical Expressions

Inline mathematics uses `$...$`.

Display mathematics uses `\[...\]`.

```latex
\[
E=mc^2
\]

\[
\frac{a+b}{c}, \quad \sqrt{x}
\]

\[
\sum_{i=1}^{n}x_i
\]
```

Other mathematical elements:
- Superscripts: `^`
- Subscripts: `_`
- Greek letters: `\alpha`, `\beta`, `\gamma`
- Integrals: `\int`
- Products: `\prod`

## 6. Arrays and Matrices

Array example:

```latex
\[
\begin{array}{cc}
a & b\\
c & d
\end{array}
\]
```

Matrix environments:
- matrix
- pmatrix
- bmatrix
- Bmatrix
- vmatrix
- Vmatrix

## 7. Lists

Three list environments:

- `itemize` – Bulleted list.
- `enumerate` – Numbered list.
- `description` – Description list.

```latex
\begin{itemize}
\item Apple
\item Mango
\end{itemize}
```

## 8. Tables

Tables use the `tabular` environment.

Column alignment:
- `l` – Left
- `c` – Center
- `r` – Right

```latex
\begin{tabular}{|c|c|}
\hline
Name & Marks\\
\hline
Alice & 90\\
Bob & 85\\
\hline
\end{tabular}
```

Important commands:
- `&` – Separates columns.
- `\\` – Ends a row.
- `\hline` – Horizontal line.
- `\multicolumn` – Combines columns.
- `\multirow` – Combines rows.

## 9. Document and Page Styles

```latex
\pagestyle{plain}
```

Available page styles:
- plain
- headings
- empty

Other formatting commands:
- `\newpage` – Page break.
- `\vspace{}` – Vertical space.
- `\hspace{}` – Horizontal space.
- `\setcounter{}` – Changes numbering.

## 10. Colours

The xcolor package provides colour support.

```latex
\usepackage{xcolor}
\textcolor{red}{Hello World}
```

Other commands:
- `\colorbox{}` – Coloured background.
- `\fcolorbox{}` – Coloured frame.

## 11. Figures

The graphicx package is used to insert images.

```latex
\usepackage{graphicx}

\includegraphics[scale=0.5]{image.jpg}
```

Figure environment:

```latex
\begin{figure}[h]
\centering
\includegraphics[width=0.5\textwidth]{image.jpg}
\caption{Sample Figure}
\label{fig:sample}
\end{figure}
```

## 12. Picture Environment

The picture environment draws lines, arrows and circles using coordinates.

```latex
\setlength{\unitlength}{1cm}

\begin{picture}(4,2)
\put(0,0){\vector(1,0){4}}
\put(2,1){\circle{0.2}}
\end{picture}
```

## 13. Cross References

- `\label{key}` – Defines a label.
- `\ref{key}` – Refers to a label.
- `\cite{key}` – Inserts a citation.
