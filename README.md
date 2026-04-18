# Transformed L1 Regularizations for Robust PCA

This repository contains the official MATLAB implementation for the paper:  
**"Transformed $\ell_1$ Regularizations for Robust Principal Component Analysis: Toward a Fine-Grained Understanding"**  

**Authors:** Kun Zhao, Haoke Zhang, Jiayi Wang, and Yifei Lou  
Read the full paper on arXiv https://arxiv.org/pdf/2510.03624

---

This project addresses the **Robust Principal Component Analysis (RPCA)** problem, which decomposes an observation matrix (a high-dimensional data) into a **low-rank matrix** (background) and a **sparse matrix** (noise or outliers) under general (potentially non-uniform) sampling schemes, leveraging nonconvex TL1 regularization to better approximate rank and sparsity compared to classical convex approaches. An efficient ADMM-based optimization algorithm is developed to solve the resulting problem, with tailored updates for both singular values (low-rank structure) and entry-wise sparsity. The implementation includes reproducible experiments on synthetic and real datasets, demonstrating improved recovery accuracy, robustness to missing data, and enhanced control over rank and sparsity relative to standard nuclear norm and $\ell_1$-based methods.

---

## How to Run

### 1. Synthetic Data
Run the `simulation.m` script to reproduce the numerical experiments in the paper.  
This compares our proposed TL1 model with the traditional L1 model.

### 2. Video Data
Run the `video.m` script to process the `shoppingmall.mat` video data to achieve background–foreground separation.
