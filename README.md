# Cobrapy_vs_Wolfram_optimization
Discrepancies between the FBA solution obtained by cobra optimization and the FindMaximum module of Wolfram Mathematica
In this repository, we are comparing the FBA results using two optimizers. The first optimizer is the most used one implemented in Cobra. 
The results with other cobra optimizers are the same.  
The other optimizer for FBA is the one implemented in Wolfram-Mathematica version 12 (also version 13). 
The file iYS854_version_4.json contains the metabolic network of SA in the iYS854.json model after a cleaning process where the following elements were removed:
1) metabolites that do not participate in any reaction
2) metabolites that participate in only one reaction (which flux should be 0)
3) reactions containing metabolites that only participate on that reaction
