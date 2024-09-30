# Computer Vision - Instance Detection and Classification

This repository contains the code developed for the practical part of the Image Processing and Computer Vision exam.

## Assignment 1: Instance Detection

The first assignment focuses on an instance detection task for products on shelves, using **classical computer vision methods** (no deep learning involved). The task was divided into two parts that were done using **OpenCV** library:

1. **Single Instances Identification using SIFT**  
   After denoising the noisy images, we utilized the **SIFT (Scale-Invariant Feature Transform)** algorithm to detect and identify products on shelves. SIFT allowed us to extract key points and descriptors from images, which were then used to match products in the scene.

2. **Generalized Hough Transform for Multiple Instances**  
   The second part posed a greater challenge due to:
   - The presence of really **noisy images**.
   - Multiple instances of the same product appearing within a single image.

   To tackle this, we implemented a variation of the **Generalized Hough Transform**. Instead of using the traditional R-Table, we constructed the object model by joining vectors from the SIFT-extracted features to their barycenter. At runtime, image features that matched the model cast votes for the position of the barycenter, scaling and rotating the vectors accordingly.

## Assignment 2: Product Classification

The second assignment was focused on the **classification** of supermarket products and was also divided into two parts. For this task, we used the **PyTorch** library to build and train deep learning models. Evaluation was done using **Weight and Biases** features.

1. **Vanilla CNN and Incremental Improvements**  
   We started with a basic **vanilla Convolutional Neural Network (CNN)**. By incrementally adding improvements—such as tweaking layers, activation functions, and regularization techniques—we enhanced the model's performance.

2. **Transfer Learning with ResNet-18**  
   In the second part, we implemented **transfer learning** and **fine-tuned** a pre-trained **ResNet-18** model, building upon the hyperparameters from the previous network. 

## Authors

• [Davide Crociati](https://github.com/davidecrociati)

• [Davide Sonno](https://github.com/davidesonno)

• [Lorenzo Pellegrino](https://github.com/lollopelle01)

---
