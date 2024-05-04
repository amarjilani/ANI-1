# From Structure to Energy: ML Approaches with ANI-1

Project Goal:
There are two main goals for this project.
1) Develop a deep neural network that can accurately predict the energy of a molecular
conformation, given information about the molecular structure (i.e. 3D coordinates and
molecular composition).
2) Develop a latent representation of the molecular structure using an Autoencoder network for
efficient data representation. This encoding would apply to a specific molecular conformation.
Train a second deep neural network that predicts energy based on the encoded representation.
The two models described above can then be compared in terms of accuracy and efficiency.

Dataset:
This project is utilizing the ANI-1 dataset. The ANI-1 dataset is large database consisting of over 20
million molecular conformations for over 57,000 unique organic molecules. For each molecule, there is
information of the coordinates of each atom for each conformation, the SMILES representation of the
molecule, and the energies of each unique conformation. There is a large variation in the number of
conformations per molecule, but most have several thousands of different conformations. The energies for
each conformation were calculated using DFT. Furthermore, the data will be converted to AEV
form, which will accounted for translational, rotational and permutational invariance. 

Results:
This project was able to accurately predict molecular energy from the 3D structure. Surprisingly, the encoded verison is able generalize better to larger molecules compared to the uncompressed version, demonstrating the usefulness of the autoencoder network.  
