# DeepLearning


## 1. Sign Language Digits Dataset Description: 

- Sign languages (also known as signed languages) are languages that use the visual-manual modality to convey meaning
- This can include simultaneously employing hand gestures, movement, orientation of the fingers, arms or body, and facial expressions to convey a speaker's ideas. 
- The aim is to create a model that can predict Sign language digits (0 - 9) from the input images. 
- Deep Learning is founded on novel algorithms and architectures for artificial neural networks together with the recent availability of very fast computers and massive datasets enables multitasking thereby learning highly informative features.
- Since we were dealing with images, it seemed intuitive to use CNN as it greatly reduces the number of parameters of the model to learn.

## 2. Overview of Data: 

- Sign Language Digits Dataset dataset prepared by Turkey Ankara Ayrancı Anadolu High School students.
- Details of datasets:
    - Image size: 64x64
    - Color space: Grayscale
    - Number of classes: 10 (Digits: 0-9)
    - Number of participant students: 218
    - Number of samples per student: 10
- A Kaggle link to the dataset is given here https://www.kaggle.com/ardamavi/sign-language-digits-dataset

## 3. Deep Learning Model 

**(a). Data Exploration:** 

    - The dataset was presented as separate X and Y files
    - The shape of X data is (2062, 64, 64, 1)
    - The shape of Y data is (2062, 10)
    - The Y is already one – hot – encoded in the file and readily available for analysis
    - The data was split into test – train (20 : 80)

**(b). Model Pipeline:** 

    - A basic deep learning modeling pipeline was proposed

**(c). Visualization of model results:**

    - Model accuracies with various parameters were plotted

**(d). Comparison of results:**

    - Results obtained with various optimizers were compared

## 4. Conclusions:
 
- In this work we created a deep learning model pipeline to study the sign language dataset of digits
-  The model was tuned for various loss and activation functions for accuracy
- We chose two different optimizers Stochastic Descent and Adam optimizers and obtained results iteratively for 
statistical variability
- While Adam optimizer resulted in statistically rich results for accuracies in the iteration SGD optimizer resulted 
in a more uniform set of values
- Moreover, accuracies with SGD optimizer suffered as it got stuck in local minimums at the stage of minimizing 
the error with frequent updates and performed lower than other optimizers at equal epoch values.
- **Adam Optimizer** gave an **accuracy of about 45%** and it is better for the current dataset

## 5. Future Scope:

- A more sophisticated modeling pipeline with convolution, pooling, flatten will have better accuracy than the 
one currently proposed
- The novel developments in computer vision and other deep learning techniques make the development in image 
classification calls for interesting improvements in the model but it is beyond the scope of the current study as it 
is just an introductory level study in deep learning. 