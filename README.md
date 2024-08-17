# DL-Project-Brain-MRI-Calssification
Implementation of a CNN classifier of brain MRI images to Alzheimer's severities and comparisom to transfer leaning (using multiple models)


  * [Background](#background)
  * [Prerequisites](#prerequisites)
  * [Files in the repository](#files-in-the-repository)
  * [Dataset](#dataset)
  * [AltzCNN - Our CNN Archtiecture](#altzCNN---our-cnn-archtiecture)

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
|`Trained_models`| This directory contains .pth files, one for each model. These are the saved states of the models trained in this project|

## Dataset
Contains 44,000 brain MRI images categorized into 4 distinct classes

The dataset is augmented

We divide the dataset to 
70% train
15% validation
15% test

////////////////////TODO add exapmles

## AltzCNN - Our CNN Archtiecture
![image](https://github.com/user-attachments/assets/854d7e83-5989-44ca-bf16-b6740dfd8cc0)

## Results

## References


