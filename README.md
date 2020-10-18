# Face-Detection-in-CNN-HOG-SSD-SVM-
(CNN, HOG, SSD, SVM) Multiple Model Face Detection.

![image](https://user-images.githubusercontent.com/39921122/96381015-b811f400-11b1-11eb-8a91-babf0c773d61.png)



# (CNN) A Convolutional Neural Network Cascade for Face Detection.

Deep learning methods are powerful approaches but often require expensive computations and lead to models of high complexity which need to be trained with large amounts of data. In this paper, we consider the problem of face detection and we propose a light-weight deep convolutional neural network that achieves a state-of-the-art recall rate of 90 % at the challenging FDDB dataset. Our model is designed with a view to minimize both training and run time and outperforms the convolutional network used in for the same task. Our model consists of only 76.554 free parameters whereas the previously proposed CNN for face detection had 60 million parameters.

![image](https://user-images.githubusercontent.com/39921122/96376555-7e38f180-11a1-11eb-8ec9-03fdb4b5ac6f.png)

## The CNN trained for the task of full face detection. Bottom: The CNN trained for the task of facial parts detection. 

![image](https://user-images.githubusercontent.com/39921122/96376646-0a4b1900-11a2-11eb-8931-be7d4cbfa092.png)

The results of the proposed training methodology on the FDDB dataset for the face detection CNN. A similar approach was used for the part-based CNN and the combined CNN. 

![image](https://user-images.githubusercontent.com/39921122/96376689-467e7980-11a2-11eb-83c8-2a1e159203ea.png)

# HOG(Histogram of Oriented Gradients)

HOG is a feature descriptor used to extract the features pixel by pixel with the help of gradients. This is primarily used for face detection, recognition and object detection. HOG works on grey scale images. Every image has a particular gradient orientation which helps the HOG extract the unique features from an image.

![image](https://user-images.githubusercontent.com/39921122/96377615-92ccb800-11a8-11eb-8fed-9d9883b380a9.png)

![image](https://user-images.githubusercontent.com/39921122/96378624-243f2880-11af-11eb-9116-846900532624.png)

![image](https://user-images.githubusercontent.com/39921122/96378775-38cff080-11b0-11eb-9fa9-9e608ccce8d9.png)

# (SSD) Single Shot Detector

![image](https://user-images.githubusercontent.com/39921122/96378842-ad0a9400-11b0-11eb-8a6e-173230cabd3d.png)

![image](https://user-images.githubusercontent.com/39921122/96378858-c01d6400-11b0-11eb-81ad-48f9b9c439e0.png)

The SSD algorithm is called single shot because it predicts the bounding box and the class simultaneously as it processes the image in the same deep learning model. Basically, the architecture is summarized in the following steps:

1. A 300 x 300 image is input into the architecture.
2. The input image is passed through multiple convolutional layers, obtaining different features at different scales.
3. For each feature map obtained in 2, we use a 3 x 3 convolutional filter to evaluate small set of default bounding boxes.
4. For each default box evaluated, the bounding box offsets and class probabilities are predicted.

![image](https://user-images.githubusercontent.com/39921122/96382583-32db0f00-11b2-11eb-8f03-cb65d9ee2447.png)


# (SVM) Support Vector Machines 

Support vector machines (SVMs) are formulated to solve a classical two class pattern
recognition problem. We adapt SVM to face recognition by modifying the interpretation
of the output of a SVM classifier and devising a representation of facial images that is concordant with a two class problem. Traditional SVM returns a binary value, the class of
the object. To train our SVM algorithm, we formulate the problem in a difference space,
which explicitly captures the dissimilarities between two facial images. This is a departure
from traditionalface space or view-based approaches, which encodes each facial image as a separate view of a face.

![image](https://user-images.githubusercontent.com/39921122/96385022-f0fe9880-11b2-11eb-9dd2-64275563c928.png)

![image](https://user-images.githubusercontent.com/39921122/96385040-096eb300-11b3-11eb-854e-ff162717fd3b.png)

# Getting started

## How to run all of them ...

First you need to move in the this github file directory using **Anaconda Command Prompt**. Then install all prerequisites using this command.

**`pip install -r requirements.txt`**

## Then you can run all of the individual model using those command.

1) For Convolutional Neural Network (CNN)

**`python face_detection_cnn.py`**

2) For Histogram of oriented gradients (HOG) with support-vector machines (SVM)

**`python face_detection_hog_svn.py`**

3) For Single Shot Detection (SSD)

**`python face_detection_ssd.py`**

4) If you want to check the difference between CNN and HOG then run **all.py** file.

**`python all.py`**

# Thank You !
