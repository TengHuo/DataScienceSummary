# Image Processing

## Overview

### What is Computer Vision and Why is it Difficult?
Extracting descriptions of the world from pictures or sequences of pictures.

1. one image $\rightarrow$ many interpretations – problem is ill-posed
2. one object $\rightarrow$ many images – problem is exponentially large

### Applications of Computer Vision
- Autonomous vehicles
- Guiding tools for blind
- Object/Face recognition
- Content-based image retrieval
- Object tracking

### Image Formation

## Low-level Image Processing

### 1. Convolution



### 2. Masks

#### (a) Smoothing mask (mean filter, box mask)

#### (b) Gaussian mask

#### (c) Difference mask



### 2. Canny Edge detection
One of the most popular edge detectors is based on Gaussian derivative masks



### 3. Template matching
A mask can be viewed as a template for a particular image feature

## Mid-Level Image Processing

### 1. Feature space

**Grouping and Segmentation**: Group together those elements of an image that “belong together”, and segment these elements from all others.

### 2. Thresholding methods

Converting images from greyscale to black-and-white

### 3. Region-based methods

take into account the **location** of each pixel as well as its intensity, or colour, or texture (or other features or combination of features are being used to define similarity)


### 4. Clustering methods

A general class of methods for unsupervised classification of data (i.e. classes are not predefined). These methods can be used to group image elements based on similarity.

### 5. Fitting methods

A class of methods that try to use a mathematical model to represent a set of tokens. These methods are useful for identifying regular features in images, such as lines, circles, geometric shapes, etc.

e.g., Hough Transform



## High-Level Image Processing

1. Overview
2. Edge matching
3. Intensity histograms
4. Feature-based object recognition
5. Bag-of-words
6. Deep Learning Object Recognition















