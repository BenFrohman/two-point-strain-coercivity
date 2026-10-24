# Zenodo Deposit Cheat-Sheet

Mint the DOI by uploading `two_point_strain_coercivity.pdf`, `two_point_strain_coercivity.tex`, `two_point_strain_coercivity.md`, `LICENSE`, `NOTICE`, and `CITATION.cff` to <https://zenodo.org/deposit/new> (or via the GitHub → Zenodo webhook).

| Field | Value |
|---|---|
| **Upload type** | Publication → Preprint |
| **Title** | On Local Two-Point Strain Coercivity in the 3D Vorticity Equation |
| **Creator** | Frohman, Benjamin Stanley (ORCID: `0009-0006-7068-3718`, Independent Researcher) |
| **License** | Apache License 2.0 (`Apache-2.0`) |
| **Version** | `1.0.0` |
| **Subjects / Keywords** | `35Q30`, `76D03`, `Navier-Stokes`, `vorticity stretching`, `Constantin-Fefferman`, `two-point kernel` |
| **Description** | Short note showing that a conjectured local two-point strain coercivity inequality for the 3D vorticity equation fails for general smooth divergence-free fields on T^3, and that the Biot–Savart / Calderón–Zygmund closure without Lipschitz control of the direction field yields a positive right-hand side `C_* = C_CZ * M` rather than `-gamma`. |

After Zenodo mints `10.5281/zenodo.<RECORD_ID>`:

1. Replace the placeholder badge in `README.md` with:
   ```markdown
   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.<RECORD_ID>.svg)](https://doi.org/10.5281/zenodo.<RECORD_ID>)
   ```
2. Uncomment and fill `doi: "10.5281/zenodo.<RECORD_ID>"` in `CITATION.cff`.
