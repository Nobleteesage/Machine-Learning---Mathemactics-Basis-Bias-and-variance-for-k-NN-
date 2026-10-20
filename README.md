# Machine Learning: Mathematical Basis

Solutions to some projects in *Machine Learning: Mathematical Basis*, MSc Applied Mathematics and Informatics, Sfedu (2026).

**Author:** Goriola-Obafemi Babatunde Sukanmi ([ORCID 0009-0000-2865-5242](https://orcid.org/0009-0000-2865-5242))

## Contents

| Folder | Topic | Notebook |
|---|---|---|
| `HW3/` | Local Methods: bias and variance of k-NN, curse of dimensionality | [HW3_Local_Methods.ipynb](HW3/HW3_Local_Methods.ipynb) |

## HW3. Local Methods

**Part I. Bias and variance for k-NN.** Monte Carlo study (B = 1000) of the k-NN estimator for $f^*(x)=\sin(2\pi x)+0.5x$ with fixed design (n = 250). Empirical conditional mean and variance are compared with the theoretical formulas, and the bias–variance tradeoff is plotted at an interior point (x = 0.50) and near the boundary (x = 0.05).

**Part II. How much data does high dimension cost?** Required sample size so that the 10th nearest neighbour of the cube centre lies at distance 0.3, for d from 1 to 15, verified by simulation for d = 2, 5, 8.

**Key results**
* Best k: 40 at x = 0.50, 20 at x = 0.05 (smaller near the boundary because of one sided neighbourhoods)
* Required n grows from 17 (d = 1) to about 1.8 × 10⁹ (d = 15)
* Halving the neighbourhood radius multiplies the required sample size by 2ᵈ

## How to run

Open the notebook in Google Colab or Jupyter and run all cells. Requirements: `numpy`, `pandas`, `matplotlib`. All randomness uses `SEED = 2026`, so results are reproducible.
