Constraint-Weighted Growth
Monotone Scaling Modulation and Nonlinear Transport Suppression

This repository contains the simulation code accompanying the manuscript:

Constraint-Weighted Growth Induces Monotone Scaling Modulation and Nonlinear Transport Suppression: A Structural Mechanism in Directed Stochastic Growth
Georgios Kouvidis (2026)

The repository provides two primary computational artifacts corresponding to the empirical and illustrative components of the paper.

Repository Structure
constraint-weighted-growth/
│
├── README.md
├── requirements.txt
└── notebooks/
    ├── 01_growth_scaling.ipynb
    └── 02_transport_surrogate.ipynb
1. Growth Scaling Simulation

Notebook: 01_growth_scaling.ipynb

This notebook generates the primary empirical results reported in Section 3 of the manuscript.

It implements:

Directed acyclic graph (DAG) growth

Admissible extension generation

Increment dispersion computation

Softmax compatibility weighting

Time-series evaluation of normalized out-degree dispersion

Log–log regression to estimate scaling exponent α(λ)

Control experiments (uniform and shuffled penalty)

Outputs include:

Φ(t) time series

Estimated scaling exponents α(λ)

Standard deviations across realizations

Goodness-of-fit (R²)

This notebook reproduces the exponent table reported in the paper.

2. Transport Surrogate and Dynamical Embedding

Notebook: 02_transport_surrogate.ipynb

This notebook implements the coarse-grained transport proxy and illustrative dynamical embedding described in Sections 4–5.

It includes:

Conditional increment distribution under exponential penalty

Computation of effective transport proxy χ_eff(λ, g)

Gradient elasticity evaluation

Cutoff activation analysis

Illustrative nonlinear diffusion surrogate with regulator dynamics

This notebook demonstrates the structural suppression mechanism induced by exponential tail truncation.

Reproducibility

All simulations are deterministic given the random seed.

To reproduce results:

Install dependencies:

pip install -r requirements.txt

Run notebooks sequentially from top to bottom.

Each discrete growth step corresponds to one unit time increment in the coarse-grained description.

Code Versions and Archival

Each notebook corresponds to an archived Zenodo release:

Growth scaling implementation → DOI: (to be assigned)

Transport surrogate implementation → DOI: (to be assigned)

The GitHub repository reflects the development version; Zenodo releases provide frozen, citable snapshots used in the manuscript.

License

This project is released under the MIT License (or specify your license here).

Citation

If you use this code, please cite:

Kouvidis, G. (2026).
Constraint-Weighted Growth Induces Monotone Scaling Modulation and Nonlinear Transport Suppression.

and the corresponding Zenodo code release.

Notes

This repository implements a structural stochastic growth mechanism.
It does not model specific physical transport systems; the transport surrogate is illustrative and structural in nature.
