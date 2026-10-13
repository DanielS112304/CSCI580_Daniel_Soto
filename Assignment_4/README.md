# CSCI 580 — Assignment 4: TSP with SA and GA

This directory contains a completed and executed notebook, the technical report, figures, and machine-readable experiment results.

## Run

1. Install Python 3 and Jupyter or use Google Colab.
2. Install matplotlib (`pip install matplotlib notebook`).
3. Open `TSP_SA_GA_Completed.ipynb` and choose **Run All**.
4. Inspect the embedded execution output and Part 6 graphs. The notebook also writes `figures/` and `experiment_results.json` relative to its working directory.

## Contents

- `TSP_SA_GA_Completed.ipynb`: fully implemented SA and GA functions and experiment cells, with stored outputs.
- `CSCI580_Assignment4_Technical_Report.pdf`: technical report with algorithms, experiment graphs, and Part 6 discussion.
- `figures/`: generated tour plots, convergence comparisons, and diagnostics.
- `experiment_results.json`: results from notebook execution.

## Default instance and settings

40 cities (seed 7). SA: 20,000 iterations, initial temperature 0.2, alpha 0.9995, seed 123. GA: 200 individuals, 400 generations, tournament 5, 90% crossover, 20% mutation, 5 elites, seed 999. Both use the nearest-neighbor reference. There are five runs varying each algorithm's random seed.

## Important notes

The Genetic Algorithm performs substantially more tour-length evaluations than SA with the default settings. The report compares both algorithms using actual evaluations, not just iteration or generation indices. Notebook output is reproduced with the specific seeds above.
