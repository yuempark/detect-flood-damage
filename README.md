# Satellite Images of Hurricane Damage

## Overview

The data used in this notebook are satellite images from the Greater Houston area after Hurricane Harvey in 2017. Each image has been labelled as either "Flooded/Damaged" or "Undamaged".

The data is available for download [here](https://www.kaggle.com/kmader/satellite-images-of-hurricane-damage), and the study associated with the dataset is available [here](https://arxiv.org/abs/1807.01688).

## Motivation

As stated in the abstract of the associated study:

> After a hurricane, damage assessment is critical to emergency managers for efficient response and resource allocation. One way to gauge the damage extent is to quantify the number of flooded/damaged buildings, which is traditionally done by ground survey. This process can be labor-intensive and time-consuming.

One way to improve the efficiency of building damage assessment is to identify flooded/damaged buildings from satellite remote sensing data alone.

## Method

In this notebook, I train a convolutional neural network to identify flooded/damaged buildings.

In particular, I use transfer learning with fine-tuning to achieve high accuracy while minimizing the amount of compute required to train the classifier.

Note that the notebook was executed using a Kaggle GPU kernel, so if you are viewing this notebook on GitHub, the images themselves have not been downloaded into the GitHub repository. However, you can still execute this notebook by either downloading the data using the links above, or forking this notebook on Kaggle [here](https://www.kaggle.com/yuempark/satellite-images-of-hurricane-damage).
