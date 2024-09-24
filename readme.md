"This repository is directly related to the AlignVSR paper. We will continue to maintain and improve the code in the future."

# Preprocess
We have adopted a consistent approach with the [AUTO-AVSR repository](https://github.com/mpc001/auto_avsr) for preprocessing the LRS2 and Single datasets.

Then, following the steps from [AUTO-AVSR (preparation)](https://github.com/mpc001/auto_avsr/tree/main/preparation), we process the LRS2 and CNVSRC.Single datasets to generate the corresponding `train.csv` and `test.csv`.

# Phase1-k-means
For the LRS2 and CNVSRC.Single datasets, we randomly sample a portion of the audio data from the training set to train a k-means model with a total of 200 clusters. For specific steps, please refer to [this link](https://github.com/liu12366262626/AlignVSR/tree/master/align_vsr/Phase1_k-means_cluster). After completing this step, we will obtain the k-means model for the next phase of training.
