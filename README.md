# Compendium of available data sets and methods of hot spot prediction in literature

This compendium has been created to collect data sets and computational methods for protein-protein interaction hot spots that are available in literature.

## How to cite
#### If you use any of the lists collected in this repository, please cite the respective article.

### References for Data Sets

Thorn KS, Bogan AA: ASEdb: a database of alanine mutations and their effects on the free energy of binding in protein interactions. Bioinformatics 2001, 17:284-285.

Assi SA, Tanaka T, Rabbitts TH, Fernandez-Fuentes N: PCRPi: Presaging Critical Residues in Protein interfaces, a new computational tool to chart hot spots in protein interfaces. Nucleic Acids Res 2010, 38:e86.

Petukh M, Li M, Alexov E: Predicting Binding Free Energy Change Caused by Point Mutations with Knowledge-Modified MM/PBSA Method. PLoS Comput Biol 2015, 11:e1004276.

Peng Y, Sun L, Jia Z, Li L, Alexov E: Predicting protein-DNA binding free energy change upon missense mutations using modified MM/PBSA approach: SAMPDI webserver. Bioinformatics 2018, 34:779-786.

Jankauskaite J, Jimenez-Garcia B, Dapkunas J, Fernandez-Recio J, Moal IH: SKEMPI 2.0: an updated benchmark of changes in protein-protein binding energy, kinetics and thermodynamics upon mutation. Bioinformatics 2019, 35:462-469. SKEMPI 2.0 is the most recent and the largest database and hence, it is the most widely used database in computational hot spot prediction studies.

### References for Prediction Methods

Deng L, Sui Y, Zhang J: XGBPRH: Prediction of Binding Hot Spots at Protein(-)RNA Interfaces Utilizing Extreme Gradient Boosting. Genes (Basel) 2019, 10.

Preto AJ, Moreira IS: SPOTONE: Hot Spots on Protein Complexes with Extremely Randomized Trees via Sequence-Only Features. Int J Mol Sci 2020, 21. Using sequence-only features this work can accurately classify hot spot residues without a need for three-dimensional structure of the proteins. Additionally, this work is one of the very few methods which apply deep learning i.e., neural networks.

Tuncbag N, Keskin O, Gursoy A: HotPoint: hot spot prediction server for protein interfaces. Nucleic Acids Res 2010, 38:W402-406.

### Table 1. The list of experimental databases used for computational hot spot prediction. ΔΔG represents the change in binding free energy upon mutation.

| Database                   | Interactions                                                | Method  Used to  Obtain Data         | Number of proteins annotated | Number of Mutations annotated | ΔΔG | Year |
|----------------------------|-------------------------------------------------------------|--------------------------------------|-------------------------------|-------------------------------|-----|------|
| ASEdb                      | protein–protein protein–nucleic acid protein–small molecule | Experimentally                       | NA                            | 2919                          | +   | 2001 |
| Assi et al.‘s Ab+ data     | protein-protein                                             | Experimentally  validated            | 25                            | 636                           | -   | 2009 |
| Petukh et al.‘s Alexov sDB | protein-protein                                             | Experimentally                       | 81                            | 2041                          | +   | 2015 |
| SAMPDI                     | protein–nucleic acid (DNA)                                  | Experimentally                       | 13                            | 105                           | +   | 2018 |
| SKEMPI                     | protein-protein                                             | Experimentally and literature mining | 345 PDB entry                 | 7085                          | +   | 2019 |

### Table 2. Recent and/or highly cited computational hot spot prediction methods.

| Method                                               | Data                      | Features                                                                                                                             | Classifiers                                                   | Results#                                                               |
|------------------------------------------------------|---------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|------------------------------------------------------------------------|
| XGBPRH (Binding Hot Spots at Protein–RNA Interfaces) | 47 protein–RN A complexes | RDa (Cα atom depth), Closeness, Eccentricity, Relative total side ASA, Conservation, The number of Cβ atoms in the lower half sphere | XGBoost                                                       | AUC: 0.817 F1-score: 0.802                                             |
| SPOTONE                                              | ASEdb, BID, PINT, SKEMPI  | Secondary structure propensity, pKa associated values, Number of atoms of each type, Standard area, Mass associated values           | MLP, Random Forest, AdaBoost, SVM, Extremely Randomized Trees | Accuracy: 0.82 AUROC: 0.83 Precision: 0.91 Recall: 0.82 F1-Score: 0.85 |
| HotPoint                                             | ASEdb, BID                | Relative ASA, Knowledge-based pair potentials                                                                                        | An empirical formula                                          | Accuracy: 0.70 Precision: 0.73 Recall: 0.59 Specificity: 0.79          |

#As reported in their article.

