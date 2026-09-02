# The Complete Bayesian Modeling Masterclass in R
### *From Classical Frequentist Estimation to Production Hamiltonian Monte Carlo*

This repository contains a comprehensive 4-part hands-on curriculum for parameter estimation, convergence diagnosis, and posterior prediction using **R**.

---

## 📚 Curriculum Structure

| Notebook | Title | Core Concept | Primary Tools |
| :--- | :--- | :--- | :--- |
| **[00_START_HERE.ipynb](00_START_HERE.ipynb)** | **Course Syllabus & Overview** | Course roadmap, comparison matrices, and quick-start links | Jupyter |
| **[01_frequentist_vs_grid_approximation.ipynb](01_frequentist_vs_grid_approximation.ipynb)** | **Foundations: Frequentist vs. Grid Approx** | Generative models, CI vs. Credible Intervals, 7 Deep Dives, Prior sensitivity & shrinkage | `t.test()`, `expand.grid()`, `dnorm()` |
| **[02_quadratic_laplace_approximation.ipynb](02_quadratic_laplace_approximation.ipynb)** | **Rapid Prototyping: Quadratic (Laplace) Approx** | Parabolic log-posteriors, inverting the Hessian matrix, Multivariate Normal draws | `optim(..., hessian=TRUE)`, `rethinking::quap()` |
| **[03_mcmc_mechanics_from_scratch.ipynb](03_mcmc_mechanics_from_scratch.ipynb)** | **First Principles: MCMC Mechanics from Scratch** | Detailed balance, 3-step Metropolis rule, step-size tuning failure modes, autocorrelation decay | Pure Base R (`rnorm()`, `runif()`, `acf()`) |
| **[04_mcmc_production_diagnostics.ipynb](04_mcmc_production_diagnostics.ipynb)** | **Production Scale: Multi-Chain MCMC & Stan** | Multi-chain convergence, Gelman-Rubin $\hat{R}$, Effective Sample Size ($ESS$), HMC physics, PSIS-LOO model comparison | `coda`, `rethinking::ulam()`, `loo` |

---

## 🛠️ Environment Prerequisites

- **R version**: 4.6.1+
- **R Packages**: `rethinking`, `coda`, `loo`, `MASS`, `IRkernel`
- **Jupyter**: Jupyter Notebook / JupyterLab with `ir` kernel support

---

## 🚀 Getting Started

Launch your Jupyter server pointing to the repository root:
```bash
jupyter notebook --notebook-dir="C:\Users\tarob\scratch\r"
```
Open **`00_START_HERE.ipynb`** in your browser to begin.
