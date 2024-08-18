# DL-Project-Brain-MRI-Calssification
Implementation of a CNN classifier of brain MRI images to Alzheimer's severities and comparisom to transfer leaning (using multiple models)


  * [Background](#background)
  * [Prerequisites](#prerequisites)
  * [Files in the repository](#files-in-the-repository)
  * [Dataset](#dataset)
  * [AltzCNN - Our CNN Archtiecture](#altzCNN---our-cnn-archtiecture)
  * [Results](#results)
  * [References](#references)

## Background
Alzheimer's disease is a brain disorder that slowly destroys memory and thinking skills, and eventually, the ability to carry out the simplest tasks. 
This project’s goal was to train a DL model that classifies brain MRI images to 4 Alzheimer’s severities: 
Non-Demented, Verry Mild-Demented, Mild-Demented and Moderate demented. 
Below you can see examples of MRI images from each class.
The motivation to use DL for Alzheimer’s classification comes from the tedious process patients need to go through to be diagnosed – multiple visits to doctors, 
mental status tests, physical and neurological exams and brain imaging. 
If a DL learning model can be trained to high classification accuracy, a brain MRI is the only step that will be needed.
In addition to designing a CNN classifier we also used transfer learning on other models and analysed their performance on the data. 
This gives a perspective of which models perform better on this task with respect to training times, accuracy and memory. 

![image](https://github.com/user-attachments/assets/bb13e16b-1c78-463d-af7d-b56005378244)


## Prerequisites
/////////////////////////////TODO update versions
|Library         | Version |
|----------------------|----|
|`Python`|  `3.5.5`|
|`torch`|  `0.4.1`|
|`torchvision`|  `0.4.1`|
|`kronia`|  `0.4.1`|
|`numpy`|  `0.4.1`|
|`matplotlib`|  `0.4.1`|
|`tqdm`|  `0.4.1`|
|`random`|  `0.4.1`|
|`sklearn`|  `0.4.1`|
|`seaborn`|  `0.4.1`|
|`PIL`|  `0.4.1`|
|`time`|  `0.4.1`|
|`os`|  `0.4.1`|




## Files in the repository

|File name         | Purpsoe |
|----------------------|------|
|`Brain_MRI_Altz_classification.ipynb`| The project's notebook, contains all models, training, graphs|
|`Results`| This directory contains multiple directories, one for each model. Each model directory contains images of training graphs and confusion matrix|

///////////////////////TODO upload models weights
## Dataset
[dataset](https://www.kaggle.com/datasets/aryansinghal10/alzheimers-multiclass-dataset-equal-and-augmented)
Contains 44,000 brain MRI images categorized into 4 distinct classes

The dataset is augmented

We divide the dataset to 
70% train
15% validation
15% test


## AltzCNN - Our CNN Archtiecture
![image](https://github.com/user-attachments/assets/854d7e83-5989-44ca-bf16-b6740dfd8cc0)

## Saved Models
Saved trained models can be found [here](https://drive.google.com/drive/folders/1Zx3zuQ56vP9jFeDkFAoaK-iTWzo-otPx?usp=sharing)

## Results
|model                   | size [MB] | Train Time [s] | Accuracy [%] |
|------------------------|-----------|----------------|--------------|
|`AltzCNN (Ours)`        |`22.93`    |`6553`          |`95.86`       |
|`ResNet-50`             |`89.91`    |`1136`          |`99.03`       |
|`ResNet-50 with DoRA`   |`89.95`    |`1117`          |`99.13`       |
|`EfficientNet`          |`15.47`    |`1578`          |`99.04`       |
|`EfficientNet woth DoRA`|`15.49`    |`1132`          |`98.92`       |
|`Vision Transformer`    |`327.31`   |`10136`         |`98.91`       |


![image](https://github.com/user-attachments/assets/9ec80d86-f7f0-4c4c-a02a-fc78b8171fe6)


## References
* [Vision Transformers](https://arxiv.org/abs/2010.11929v2)
* [CNN for image classification](https://ieeexplore.ieee.org/document/8379889)
* [ResNet](https://arxiv.org/abs/1512.03385)
* [EfficientNet](https://arxiv.org/abs/1905.11946)
* [DoRA](https://arxiv.org/abs/2402.09353)
* [Dataset](https://www.kaggle.com/datasets/aryansinghal10/alzheimers-multiclass-dataset-equal-and-augmented)
* [Previous work](https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset-v2/code)
