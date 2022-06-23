# Acetylacetone dataset

units: Angstrom, eV, eV / A

QM method: ORCA 5.0, UHF PBE + D3, def2-SVP basis set, VeryTight SCF convergence settings, and basin-hopping

`isolated_atoms.xyz` : Energies of the isolated atoms evalauted at the reference DFT settings

`train_300K.xyz` : 500 decorrelated geometries sampled from 300 K xTB MD run

`train_600K.xyz` : 500 decorrelated geometries sampled from 600 K xTB MD run

`test_MD_300K.xyz` : test set of decorrelated geometries sampled from 300 K xTB MD

`test_MD_600K.xyz` : test set of decorrelated geometries sampled from 600 K xTB MD

`test_H_transfer.xyz` : NEB path of proton transfer reaction between the two forms of the molecule

`test_dihedral.xyz` : Dihedral scan about one of the C-C bonds of the conjugated system 
