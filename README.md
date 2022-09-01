# Neural_Network_Charity_Analysis

## Overview

A client who chooses charities to invest in, wanted us to use a dataset of charities and their successes to determine if we coulud predict/decide which charities are best to invest in.

## Reources
- pandas
- keras / tensorflow
- carity_data.csv


## Results

### Preprocessing
1. Identified our target: the application "IS_SUCCESSFUL" column
2. Identified the features that woulud mold our model: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, STATUS
3. Removed: "EIS", "NAME", and "ASK_AMT"
  - we removed ask amount, as we felt there was too much variance within the column. 
  
### Compiling, Training and Evaluation
1. Chose 3 layers, with 24/12/6 layers respectively.
2. Used 'relu' as the activation function for all layers
3. Used 'sigmoid' as the activation function for the output layer
4. The target accuracy was 75%, we reached 61%, so there may still be some optimization to be done. 
5. The original model started at 47% accuracy.

### Optimization
Seeing as how the original model started at 47% accuracy, and we wanted to reach 75%, we tried some optimization options.
1. Removed ask_amt 
2. Added an additional layer
3. Increased the nodes for each layer from 10/5 to 24/12/6


### Summary

The model that we chose did not reach the desired accuracy rating of 75%.  It is possible that this problem could be solved by a different model, it may be reccommended to use a random forest model, as it would be faster, more efficient and may yield better results.
