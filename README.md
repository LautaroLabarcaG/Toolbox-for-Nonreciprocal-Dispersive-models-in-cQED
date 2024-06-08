# Toolbox-for-Nonreciprocal-Dispersive-models-in-cQED
Codes to reproduce main results of arxiv.2312.08354

## Example with Capacitive Filter

The responses were obtained with Mathematica file X. Then, the analytical expressions were typed onto Python functions, and used to get all relevant matrices developed in appendix C. We do not recommend to follow this apporach. Instead, we recommend to follow the approach in Example with resonator filter. 

## Example with resonator filter

The analytical form of the response was obtained with Mathematica in file X. Then, this was save as ,wbl file. Using this, the decompision Eq. A1 is Numerically obtained from Mathematica. Input the values in the python file, then run the mathematica, and finish running the python file. Finally, the quantum dynamics are obtained by truncating the Hilbert space to a maximum of 4 photons (5 to check convergence). 
