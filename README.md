# PRISMA
Perceptually Robust Iterative Similarity Momentum Attack

Abstract: The widespread sharing of facial images on social media platforms has enabled unauthorized facial recognition (FR) systems to systematically track and profile individuals without their consent. We introduce PRISMA (Perceptually Robust Iterative Similarity Momentum Attack), whose artificial intelligence contribution is a novel two-stage adversarial attack framework that combines momentum-based optimization with perceptual constraints. The first stage computes robust target features across multiple classes, while the second stage uses these features along with momentum-based optimization to generate visually imperceptible perturbations. The engineering application of PRISMA is privacy protection against unauthorized FR systems. Our empirical evaluation reveals a critical vulnerability in existing protection methods: they can be circumvented through reverse attacks that achieve recognition rates up to 74.64\%. In contrast, PRISMA significantly outperforms state-of-the-art methods by reducing FR accuracy to below 26.28\% while maintaining high perceptual quality (PSNR-HVS-M of 35.82 dB). Our method demonstrates strong transferability across different model architectures and commercial APIs, which makes it a practical solution for protecting users' privacy.

# The Dataset
We have used the MTF data set which contains 5246 images with a distinct distribution of celebrities' image faces that emerged across different labels.

Get the Dataset
The MTF data set can be accessed through the following link

https://sobigdata.d4science.org/catalogue-sobigdata?path=/dataset/multi-task_faces_mtf_dataset

# Minors Dataset
Along with that we have also compiled a dataset of under-age public figures to add more images to the MTF dataset.

Get the Dataset
The minors dataset can be accessed through the following link

https://drive.google.com/drive/folders/1FaUx_nDxKmz_baxsC5C7pTT8_w2sGNI0?usp=sharing

# To Execute the code please follow these steps

# 1. Install the Required packages and libraries
      Provided in the Requirements.txt file
# 2. Stage 1: Train a Face Reconition model and Compute Target Features (use FR_Train.ipynb & Compute_Targets.ipynb)
      After you have downloaded the datasets and the models, and have installed the required libraries & packages,
      2.1. Open the ipynb file named FR_Train.ipynb to train the initially required model
      2.1.1 Change the required paths
      2.1.2. Run the code
      2.2. Compute Target Features
      2.2.1. Change the paths
      2.2.2. Run the code
# 3. Stage 2: To protect the images (Use PRISMA.ipynb)
      After you have trained the model and computed the target features, we now protect the images
      1. Open the ipynb file named PRISMA.ipynb to protect the images
      2. Change the required paths
      3. Set the parameters, we have already included the recommended parameter values
      4. Run the code to generate and save protected images
