# IC50 Curve Fitter

Static, browser-based IC50 curve fitting tool for teaching.

## Model

3-parameter inhibitory dose-response model:

`Y = Top / (1 + 10^((X - logIC50) * HillSlope))`

- Bottom is fixed at 0.
- Top, logIC50, and Hill slope are fitted by nonlinear least squares.
- Input X is log10(dose).
- Input Y is % Vehicle.
- Replicates are fitted as individual observations.

## GitHub Pages

This repository is designed to run without a server. After enabling GitHub Pages from the `main` branch root, the app URL is:

`https://elisbeth.github.io/lc50cal/`
