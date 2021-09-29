# Facial Expression Recognition with Convolutional Neural Network and Visualization with Grad-CAM and OpenCV

## Blog

[Medium Blog]()

## Introduction

We will build a Convolutional Neural Network to categorize the emotion shown in the facial expression in to one of seven categories: 0 = Angry, 1 = Disgust, 2 = Fear, 3 = Happy, 4 = Sad, 5 = Surprise, 6 = Neutral. 

Grad-CAM will be used to identify what the machine is seeing when making decision.

Once trained, the model will be deployed to a web interface using Flask to perform real-time facial expression recognition, using the Haar Cascade method from OpenCV, on video and image data.

## Data Source

Data comes from Kaggle competition: Facial Expression Recognition Challenge (FER-2013). The train set consists of 28,709 examples of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centered and occupies about the same amount of space in each image. 

* emotion column contains a numeric code ranging from 0-6.

* pixels  column contains a string surrounded in quotes for each image.

## Exploratory Data Analysis

<img src = '../main/Data/samples.png'>

## Modeling

### Model Architect

<img src = '../main/Data/model_summary.png'>

### Model Evaluation

**Accuracy & Loss Curves**

<img src = '../main/Data/acc_loss_curve.png'>

**Confusion Matrix**

<img src = '../main/Data/cm.png'>

**Classification Report**

<img src = '../main/Data/classification_report.png'>

## Grad-CAM

<img src = '../main/Data/gradcam1.png'>

<img src = '../main/Data/gradcam2.png'>

<img src = '../main/Data/gradcam3.png'>

<img src = '../main/Data/gradcam4.png'>

<img src = '../main/Data/gradcam5.png'>

<img src = '../main/Data/gradcam6.png'>

<img src = '../main/Data/gradcam7.png'>

## Reference

Edwards, V. (2014). The definitive guide to reading micro-expression (Facial expressions). Science of People. Retrieved September 27, 2021, from https://www.scienceofpeople.com/microexpressions/.

Emotion detection and recognition market. Market Research Firm. (n.d.). Retrieved September 27, 2021, from https://www.marketsandmarkets.com/Market-Reports/emotion-detection-recognition-market-23376176.html.

Goodfellow, I.J., et.al. (2013). Challenged in representation learning: A report of three machine learning contests. Neural Networks, 64, 59–63. doi:10.1016/j.neunet.2014.09.005.

Kekre, S. (n.d.). Facial expression recognition in Keras [MOOC]. Coursera. https://www.coursera.org/projects/facial-expression-recognition-keras.
Universal emotions. Paul Ekman Group. (2021). Retrieved September 27, 2021, from https://www.paulekman.com/universal-emotions/.
