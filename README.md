# **Chest-X-Ray-Classification-using-CNNs**

## 📑 Overview:

This project designs and evaluates two convolutional neural networks (CNNs) for the classification of chest X-ray images: normal and with pleural effusion.
This binary image classification problem was part of a Machine Learning module within a Bioinformatics and Biostatistics Master’s program. 

The dataset was based on a NIH ChestXray dataset available in Kaggle:
https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publiclyavailable-chest-x-ray-datasets-scientific-community.
https://www.kaggle.com/datasets/nih-chest-xrays/data

Model 1 outperformed Model 2 across multiple metrics, demonstrating a superior ability to discriminate between normal and pathological radiographs.

## 🔬 Methodology

1.	**Data import and exploration**
2.	**Image preprocessing**. All images were resized from 512x512x3 to 64x64x1, normalized and only one grayscale channel was kept.
3.	**Data splitting**. 600 training / 100 test images
4.	**Model development**. Two CNN models: ≤6 convolutional layers, pooling layers, 2 fully connected layers, >60K trainable parameters, sigmoid output.
5.	**Evaluation and comparison**: quality metrics and ROC curve analysis.

## 📚 Key results
- Due to the stocastic nature of CNN training and the usage of dropout, small variations were found in the ROC curves and confusion matrix results. 
- Model 1 achieved a higher AUC, with its ROC curve closer to the top left corner of the graph.
- Model 1 showed higher precision, atlhough Model 2 produced less false negatives.

