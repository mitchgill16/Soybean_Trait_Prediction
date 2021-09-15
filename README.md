Notebooks for Soybean Trait Prediction

These notebooks were used to predict soybean traits from genomic data however given data formatted in the same manner they could be used to predict other traits
from other crops. Data used for this project can be requested at mitchell.gill@research.uwa.edu.au

Required: Numpy, Pandas, tensorflow, python, jupyter

Open a jupyter notebook server either locally or connected to a gpu backend with singularity

Each Notebook contains cells to manipulate, train and evaluate an XGBoost model, RF model, CNN & DNN
Notebooks are not trait specific however they're data type specific. BC = Binary classification, MCC = multiple class clasffication, reg = regression
For example Flower Colour had 2 categorical traits to predict (notated as 0 or 1). The traits and input data typeswere kept in separate notebooks for easier result notation.
However if you have a trait you'd like to predict that requires binary classification you could use any notebook that ends in BC.



Your own data should be formatted as follows

Rows: Individual Line Samples

Columns: SNPs

Final Column: Recorded phenotype for given trait

A holdout set was used, where each of the columns were the same SNP inputs, however these were not seen by the model until after training.
EG. If the training data had column headers SNP_01 SNP_02 ..... SNP_99999 Value, the holdout data would have the same column headers but different rows

New Commit: Comments on some notebooks were updated and added to explain some of the inbetween helper functions eg. the massive load in function, one hot encode etc. Both flower colour notebooks in particular are the best notated and should explain what each cell and new function does.
