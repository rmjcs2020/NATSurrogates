# NAT_Surrogates
Supporting code for ICML 2020 submission: Non-autoregressive time-series methods for stable parametric surrogate models

# Data for assessments
Please download data from [here](https://drive.google.com/drive/folders/133_6rn25pb_8xmvR2OB6_YNcSgymQFss?usp=sharing) and save the downloaded data to a folder `SWE_Data` alongside the `Results` and `Dropout_Results` folders.

The correct file structure for running the notebooks is:
1. `Results/`
2. `Dropout_Results/`
3. `SWE_Data/`
    1. `Data/`
    2. `PCA_Coefficients_q1.npy`
    3. `PCA_Vectors_q1.npy`


# Running the code
Each experiment from Section 4 of the paper is in its separate folder:
1. Section 4.3 results are in the folder marked `Standard/` and are named according to the nomenclature in the paper (see Table 1).
2. Section 4.4 results are in the folder marked `Dropout/` and are also named according to the same nomenclature.
3. Ablation results from Figure 4 in the paper can be found in `Ablation/`.

Within each experimental folder of `Standard` and `Dropout`, a jupyter-notebook can be run that loads the trained model and make predictions on the test data. A separate folder called `Figures` has a jupyter-notebook that loads the predictions for the purpose of comparitive visualization.