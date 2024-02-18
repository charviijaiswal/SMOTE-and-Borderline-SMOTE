# SMOTE-and-Borderline-SMOTE

This is a simple project that performs a comparison of SMOTE and Borderline-SMOTE.

Synthetic Minority Over-sampling Technique
The main idea behind SMOTE is that generated instances should be constructed from available observations, but should not be identical.

1. Take difference between a sample and its nearest neighbour (from minority class)

2.Multiply the difference by a random number between 0 and 1. This gives us a synthetic example along the line between the two points.

3.Add this difference to the sample to generate a new synthetic example in feature space.

4.Repeat until number of samples is enough according to the oversampling ratio threshold (hyper-parameter).

Disadvantage of SMOTE: . Overfitting and poor generalization performance due to synthetic samples generated in dense clusters that may be near replicas of the seed sample.

BorderlineSMOTE is a variant of the SMOTE algorithm which makes the following assumption:
“Instances closest to a decision boundary are more relevant."
