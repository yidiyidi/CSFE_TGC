# CSFE_TGC
## Data Generation
The codes applied here is for the main experiment using RML dataset. The "1_Make_Data_signal.ipynb" file is intended to generate required features. Firstly, the labels of each class are randomly chosen to be wrong up to a pre-determined proportion, therfore forming a desired noisy dataset. Secondly, through the DNN, we can therefore extract features embedding from any iteration and any layer of the DNN.\\

## Main Ideas
The "2_CSFE_TGC train boundaries.ipynb" file consists of main ideas of our paper, which are Class Sensitivity Feature Extractor (CSFE) and T-type Generative Classifier (TGC). With the features from the DNN and their corresponding noisy labels taking the part of the input, we can form a rank of these features through CSFE and extract certain amount that we require, and then apply TGC on these extracted features to form a robust decision boundries. Things left to do is just a simple retraining.
