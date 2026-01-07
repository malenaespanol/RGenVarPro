# RGenVarPro and iRGenVarPro

This repository contains reference Python implementations and Jupyter notebooks corresponding to the paper

> **Variable Projection Methods for Solving Regularized Separable Inverse Problems with Applications to Semi-Blind Image Deblurring**  
> D. B. Comerso Salzer, M. I. Español, and G. Jeronimo.

The code was used to generate the numerical experiments reported in the paper.

---

## Project Description

The repository provides implementations of variable projection methods for separable nonlinear least squares problems with regularization on both the linear and nonlinear variables.

In particular, it includes:

- **RGenVarPro**: a quasi-Newton variable projection method for problems with  
  - general-form Tikhonov regularization on the linear variables, and  
  - differentiable regularization on the nonlinear parameters.

- **iRGenVarPro**: an inexact variant in which the inner linear subproblems are solved approximately using LSQR with adaptive stopping tolerances.

The numerical examples focus on semi-blind image deblurring with low-dimensional parameterizations of the blur operator, as described in the paper.

---

## Contents of the Repository

- **Python source files**  
  Core implementations of the RGenVarPro and iRGenVarPro algorithms.

- **Jupyter notebook (`.ipynb`)**  
  A notebook used to run the numerical experiments and generate the figures reported in the paper.

The notebook is intended to illustrate usage of the methods and to reproduce the reported results.

---

## Software Requirements

The code is written in **Python** and was tested using:

- Python 3.10+
- NumPy
- SciPy (for LSQR and linear algebra routines)
- Matplotlib (for visualization)

The experiments were executed on Google Colab, but the code can also be run locally with a standard Python installation.

---

## Reproducibility

The Jupyter notebook included in this repository reproduces the numerical results presented in the paper, using the parameter values and experimental settings described therein.

The code is provided for **research and reproducibility purposes** and is not optimized for performance or large-scale production use.

---

## Citation

If you use this code, please cite the associated paper:

