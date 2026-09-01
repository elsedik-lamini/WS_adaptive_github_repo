# WS_adaptive: companion code

Companion code and notebook for the paper **"WS_adaptive: A Saturation-Free Generalization of the WS Rank Similarity Coefficient for Large-Scale Rankings"** (El-Sedik Lamini, RECITS Laboratory, USTHB — submitted to *Information Processing Letters*).

This repository contains a single Jupyter notebook, `WS_adaptive_notebook.ipynb`, which is the complete, reproducible source of **every number, table, and figure reported in the paper**. Running the notebook top to bottom regenerates all results from scratch — no external data files are needed.

## Contents

- **Part 1** (Sections 1-9): implements `WS` (Sałabun & Urbaniak, 2020) and the proposed `WS_adaptive` coefficient; visualizes the saturation proof; reproduces the small-N and large-N validation tables and the saturation curve.
- **Part 2** (Sections 10-16): distributional behavior of `WS`, `WS_adaptive`, `WS_dra`, Spearman's rho and Kendall's tau under uniformly random rankings; numerical verification of the paper's Propositions 2 and 3; the concentration analysis; and the practical usage-guide calibration.

## Requirements

Python >= 3.9, with:

```
pip install -r requirements.txt
```

## Usage

```
jupyter notebook WS_adaptive_notebook.ipynb
```

Run all cells top to bottom. Figures are written to `./figures/` as both PDF (for LaTeX) and PNG; tables are written as CSV. Total runtime is a few minutes (the concentration analysis in Section 14 is the slowest cell).

## Citation

If you use this code, please cite the paper:

```
El-Sedik Lamini. "WS_adaptive: A Saturation-Free Generalization of the WS Rank
Similarity Coefficient for Large-Scale Rankings." Information Processing
Letters (submitted).
```

A citable archive of this repository is available on Zenodo: DOI: 10.5281/zenodo.22239268.

## License

Released under the MIT License (see `LICENSE`).
