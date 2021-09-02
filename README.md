Notebooks for Soybean Trait Prediction

These notebooks were used to predict soybean traits from genomic data however given data formatted in the same manner they could be used to predict other traits
from other crops. Data used for this project can be requested at mitchell.gill@research.uwa.edu.au

Required: Numpy, Pandas, tensorflow, python, jupyter

Open a jupyter notebook server either locally or connected to a gpu backend with singularity

Each Notebook contains cells to manipulate, train and evaluate an XGBoost model, RF model, CNN & DNN

Otherwise data should be formatted as follows

Rows: Individual Line Samples

Columns: SNPs

Final Column: Recorded phenotype for given trait

A holdout set was used, where each of the columns were the same SNP inputs, however these were not seen by the model until after training.
EG. If the training data had column headers SNP_01 SNP_02 ..... SNP_99999 Value, the holdout data would have the same column headers but different rows
