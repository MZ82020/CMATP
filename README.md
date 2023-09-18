# Cross-Modal Attention for Accurate Pedestrian Trajectory Prediction

# Overview
This repository contains the implementation of Cross-Modal Attention for Accurate Pedestrian Trajectory Prediction.

we propose a novel approach called Cross-Modal Attention Trajectory Prediction (CMATP) able to predict human paths based on observed trajectory and dynamic scene context. Our approach uses a bimodal transformer network to capture complex spatio-temporal interactions and incorporates both pedestrian trajectory data and contextual information.

Our approach includes a cross-attention module that integrates trajectory data with contextual information, allowing the network to capture the general temporal consistency of pedestrian movement. By using a convolutional model for feature extraction and a bimodal transformer, CMATP captures intricate spatio-temporal interactions, improving accuracy while maintaining the same computational complexity as using a single data type.

![Architecture_CMATP_Final_BMVC2023 drawio](https://github.com/MZ82020/CMATP/assets/94976539/00d6d619-6e66-4279-bfac-34afb999da80)

# Prerequisites

To install all the dependency packages, please run:

pip install -r requirements.txt

# Data Preparation

1- We use ETH and UCY datasets. Please download and extract information into the ./data_trajpred folder. Click on here to download data : https://drive.google.com/drive/folders/1REq_if6nqdjw_jYtuRVPJqmDNTcIxoJU?usp=drive_link
Then, update the data path (under DataBase Variables). The dataset used for training is set by default to eth, you can change that in the code into hotel, zara_01, zara_02, university (dataset_name variable).

The dataset should be in the /data folder and have the following structure:

    -data
        -data_trajpred
            -datasetname (eth, hotel, zara_01, zara_02, university)
                -visual_data
                -pos_data_train.db
                -pos_data_val.db
                -pos_data.db 

2- Set the path for saving your trained models in the code (save_path variable).
3- Run the following jupyter Pred_Traj_2EncDecTransf_CA_eth.ipynb to train and test the model

# Notes
The repository is still under construction. Please let me know if you encounter any issues.
Best, 
Mayssa ZAIER






