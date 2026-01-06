# HHCBR: A Hypergraph-Enhanced Framework for Balancing Healthiness and Preference in Meal Recommendation
This is our Pytorch implementation for the paper:

>Jialiang Shi, Takahiro Komamizu, and Ichiro IDE. HHCBR: A Hypergraph-Enhanced Framework for Balancing Healthiness and Preference in Meal Recommendation. 

Author: Jialiang Shi (shij@cs.is.i.nagoya-u.ac.jp)

## Introduction
HHCBR is a meal recommendation model based on graph neural network and contrastive learning for bundle recommendation, highlighting both the strength of hypergraph-based learning and the effectiveness of the FSA-driven healthiness partial ranking, while maintaining competitive performance in preference prediction compared with the state-of-the-art methods.

## Requirements
* OS: Ubuntu 18.04 or higher version
* python == 3.7.3 or above
* supported(tested) CUDA versions: 10.2
* Pytorch == 1.9.0 or above


## Code Structure
1. The entry script for training and evaluation is: [train.py](https://github.com/Shi-Jialiang/HHCBR/blob/d5a46e95e90e84193bc3ce2ed9d667b3f0538cc5/train.py).
2. The config file is: [config.yaml](https://github.com/Shi-Jialiang/HHCBR/blob/d5a46e95e90e84193bc3ce2ed9d667b3f0538cc5/config.yaml).
3. The script for data preprocess and dataloader: [utility.py](https://github.com/Shi-Jialiang/HHCBR/blob/d5a46e95e90e84193bc3ce2ed9d667b3f0538cc5/utility.py).
4. The model folder: [./models](https://github.com/Shi-Jialiang/HHCBR/tree/main/models).

## How to run the code
1. Train HHCBR on the dataset MealRec+L with GPU 0: 

   > python train.py -g 0 -m HHCBR -d MealRec+L

## Acknowledgement
This code is implemented based on the open source code from the paper **CrossCBR : Cross-view Contrastive Learning for Bundle Recommendation** (KDD '22).
