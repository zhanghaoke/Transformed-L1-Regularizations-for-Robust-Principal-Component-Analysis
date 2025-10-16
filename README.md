# Transformed L1 Regularizations for Robust PCA

This repository contains the official MATLAB implementation for the paper:  
**"Transformed $\ell_1$ Regularizations for Robust Principal Component Analysis: Toward a Fine-Grained Understanding"**  

**Authors:** Kun Zhao, Haoke Zhang, Jiayi Wang, Yifei Lou  
Read the full paper on arXiv https://arxiv.org/pdf/2510.03624?

---

This project addresses the **Robust Principal Component Analysis (RPCA)** problem, which decomposes an observation matrix into a **low-rank matrix (background)** and a **sparse matrix (noise/outliers)**.

Traditional methods:** use the **nuclear norm** and **$\ell_1$ norm**.  
Our approach:** introduces **Transformed $\ell_1$ (TL1)** regularization terms for both the low-rank and sparse components.

The TL1 regularization provides a tighter approximation to the rank function and $\ell_0$ norm, achieving better recovery performance both theoretically and empirically, especially under **non-uniform sampling** conditions.

---

## How to Run

### 1. Synthetic Data
Run the `simulation.m` script to reproduce the numerical experiments in the paper.  
This compares our proposed TL1 model with the traditional nuclear norm model.

### 1. Synthetic Data
Run the video.m script to process the shoppingmall.mat video data, achieving background–foreground separation.
