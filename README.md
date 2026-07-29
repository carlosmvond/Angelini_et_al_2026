# Angelini_et_al_2026

Code and data reproducing the figures of

> M. Angelini, C. Hermosilla, and C. Martínez,
> *Optimal switching time in inducible bioprocesses with growth and production trade-offs*, 2026.

Each notebook runs in Google Colab or locally and reads the data files directly from this repository, so no manual upload is needed.

## Contents

- **`Angelini_et_al_2026_fitting_model.ipynb`** — reproduces **Figure 1**: calibrates the kinetic model against optogenetic *E. coli* data and reports the parameters of Table 1.
- **`Angelini_et_al_2026_heatmap.ipynb`** — reproduces **Figure 2**: optimal switching time and objective value over the `(η, γ)` plane, with the threshold `R = η/γ = 1`.
- **`Angelini_et_al_2026_trajectories.ipynb`** — reproduces **Figure 3**: optimal trajectories for two cases, one on each side of the threshold.
- **`sample100KJJ.csv`** — optimal objective value over the `(η, γ)` grid (input to Figure 2).
- **`sample100KTL.csv`** — optimal switching time over the `(η, γ)` grid (input to Figure 2).

The CSV files are `100 × 100` grids over `η, γ ∈ [0.01, 1]`, with `η` in rows and `γ` in columns.

## Requirements

`numpy`, `scipy`, `matplotlib`, and `lmfit` (Figure 1), `casadi` (Figure 3). The notebooks install `lmfit` and `casadi` automatically if needed.

## Data

The experimental data in Figure 1 are from S. Espinel-Ríos et al., *Process Biochemistry*, 143 (2024), pp. 174–185.

## License

See [`LICENSE`](LICENSE).
