# Beamer

## 1. What is Beamer?

Beamer is a LaTeX document class used to create professional slide presentations. It is commonly used for academic presentations, lectures, seminars, and technical talks.

Each slide is usually created inside a `frame` environment.

## 2. Basic Structure of a Beamer Presentation

A minimal Beamer presentation looks like this:

```latex
\documentclass{beamer}

\title{My Presentation}
\author{Student Name}
\institute{MNIT Jaipur}
\date{\today}

\begin{document}

\begin{frame}
    \titlepage
\end{frame}

\begin{frame}{Introduction}
    This is my first slide.
\end{frame}

\end{document}
```

## 3. Important Commands

- `\title{}`: Sets the presentation title.
- `\author{}`: Specifies the author's name.
- `\institute{}`: Specifies the institution.
- `\date{}`: Sets the presentation date.
- `\begin{frame}{Title}`: Starts a new slide.
- `\titlepage`: Displays the title slide.
- `\frametitle{}`: Sets the title of a slide.

## 4. Creating Lists

Beamer supports both unordered and ordered lists.

**Unordered List:**

```latex
\begin{frame}{Objectives}
    \begin{itemize}
        \item Understand the topic
        \item Study an example
        \item Review the results
    \end{itemize}
\end{frame}
```

**Ordered List:**

```latex
\begin{frame}{Steps}
    \begin{enumerate}
        \item Introduction
        \item Explanation
        \item Conclusion
    \end{enumerate}
\end{frame}
```

## 5. Themes

Themes control the overall appearance of a presentation.

Example:

```latex
\usetheme{Madrid}
```

Other commonly used themes include:

- `CambridgeUS`
- `Warsaw`
- `Berlin`
- `Singapore`
- `Pittsburgh`

The theme command is generally placed in the preamble.

## 6. Creating Columns

The `columns` environment is used to divide a slide into multiple sections.

```latex
\begin{frame}{Two Columns}

\begin{columns}

    \column{0.48\textwidth}
    Left-side content

    \column{0.48\textwidth}
    Right-side content

\end{columns}

\end{frame}
```

## 7. Adding Images

To insert images, use the `graphicx` package in the preamble.

```latex
\usepackage{graphicx}
```

Example:

```latex
\begin{frame}{Diagram}
    \centering
    \includegraphics[width=0.7\textwidth]{diagram.png}
\end{frame}
```

## 8. Overlays and Step-by-Step Presentation

Overlays allow content to appear gradually on a slide.

```latex
\begin{frame}{Important Points