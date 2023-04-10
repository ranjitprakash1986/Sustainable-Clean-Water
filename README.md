# Sustainable-Clean-Water

- author: Ranjitprakash Sundaramurthi
- contributors: Caesar Wong

## Introduction

This project was performed as part of the Biznovate 2023 Datathon conducted by the Pacific Conference on Artificial Intelligence 2023. The goal of this Datathon was to gain insight toward the Sustainable Develoment Goals of clean water.

> The model from this project ranked 9th at the competition closure on March 30, 2023. However, the quest to further improve my model continues beyond the termination of the competition.

### Objective

>**The challenge is to estimate the water quality index of a given region using satellite images. Data is provided with the water quality index of households, on a ranking scale of 1-5, five being the highest and one being the lowest.**

## Dataset

The dataset used in the project comes divided into train and test batches. Furthermore images for each of the train and test examples are provided. The images are stored in the *.npz file format. These satellite images are comprised of 8 bands.

The columns of train and test csv files correspond to the following:

- path: relative to the referenced image in dhs_train.
- water_index:  The target your model will be estimating.
- asset_index: Asset wealth index of the cluster.
- cluster_id: Identifier for the cluster of homes used for this datapoint.
- adm1dhs and adm1fips: More general identifiers for clusters referring to regions.
- cname: Country code.
- DHSID_EA: Survey ID of this datapoint, aligns with the associated image in the dataset.
- n_asset, n_water: Refers to number of homes within this cluster.
- urban: Binary identifier, where R = rural and U = Urban

The geocoordinates have been jittered randomly for privacy protection with a randomization of 2-10 Km.

The complete dataset can be downloaded [here](https://www.kaggle.com/competitions/bizinnovate-2023/data). This project is developed from SustainBench. The details of related domains of research under SustainBench can be read [here](https://openreview.net/pdf?id=5HR3vCylqD). The satellite images were source from [here](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9441016)

## Analysis Roadmap

## Results and Conclusions Roadmap

# License

The Student Dropout Predictor materials here are licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. This allows for the sharing and adaptation of the datasets for our purpose of academic study and understanding, with the appropriate credit given.

# References

Image processing techniques using Sobel Filters were referenced from:

- <https://www.youtube.com/watch?v=Ijc-9L2iXEc&list=PLZsOBAyNTZwYx-7GylDo3LSYpSompzsqW>
- <http://www.adeveloperdiary.com/data-science/computer-vision/how-to-implement-sobel-edge-detection-using-python-from-scratch/>
