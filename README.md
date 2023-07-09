# Candidate Elimination ALgorithm

For a given set of training data examples stored in a .CSV file, implement and demonstrate 
the Candidate-Elimination algorithm to output a description of the set of all hypotheses 
consistent with the training examples.

CANDIDATE-ELIMINATION Learning Algorithm
The CANDIDATE-ELIMINTION algorithm computes the version space containing all 
hypotheses from H that are consistent with an observed sequence of training examples.

Initialize G to the set of maximally general hypotheses in H
Initialize S to the set of maximally specific hypotheses in H
For each training example d, do
• If d is a positive example
• Remove from G any hypothesis inconsistent with d
• For each hypothesis s in S that is not consistent with d
• Remove s from S
• Add to S all minimal generalizations h of s such that
• h is consistent with d, and some member of G is more general than h
• Remove from S any hypothesis that is more general than another hypothesis in S
• If d is a negative example
• Remove from S any hypothesis inconsistent with d
• For each hypothesis g in G that is not consistent with d
• Remove g from G
• Add to G all minimal specializations h of g such that
• h is consistent with d, and some member of S is more specific than h
• Remove from G any hypothesis that is less general than another hypothesis in G

![image](https://github.com/ShreyaAR16/ML_OEE/assets/78254931/ab60b922-6ca2-4e52-bbff-a09f4227a134)

Dataset:

![image](https://github.com/ShreyaAR16/ML_OEE/assets/78254931/ebfc353d-97a4-45c1-9553-b950a870ec14)


