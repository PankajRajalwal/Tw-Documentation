# LaTeX

## 1. What is LaTeX?

LaTeX is a document preparation system commonly used for creating technical, scientific, and academic documents. It is especially useful for writing mathematical equations, tables, figures, and references.

## 2. Basic Structure of a LaTeX Document

Every LaTeX document has a basic structure:

```latex
\documentclass{article}

\begin{document}

Hello, LaTeX!

\end{document}
```

- `\documentclass{article}` selects the document type.
- The preamble contains settings and packages before `\begin{document}`.
- The document content is written between `\begin{document}` and `\end{document}`.

## 3. Common Document Classes

- `article`: Short documents and assignments.
- `report`: Long reports and projects.
- `book`: Book-length documents.
- `letter`: Letters.

## 4. Text Formatting and Sections

LaTeX provides commands for text formatting.

```latex
\textbf{Bold Text}

\textit{Italic Text}

\underline{Underlined Text}
```

For headings, use:

```latex
\section{Introduction}
\subsection{Overview}
\subsubsection{Details}
```

## 5. Lists

LaTeX supports two main types of lists.

**Unordered List:**

```latex
\begin{itemize}
    \item First point
    \item Second point
\end{itemize}
```

**Ordered List:**

```latex
\begin{enumerate}
    \item First step
    \item Second step
\end{enumerate}
```

## 6. Mathematical Equations

LaTeX is widely used for writing mathematical expressions.

**Inline Equation:**

```latex
\(a^2+b^2=c^2\)
```

**Displayed Equation:**

```latex
\[
E = mc^2
\]
```

**Numbered Equation:**

```latex
\begin{equation}
F = ma
\end{equation}
```

## 7. Tables

The `tabular` environment is used to create tables.

```latex
\begin{tabular}{|c|c|}
\hline
Name & Marks \\
\hline
Asha & 90 \\
Ravi & 85 \\
\hline
\end{tabular}
```

- `c` means center alignment.
- `l` means left alignment.
- `r` means right alignment.
- `\hline` creates a horizontal line.

## 8. Adding Figures and Images

To insert images, include the graphicx package in the preamble.

```latex
\usepackage{graphicx}
```

Example:

```latex
\begin{figure}[h]
    \centering
    \includegraphics[width=0.6\textwidth]{image.png}
    \caption{Example Figure}
    \label{fig:example}
\end{figure}
```

## 9. Labels and References

The `\label{}` command assigns a reference name to an item, and `\ref{}` is used to refer to it.

```latex
\section{Introduction}
\label{sec:intro}

See Section \ref{sec:intro}.
```

Bibliographies can be managed using a `.bib` file with BibTeX or another bibliography workflow.

## 10. Compiling a LaTeX Document

A common command to compile a LaTeX file is:

```bash
pdflatex main.tex
```

Compilation generates a PDF document. Some documents require multiple compilation passes or a bibliography tool.

## 11. Important Points and Best Practices

- Add required packages in the preamble.
- Close every environment correctly.
- Use proper section headings.
- Escape special characters such as `#`, `$`, `%`, `&`, `_`, `{`, and `}` when used as ordinary text.
- Compile the document and inspect the generated PDF.
- Keep images and other required files in the correct location.

## 12. Conclusion

LaTeX is a powerful tool for preparing professional technical and academic documents. It provides useful features for formatting text, writing equations, creating tables, inserting figures, and managing references.

> These are introductory notes. Follow the lab handout for the exact packages, compiler, and formatting requirements.