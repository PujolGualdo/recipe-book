# Plasma proteomics (training and testing split options)

## LASSO

- splitting sample between 50-50 for training and testing
- taking the full set for associations with disease


## LightGBM

- 70-30 (testing diff models)
- then 5fold crossvalidation in all sample to retain full sample (data leakage)

## Tecla's approach
- nested CV, so we retain full sample for the selection of model, parameters and also the downstream associations (seems the most fair because of treating steps equally with same rationale about how predictions were built)
