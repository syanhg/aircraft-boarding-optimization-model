# Aircraft Boarding Optimization Model

This repository contains the LaTeX code for the conclusion and evaluation sections of a mathematical modeling study on optimizing passenger boarding in aircraft, with a specific focus on the Boeing 737-800 single-aisle configuration.

## Repository Contents

- `conclusion.tex`: Comprehensive conclusion section summarizing key findings, theoretical implications, practical applications, and final remarks
- `evaluation.tex`: Critical evaluation of the methodology, strengths, limitations, and future research directions, including a TikZ diagram comparing boarding strategies
- `main.tex`: Main LaTeX document that includes both sections in a properly formatted document

## Highlights

The study compares three boarding strategies:
- Back-to-front strategy (traditional approach)
- Outside-in strategy (window-middle-aisle)
- Hybrid strategy (combining row and seat position optimization)

Key findings indicate that both the outside-in and hybrid strategies outperform the traditional back-to-front approach, reducing boarding time by approximately 16.7% (from 12.0 to 10.0 minutes).

## Mathematical Framework

The study employs a first-order differential equation model that treats passenger flow as a continuous fluid system:

```
dN(t)/dt = -k · N(t) · (1 - C(t))
```

Where:
- N(t) is the number of passengers remaining to be seated at time t
- k is the efficiency coefficient
- C(t) is a congestion factor that models interference between passengers

## Compiling the Document

To compile the LaTeX document:

1. Ensure you have a LaTeX distribution installed (e.g., TeX Live, MiKTeX)
2. Make sure the required packages are installed (amsmath, pgfplots, tikz, etc.)
3. Compile using pdfLaTeX:
   ```
   pdflatex main.tex
   pdflatex main.tex  # Run twice for proper references and ToC
   ```

## Visualization

The evaluation section includes a TikZ diagram that visualizes the comparative performance of the three boarding strategies, illustrating how passenger count decreases over time under each approach.

## Applications

The findings of this research have practical applications for airlines seeking to optimize turnaround times, improve operational efficiency, enhance passenger experience, and reduce costs associated with aircraft boarding procedures.