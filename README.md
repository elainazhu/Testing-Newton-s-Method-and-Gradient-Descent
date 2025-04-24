# Testing Optimizers

This repository implements a variety of classical optimization algorithms to train a linear classifier with **exponential loss** on a steganography dataset (1000 cover images vs. 1000 stego images, each with 136 standardized features plus a bias term).

## Files

- **cm-sheet5-X.txt** – Feature matrix `X` (2000×137), one tab-delimited row per sample.  Last column is constant 1 (bias).
- **cm-sheet5-y.txt** – Label vector `y` (2000 entries of ±1).
- **exp\_loss\_optimizers.py** / **main.ipynb** – Implementations of seven optimizers; prints final loss, iteration count, and **accuracy** on the full dataset.

## Optimizers (to be) Implemented

1. Newton’s Method
2. Quasi-Newton (BFGS)
3. Limited-memory BFGS (L‑BFGS)
4. Batch Gradient Descent
5. Nonlinear Conjugate Gradient (Polak–Ribiere)
6. Stochastic Gradient Descent (SGD)
7. Minibatch Gradient Descent

## Results (Accuracy on Full Dataset)

| Method                                | Accuracy |
| ------------------------------------- | -------- |
| Newton’s Method                       | 0.9480   |
| Batch Gradient Descent (1000iters)    | 0.9240   |
| Batch Gradient Descent (10000iters)   | 0.9460   |
| Quasi-Newton (BFGS)                   | *TBD*    |
| Limited-memory BFGS (L‑BFGS)          | *TBD*    |
| Nonlinear Conjugate Gradient (CG)     | *TBD*    |
| Stochastic Gradient Descent (SGD)     | *TBD*    |
| Minibatch Gradient Descent (batch=64) | *TBD*    |
