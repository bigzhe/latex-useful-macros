# latex-useful-macros
Useful macros in LaTeX

## Additional packages

```tex
\usepackage{amssymb}
\usepackage{relsize}
\usepackage{mathtools}
```

## Micros used in the database report

```tex
\newcommand{\D}{\mathbf{D}}
\newcommand{\calA}{\mathcal{A}}
\newcommand{\calC}{\mathcal{C}}
\newcommand{\calP}{\mathcal{P}}
\newcommand{\calH}{\mathcal{H}}
\newcommand{\calT}{\mathcal{T}}
\newcommand{\calV}{\mathcal{V}}
\newcommand{\calX}{\mathcal{X}}
\newcommand{\calE}{\mathcal{E}}
\newcommand{\calU}{\mathcal{U}}
\newcommand{\calD}{\mathcal{D}}
\newcommand{\bfx}{\mathbf{x}}
\newcommand{\bfzero}{\mathbf{0}}
\newcommand{\bfone}{\mathbf{1}}
\newcommand{\set}[1]{\{#1\}}
\newcommand{\tuple}[1]{\langle#1\rangle}
\newcommand{\bigO}[1]{\mathcal{O}(#1)}
\newcommand{\hatO}[1]{\tilde{\mathcal{O}}(#1)}
% \newcommand{\cal}[1]{\mathcal{#1}}
```

## Example paragraphs

### Config

```tex
\setcounter{secnumdepth}{3}
\setcounter{tocdepth}{3}

\newcommand\tab[1][0.22cm]{\hspace*{#1}}
\newcounter{example}[section]
\newenvironment{example}[1][]{\refstepcounter{example}\vspace{5mm}\noindent
   \textbf{Example~\arabic{chapter}.\theexample} \tab \rmfamily}{\medskip}
```

### Usage

```tex
\begin{example}
\label{example:first}
This is the content of the example
\end{example}

The Example \ref{example:first} shows ...
```