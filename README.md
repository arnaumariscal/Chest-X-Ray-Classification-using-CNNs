# **Chest-X-Ray-Classification-using-CNNs**

## Project Statement:

As part of a Machine Learning module within a Bioinformatics and Biostatistics Master’s program, this project consisted of a binary image classification problem: distinguishing between normal chest X-rays and those showing signs of pleural effusion. The dataset was based on a subset of 700 labelled radiographs (350 normal and 350 with pleural effusion), extracted from the publicly available NIH ChestXray14 dataset:

https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publiclyavailable-chest-x-ray-datasets-scientific-community.

The objective was to design, implement, and evaluate two convolutional neural networks (CNNs) for the classification of chest X-ray images. The final step was to select the best-performing architecture based on classification metrics and ROC curve analysis.

The key responsibilities and steps involved in the project were:
1.	Data import and exploration
- The radiographs were provided in two compressed folders: one for normal cases and one for pleural effusion. Sample images from both folders were presented.
2.	Image preprocessing
-	All images were resized from 512x512x3 to64x64x1, keeping only one grayscale channel, since all three RGB channels contained the same information. 
-	Normalization was performed, using min-max scaling.
3.	Data splitting
-	The dataset was divided into training and testing subsets, maintaining class balance, with 600 images for training and 100 for testing. 
4.	Model development. Two different CNN models were built using Python with the following instructions:
-	Both models included no more than 6 convolutional layers
-	Pooling layers to reduce computational complexity
-	Two fully connected layers with 128 and 32 neurons
- The output layer used a sigmoid activation function to predict the binary outcome (normal vs. effusion)
-	Each model was designed with at least 60.000 trainable parameters to meet minimum complexity requirements
5.	Evaluation and comparison
-	Both models were tested using ROC curves and classification metrics to compare performance. 
6.	Conclusion

