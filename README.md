# Cobrapy_vs_Wolfram_optimization
Discrepancies between the FBA solution obtained by cobra optimization and the FindMaximum module of Wolfram Mathematica
In this repository, we are comparing the FBA results using two optimizers. The first optimizer is the most used one implemented in Cobra. 
The results with other cobra optimizers are the same.  
The other optimizer for FBA is the one implemented in Wolfram-Mathematica version 12 (also version 13). 
There are two examples for comparing the results from Cobrapy and FindMaximum module of Wolfram Mathematica.
The first example corresponds to the textbook e-coli metabolic core, which is relatively short in terms of the number of compounds and reactions. 
For this model, the optimization performed in Wolfram Mathematica matches the one in Cobrapy. 
The other example corresponds to a bigger model, the one for Staphylococcus aureus (SA) metabolism.
This original model is available in JSON format (iYS854). 
The original file was cleaned (iYS854_version_4.json) by removing the following:
1) metabolites that do not participate in any reaction
2) metabolites that participate in only one reaction (which flux should be 0)
3) reactions containing metabolites that only participate in that reaction
The difference in the optimization between the two approaches is notable.
It also happens without cleaning the network
