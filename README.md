# cg_param_m3

Please note, future development of this code will be at: https://github.com/cgkmw-durham/cg_param_m3

Coarse-grained mapping and parametrisation for organic molecules and surfactants, for the Martini 3 forcefield. The script takes a SMILES code as input, and outputs files for the Gromacs simulation code (.gro and .itp). The script can be run from the Linux command-line using: 

~~~~
./cg_param_m3 "[SMILES]" [name].gro [name].itp [dimer tuning (0/1)]
~~~~

Outputs .gro and .itp files compatible with Gromacs

The original version of this script for the Martini 2 forcefield, and a full description of the mapping and parametrisation procedures, can be found in the following paper:

T.D. Potter, E.L. Barrett and M.A. Miller, Automated Coarse-Grained Mapping Algorithm for the Martini Force Field and Benchmarks for Membrane–Water Partitioning, *J. Chem. Theory Comput.*, 2021, [https://doi.org/10.1021/acs.jctc.1c00322](https://doi.org/10.1021/acs.jctc.1c00322).

Additional methodology for the Martini 3 forcefield and tuning of models is introduced in:

T.D. Potter, E.L. Barrett and M.A. Miller, Mapping and parametrisation of esters and diesters in the Martini 3 force field: optimisation and automation, (in preparation).

Dependencies:

*numpy/scipy
*RDKit
*requests

The easiest way to install these dependencies is with conda

~~~~
$ conda create -c rdkit -n cg_param rdkit numpy scipy requests
$ conda activate cg_param
~~~~
