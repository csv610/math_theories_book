# Mathematics Theories in Nutshell

**A Friendly Guide to Mathematical Theories**  
*A survey with worked examples and routes for further study*

**Author:** Chaman Singh Verma

---

A compact survey of 91 mathematical theories, each presented in a single chapter with an intuitive opening, core theory, historical context, worked examples, and sample questions. Twelve worked modules at the end provide hands-on practice with guided exercises.

## What's Inside

| Component | Description |
|-----------|-------------|
| **91 chapters** | One per theory, from algebraic geometry to wheel theory, covering the full [Wikipedia list of mathematical theories](https://en.wikipedia.org/wiki/List_of_mathematical_theories) |
| **12 worked modules** | Probability, statistics, graph theory, coding, group theory, topology, dynamical systems, number theory, approximation, computation, game theory, algebraic geometry |
| **Front matter** | "Start here" guide, study advice, toolbox of definitions, map of connections, recommended reading |
| **Per-chapter structure** | Intuitive overview → Core theory → Important theorems → Glossary → Applications → Sample questions with solutions → References |
| **Student toolbox** | Plain-English definitions of 18 key terms (algebra through vector) |

## Who This Book Is For

- **Curious readers** with high-school math who want to see what university mathematics looks like
- **Undergraduates** who need a compact reference across many theories
- **Instructors** looking for short, self-contained chapter summaries

### Reading paths

- **New to proofs?** Start with the 12 worked modules (Modules 1–12). Each takes ~20 minutes.
- **Know calculus and proof techniques?** Read any chapter in any order. The intuitive opening gives the idea; the formal section gives the precision.

## Building the PDF

Requires a LaTeX distribution (TeX Live, MiKTeX, or MacTeX).

```bash
pdflatex math_theories.tex
pdflatex math_theories.tex   # second pass for references and TOC
```

### Dependencies

The document uses standard LaTeX packages: `amsmath`, `amssymb`, `hyperref`, `enumitem`, `tikz`, `pgfplots`, `geometry`, `tocloft`, and others listed in the preamble. All are included in TeX Live.

## Repository Structure

```
.
├── math_theories.tex          # Main document (preamble, macros, front/back matter)
├── chapters/                  # 91 chapter files (alphabetical order)
│   ├── algebraic_geometry.tex
│   ├── graph_theory.tex
│   ├── group_theory.tex
│   ├── knot_theory.tex
│   ├── number_theory.tex
│   ├── probability_theory.tex
│   ├── topology.tex
│   └── ... (91 files total)
└── figures/                   # TikZ figures referenced by chapters
```

## Highlights

- **Intuitive before formal** — every chapter opens with a problem, not a definition
- **Worked examples in theorems** — Lagrange's theorem with S₃, Euler characteristic on a cube, Bayes' rule with a medical test
- **Sample questions with solutions** — 5 per chapter, mathematically precise with worked answers
- **Glossary per chapter** — technical terms defined in context
- **Cross-references** — each chapter lists what it depends on and what it helps understand

## License

The explanations and examples are original. Chapter titles follow the [Wikipedia list of mathematical theories](https://en.wikipedia.org/wiki/List_of_mathematical_theories) (CC BY-SA 4.0).

## Building

```bash
# Full build (two passes for cross-references)
pdflatex -interaction=nonstopmode math_theories.tex && \
pdflatex -interaction=nonstopmode math_theories.tex
```

Output: `math_theories.pdf` (~850 pages).

## Contributing

This is a personal reference book. Issues and suggestions are welcome via GitHub Issues or pull requests.
