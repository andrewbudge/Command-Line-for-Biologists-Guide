# Command Line for Biologists — LaTeX source

*A Practical Guide to the Terminal, Tools, and Reproducible Workflows*

## Structure

```
book/
├── main.tex              # Entry point — defines the document & includes chapters
├── preamble.tex          # All packages, styles, custom commands
├── chapters/
│   ├── 00_foreword.tex
│   ├── 01_introduction.tex
│   └── 02_terminal.tex
└── .gitignore
```

## Building

Run `pdflatex` twice (the first pass builds the table of contents, the second
fills in the page numbers):

```bash
pdflatex main.tex
pdflatex main.tex
```

Or use `latexmk` which figures out how many passes are needed:

```bash
latexmk -pdf main.tex
```

To clean up auxiliary files:

```bash
latexmk -c        # keeps the PDF
latexmk -C        # also removes the PDF
```

## Adding a new chapter

1. Create `chapters/03_your_chapter.tex` starting with `\chapter{...}`.
2. Add `\include{chapters/03_your_chapter}` to `main.tex` (no `.tex` extension).
3. Compile.

## Working on just one chapter (fast iteration)

Uncomment the `\includeonly{}` line in `main.tex` and list only the chapter you
want to compile. Cross-references and the TOC will still know the others exist.

## Custom things this project defines

- `\code{...}` — inline code (just `\texttt`, escape `$`, `_`, `#`, `%`, `&`, `~`, `\` if needed)
- `\begin{reflection} ... \end{reflection}` — blue callout box for reflection prompts
- `lstlisting` environments are styled as bash shell sessions by default. The
  `$` at the start of a line renders in blue to highlight prompts.
