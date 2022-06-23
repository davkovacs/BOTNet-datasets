# Ethanol dataset

units: Å, eV, eV / Å

## QM method:
Orca 4.2, density functional theory, PBE exchange correlation functional, def2-SVP basis set, VeryTightSCF, Grid 7, NoFinalGrid

For the dissociation curve the DFT calculation uses open shell UHF-PBE and basin hopping to find the lowest energy dissociation curve. 

## Data description

In the training, MD test, and the H-removal test sets, the `OH_dist` field contains the distance between the O atom (index 2) and the neighboring H atom (index 8) in ethanol's hydroxyl group.
For the normal modes, the displacement field contains xyz along the normal mode for each frame.

`isolated_atoms.xyz` : energies of the isolated atoms evalauted at the reference DFT settings

`train.xyz` : 1000 ethanol configurations taken from the rMD17 dataset of Christensen et al. 

`test.xyz` : different 1000 ethanol configurations taken from the rMD17 dataset of Christensen et al. 

`train_eth_meth.xyz` : 300 methanol configurations added to the ethanol training set sample from 500 K Ab Initio MD simulations

`test_eth_meth.xyz` : 145 methanol configurations added to the ethanol test set sampled from 500 K Ab Initio MD simulation

`test_H_removal.xyz` : configuration path for removing the H atom from the ethanol's hydroxyl group starting from the equilibrium geometry while all other atoms are kept fixed

`test_norm_mode_874.xyz` : configurations along a vibrational mode with a wavenumber of 874 cm^-1

`test_norm_mode_3005.xyz` :  configurations along a vibrational mode with a wavenumber of 3005 cm^-1

`test_dimers.xyz` :  dissociation curves for the dimers HH, HC, HO, CC, CO, and OO; the interatomic distance is stored in the separation field. 

## References

Christensen, A. S.; Lilienfeld, O. A. von. On the Role of Gradients for Machine Learning of Molecular Energies and Forces. Mach. Learn.: Sci. Technol. *2020*, 1 (4), 045018. https://doi.org/10.1088/2632-2153/abba6f.

