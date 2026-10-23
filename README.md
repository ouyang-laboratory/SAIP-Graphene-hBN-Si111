# SAIP-Graphene-hBN-Si111

DFT reference data and SAIP parameter files for graphene/Si(111) and h-BN/Si(111) interfaces.

## DFT_data

The `Graphene_Si(111)/` and `h-BN_Si(111)/` directories contain the following data.

All energies are absolute total energies in eV. Distances and in-plane coordinates are in Å.

| File | Description |
| --- | --- |
| `Binding_energy.txt` | Columns: interlayer distance, interface total energy. |
| `Sliding_potential_energy_surface_of_low_strain_model.txt` | Low-strain sliding PES. Columns: x, y, interface total energy. |
| `Sliding_potential_energy_surface_of_high_strain_model.txt` | High-strain sliding PES. Columns: x, y, interface total energy. |
| `Isolated_graphene_*_strain.txt` / `Isolated_hBN_*_strain.txt` | Isolated graphene or h-BN layer total energy for each strain model. |
| `Isolated_Si_slab_*_strain.txt` | Complete isolated Si slab total energy for each strain model. |
| `geometry.in_low_strain` / `geometry.in_high_strain` | Low- and high-strain interface structures in FHI-aims format. |
| `control.in` | FHI-aims input settings and basis definitions, provided in the h-BN directory. |

## SAIP_code

| File | Description |
| --- | --- |
| `Si_C_gpumd.SAIP` | Graphene/Si parameters for GPUMD. |
| `Si_BN_gpumd.SAIP` | h-BN/Si parameters for GPUMD. |
| `Si_C_lammps.SAIP` | Graphene/Si parameters for LAMMPS. |
| `Si_BN_lammps.SAIP` | h-BN/Si parameters for LAMMPS. |

Compatible GPUMD or LAMMPS implementations are required.
