# Compendium of available data sets and tools of hot spot prediction in literature

This compendium has been created to collect data sets and computational tools for protein-protein interaction hot spots that are available in literature.

## How to cite
#### If you use any of the lists collected in this repository, please cite the respective article.

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
