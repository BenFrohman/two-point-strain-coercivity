<!-- Copyright (c) 2026 Benjamin Stanley Frohman. Licensed under Apache-2.0. -->
# Two-Point Strain Coercivity Is Not Free

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23627618.svg)](https://doi.org/10.5281/zenodo.23627618)

**Author:** Benjamin Stanley Frohman  
**Date:** 11 September 2026  
**Repository:** https://github.com/BenFrohman/two-point-strain-coercivity  
**Zenodo DOI:** [`10.5281/zenodo.23627618`](https://doi.org/10.5281/zenodo.23627618)

**Claim, stated directly:** The two-point pairing that would convert Constantin–Fefferman from a hypothesis into a theorem is false at kinematic strength. The Biot–Savart estimate along unmodified Navier–Stokes, without a Lipschitz bound on the vorticity direction, ends at \(C_{\mathrm{CZ}}M\), not at an \(M\)-independent \(-\gamma\).

This is a Zenodo-ready source package. It is not a proof of global regularity.

## Files

| File | Role |
|---|---|
| `README.md` | This file |
| `two_point_strain_coercivity.tex` | LaTeX source of the note |
| `two_point_strain_coercivity.md` | Markdown source of the same note |
| `two_point_strain_coercivity.pdf` | Compile locally with `pdflatex` |
| `ZENODO.md` | Deposit instructions |
| `LICENSE` | Apache-2.0 |

## Compile

```bash
pdflatex two_point_strain_coercivity.tex
pdflatex two_point_strain_coercivity.tex
```

## What is proved

1. **Theorem A.** Conjecture \((\star)_\rho\) fails for general smooth divergence-free fields on \(\mathbb{T}^3\), hence for Navier–Stokes initial data. The counterexample is intermediate-axis alignment with a slow tilt toward the principal stretching axis. Max-axis alignment is withdrawn: it gives the good sign.
2. **Theorem B.** After Biot–Savart and absorption without Lipschitz control of \(\xi\), the last line is \(C_*=C_{\mathrm{CZ}}M\) (honestly \(CM\log(2+\|u\|_{H^s})\)), not \(-\gamma\).
3. Global (no \(|x-y|\) cutoff) two-point coercivity already fails on exact two-dimensional Navier–Stokes.

## What is not proved

\((\star)_\rho\) along an unmodified Navier–Stokes trajectory with \(K_\varepsilon\) independent of \(M(t)=\|\omega\|_\infty\). That statement is Constantin–Fefferman with the hypothesis discharged. It is the regularity problem.

## Responsibility

I, Benjamin Stanley Frohman, take responsibility for this note. The equation is unmodified 3D incompressible Navier–Stokes. No 2-form and no weight in front of stretching are used.

## License

Copyright (c) 2026 Benjamin Stanley Frohman. Licensed under the Apache License, Version 2.0 (`LICENSE`, `NOTICE`).
Copies already received under CC BY 4.0 keep that grant.
Zenodo DOI: [`10.5281/zenodo.23627618`](https://doi.org/10.5281/zenodo.23627618).

## Suggested citation

Frohman, B. S. (2026). *Two-Point Strain Coercivity Is Not Free: The Intermediate-Axis Counterexample and the Calderón–Zygmund Remainder \(C_{\mathrm{CZ}}\|\omega\|_\infty\) for Unmodified Three-Dimensional Navier–Stokes*. Zenodo draft, 11 September 2026. https://github.com/BenFrohman/two-point-strain-coercivity
