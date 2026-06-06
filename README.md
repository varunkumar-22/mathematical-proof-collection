# Mathematical Proof Collection

A curated collection of mathematical proofs and derivations written in LaTeX. The goal of this project is to demonstrate rigorous mathematical reasoning alongside clean, professional document preparation.

Each proof is written to be readable and self-contained, using standard theorem, definition, and proof environments so the structure of each argument is easy to follow.

## What's inside

The collection compiles into a single typeset document with a title page and table of contents. Individual proofs live as separate LaTeX source files so they can be edited and reviewed independently.

Planned topics include classic results such as the AM-GM inequality, the binomial theorem, Euclid's algorithm for the greatest common divisor, and proof by mathematical induction.

## Repository layout

```
mathematical-proof-collection/
├── README.md              Project overview
├── main.tex               Master document (title page, TOC, includes)
├── proofs/                Individual proof source files
├── images/                Figures and diagrams
└── output/                Compiled PDF output
```

## Building the document

You need a LaTeX distribution installed (TeX Live, MiKTeX, or MacTeX). To compile the master document into a PDF:

```
pdflatex main.tex
pdflatex main.tex
```

Running the command twice ensures the table of contents and cross-references resolve correctly. The resulting PDF can be placed in the `output/` folder.

If you prefer an automated build, `latexmk` handles the multiple passes for you:

```
latexmk -pdf main.tex
```

## Adding a new proof

Create a new `.tex` file inside the `proofs/` folder containing the body of your proof, then add an `\input` line for it in `main.tex`. Keeping each proof in its own file makes the collection easy to extend over time.

## License

This project is shared for educational purposes. Feel free to read, learn from, and build on it.
