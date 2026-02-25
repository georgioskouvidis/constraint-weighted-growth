# Constraint-Weighted Growth: Tunable Scaling in Directed Networks

This repository contains the full simulation code accompanying the paper:

**Kouvidis (2026)**  
Constraint-Weighted Growth as a Mechanism for Tunable Scaling Regimes in Directed Networks.

## Overview

We study a directed acyclic graph (DAG) growth model where candidate extensions are selected using a softmax kernel penalizing increases in normalized structural heterogeneity:

P_lambda(e | G) ∝ exp( -lambda * ΔΦ )

The model demonstrates continuous exponent modulation of the form:

Φ(t) ~ t^α(lambda)

with α decreasing monotonically as lambda increases.

## Files

- `constraint_weighted_growth.ipynb` — Full simulation notebook
- `requirements.txt` — Python dependencies

## Reproducibility

All simulations were run with fixed random seeds.

To reproduce:

1. Install dependencies:
   pip install -r requirements.txt

2. Run the notebook sequentially.

## Parameter Defaults

- m = [your value]
- T = 5000
- lambda ∈ [0, 10]
- Transient cutoff t0 = 500
- N = 10 runs

## Citation

If using this code, please cite:

Kouvidis, G. (2026). Constraint-Weighted Growth as a Mechanism for Tunable Scaling Regimes in Directed Networks.

Zenodo DOI: [to be inserted]

## License

MIT License.
