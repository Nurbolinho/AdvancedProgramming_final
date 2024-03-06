`                                                                   `**Report**

**IT-2203:**

**Nurbolat Kayrbolatov**

**Aidyn Marat**

**Introduction:**

**Problem:**

This model should determine which class the image belongs to. There should be 6 classes in total, according to the number of our fingers, given that the absence of raised fingers is also a class. It's pretty clear that this is the CNN(Convolutional Neural Network) model. It is quite simple, but at the same time effective.

**Literature review with links (another solutions):**

1\. How To Implement CNN Model To Count Fingers And Distinguish Between Left And Right Hand?

<https://analyticsindiamag.com/how-to-implement-cnn-model-to-count-fingers-anddistinguish-between-left-and-right-hand/>

2\. Object Counting with CNNs (Intro to Computer Vision Part 1)

<https://www.youtube.com/watch?v=VLJ6RNlvS3Y>

3\. Finger Counting using AI

<https://www.linkedin.com/pulse/finger-counting-using-ai-chandra-sharat/>

4\. Finger Representation and Finger-Based Strategies in the Acquisition of Number Meaning and Arithmetic

<https://www.researchgate.net/figure/Representation-of-five-different-finger-counting-systems-from-A-large-parts-of-Europe_fig1_283516176>

**Current work (description of the work):**

We have created a convolution model to determine the number of fingers on an image of a hand. We used the dataset from the site "https://zenodo.org/records/3901659 " (As far as we understand, zenodo datasets do not belong to Kaggle).

Our model is quite simple, but it copes with the most important thing that it copes with its task. In the end, we gave an example of how it copes with real examples, although before that it is desirable (but not necessary) to change the color palette to dark white, for more effective prediction of the model, since our model was trained on a specific dataset. She was trained on 1200 images, 200 for each class.

Below we have provided examples of data from this dataset. ->


**Data and Methods:**

**Information about the data (probably analysis of the data with some visualisations):**

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.001.png)

And we also added the total number of data images

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.002.png)

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.003.png)

**Description of the ML/DL models you used with some theory (it is a must):**

If you tell us more about the model:

Input layer: The input data is 128x128 images.

Next is the Convolution and MaxPooling layer: Convolution layer (Conv2D) with the ReLU activation function and with 32 filters. A MaxPooling layer to reduce the dimension with a size of 2x2. After that, there are two more blocks with Convolution layers already with 64 filters and also using subsampling.

Next comes Dense Layers with 512 neurons and a ReLU activation function. One of the most important is the Dropout layer with a coefficient of 0.3 for regularization, since it prevents overfitting of the model. 

At the end there is a Dense layer with 6 neurons, each for each class.

**Results:**

**Results with tables, pictures and interesting numbers:**

Accuracy and Loss graphs…

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.004.png)

One of the most interesting part for us here, that we show bad predictions with images, wrong predicted and actual (predicted) labels (classes).

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.005.png)










Some confusion matrix:

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.006.png)

And prediction on our actual images (our hands):

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.007.png)

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.008.png)

**Discussion:**

**Critical review of results:**

The results show that our model is sufficiently trained and capable to classify images. She showed a fairly high performance in the training sets. And out of 1,200 training images, only 48 were with wrong prediction.

![](Aspose.Words.5cfe5996-fa8d-4670-b538-32c1c3784f2e.009.png)

**Include links of all the materials you used at the end of the report (sources):**

1\. How To Implement CNN Model To Count Fingers And Distinguish Between Left And Right Hand?

<https://analyticsindiamag.com/how-to-implement-cnn-model-to-count-fingers-anddistinguish-between-left-and-right-hand/>

2\. Object Counting with CNNs (Intro to Computer Vision Part 1)

<https://www.youtube.com/watch?v=VLJ6RNlvS3Y>

3\. Finger Counting using AI

<https://www.linkedin.com/pulse/finger-counting-using-ai-chandra-sharat/>

4\. Finger Representation and Finger-Based Strategies in the Acquisition of Number Meaning and Arithmetic

<https://www.researchgate.net/figure/Representation-of-five-different-finger-counting-systems-from-A-large-parts-of-Europe_fig1_283516176>

5\. How Many Hidden Layers and Neurons does a Neural Network Need

<https://youtu.be/YhatZb5SzE0?si=sFrnlQVeXyzBhg-l>

6\. Introducing convolutional neural networks

<https://youtu.be/x_VrgWTKkiM?si=K-_I4OxE8AEpwPWC>

