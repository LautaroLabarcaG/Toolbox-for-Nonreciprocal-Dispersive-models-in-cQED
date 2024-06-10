# Toolbox-for-Nonreciprocal-Dispersive-models-in-cQED
Codes to reproduce main results of arxiv.2312.08354

## Example with Capacitive Filter

The responses were obtained with the Mathematica Notebook "Example-with-capacitor-filter-response-chirality-condition.nb". Also, the chirality condition given by Eq. (9) was obtained leading to Eqs (22,23). Then, the analytical expressions were typed onto Python functions, and used to get all relevant matrices developed in appendix C. In this case we found more convenient to use the admittance response, but any of the two is equally valid in the dispersive regime.

## Example with resonator filter

The analytical form of the response was obtained with the Mathematica Notebook "Example-resonator-filter-analytical-response", saved as a .wbl file. Using this, the series decomposition Eq. (A1) is numerically obtained from Mathematica. We found the TransferFunction class of Mathematica more accurate than Sympy's equivalent. Then, the values are read and the quantum dynamics are obtained by truncating the Hilbert space to a maximum of 4 photons (5 to check convergence). The Impedance response was used, as it was found to be a convenient choice (due to the simplified resulting exact Hamiltonian due to the lack of poles at infinity), but once again, both approaches are valid in the dispersive regime.

The workflow then of this file is: Input values in "Example-with-resonator-filter" and save them as a values file. Then, run "Example-resonator-filter-get-poles-As-Bs-wjchiral", which will also give you the frequency of the qubits to get the desired hopping dynamics. Finally, run the whole of "Example-with-resonator-filter" and you will get the plots of the resulting dynamics. 
