# MgSiO3-H Equation of State Lookup Table

This repository contains a tabulated equation of state (EOS) for liquid MgSiO3-H mixtures used in the accompanying study. The table was constructed from fitted Helmholtz free-energy surfaces for the MgSiO3-H system and is formatted for use in planetary interior calculations.

## Table Info

The table spans hydrogen contents from approximately 0 to 3.86 wt% H, corresponding to approximately 0 to 4 H atoms per MgSiO3 formula unit.

The pressure-temperature coverage is:

- **1–4 GPa:** 3000–6000 K, with 1 GPa pressure spacing
- **5–800 GPa:** 3000–10,000 K, with 5 GPa pressure spacing
- **Temperature spacing:** 50 K throughout

The underlying first-principles simulations used to construct the EOS were performed primarily over **4000–8000 K** and approximately **3–650 GPa**. The lookup table extends somewhat beyond this range to provide continuous coverage for planetary modeling; these extensions were chosen conservatively.

## Columns

| Column | Description |
|---|---|
| `H_wt_pct` | Total hydrogen concentration (wt%) |
| `P_GPa` | Pressure (GPa) |
| `T_K` | Temperature (K) |
| `rho_gcc` | Density (g cm^-3) |
| `H_kJ_g` | Specific enthalpy (kJ g^-1) |
| `S_J_g_K` | Specific entropy (J g^-1 K^-1) |
| `alpha_1e5` | Thermal expansivity in units of 10^-5 K^-1 |
| `cp_J_g_K` | Isobaric heat capacity, Cp (J g^-1 K^-1) |
| `KS_GPa` | Adiabatic bulk modulus, KS (GPa) |
| `rho0_gcc` | Reference density (g cm^-3) |
| `eta` | Compression ratio, rho/rho0 |
| `gamma` | Gruneisen parameter |


## File format

The lookup table is provided as a comma-separated values (`.csv`) file. Each row corresponds to a single hydrogen-composition, pressure, and temperature state.

For details of the EOS fitting procedure, thermodynamic formulation, and first-principles calculations, please refer to the accompanying paper.
