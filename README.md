# Figure data (CSV) for: Scalable Suppression of XY Crosstalk by Pulse-Level Control in Superconducting Quantum Processors

This folder contains the processed numerical data used to generate the figures in the manuscript
**Scalable Suppression of XY Crosstalk by Pulse-Level Control in Superconducting Quantum Processors**.

Publication information:
- Phys. Rev. Applied, accepted 23 July 2026
- DOI: https://doi.org/10.1103/v8p3-qh5k

## Contents
- one CSV file per figure panel. The panel is indicated by the filename prefix (e.g.,`fig4c_...`).

## CSV format
Each CSV file contains a single header row followed by numerical data.

- The first column is the x-axis variable:
  - `t` (time) in **[ns]**, or
  - `J` (coupling strength) in **[MHz]** for (J/2\pi), or
  - `gamma` (Z-modulation driving strength) in **[100MHz]** for (gamma/2\pi).
- Remaining columns are y-axis datasets:
  - `*_infid_*`: gate infidelity, defined as (1 - F), F is average gate fidelity.
  - `*_error_*`: error terms used in the manuscript.
  - `*_decoh_*`: decoherence-only case.
- Suffixes such as `CD`, `FM`, `DD` denote the control setting.
- `X1`, `X2`, `X1X2`, `idle` indicate the gate operation considered in the dataset:
  - `X1`: single-qubit X gate on qubit 1
  - `X2`: single-qubit X gate on qubit 2
  - `X1X2`: parallel operation applying X gates on both qubits
  - `idle`: idle evolution 
- `5q` indicates simulations performed in the 5-qubit setting. If `5q` is not present, the data correspond to the 2-qubit setting.
- Labels like `N_4`, `N_6`, `N_8` denote the numbers of modulation cycles (N) used in the FM, consistent with the manuscript.
- `_nonuni_` in the filename indicates datasets for detuning nonuniformity cases.

