# SAIP-Graphene-hBN-Si111

SAIP source code, potential parameters, and DFT reference data for graphene/Si(111) and h-BN/Si(111) interfaces.

## SAIP_code

| File | Description |
| --- | --- |
| `ilp_nep.cu` | GPUMD CUDA implementation combining ILP and NEP. |
| `pair_ilp_tmd.cpp` | LAMMPS implementation of the customized `ilp/tmd` pair style. |
| `pair_ilp_tmd.h` | Corresponding LAMMPS header. |
| `Si_C_gpumd.SAIP` | Graphene/Si parameters for GPUMD. |
| `Si_BN_gpumd.SAIP` | h-BN/Si parameters for GPUMD. |
| `Si_C_lammps.SAIP` | Graphene/Si parameters for LAMMPS. |
| `Si_BN_lammps.SAIP` | h-BN/Si parameters for LAMMPS. |

The source files require compatible GPUMD or LAMMPS installations. The LAMMPS parameter files retain the legacy label `Cd_1`; use the matching atom-type mapping.

## DFT_data

`Graphene_Si(111)/` and `h-BN_Si(111)/` contain the following files:

| File | Description |
| --- | --- |
| `Binding_energy` | Energy versus interlayer separation. Columns: distance (Å), energy (meV/atom). |
| `Sliding_potential_energy_surface_of_low_strain_model` | Low-strain sliding PES. Columns: x (Å), y (Å), energy (meV/atom). |
| `Sliding_potential_energy_surface_of_high_strain_model` | High-strain sliding PES, with the same column units. |
| `control.in` | FHI-aims calculation settings and basis definitions. |
| `geometry.in_low_strain` | Low-strain atomic structure in FHI-aims format; coordinates in Å. |
| `geometry.in_high_strain` | High-strain atomic structure in FHI-aims format; coordinates in Å. |
