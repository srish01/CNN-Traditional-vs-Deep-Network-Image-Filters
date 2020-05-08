# DIP(533)_project_spring2020
## Author- Srishti Gupta

This repository contains data, code and results for the Digital Image Processing (ECE-533) class project. The distribution of different contents in this repository is as follows:

## 1. Images/standard_test_images:
This folder contains standard images popularly used for image processing research works. The images were downloaded from "http://www.imageprocessingplace.com/root_files_V3/image_databases.htm".

## 2. Filtering_traditional_filters.ipyn:
This jupyter notebook file contains python code that does the following:

  a. Load the standard images 
  
  b. Apply 3 types of noises on them- Gaussian noise (with different variances), Poisson Noise, Salt and Pepper (SnP) Noise.
 
  c. Implements 4 types of traditional filters in python- Weiner, Median, Bilateral, Non-Local Means(NLM) filters.
  
  d. Filters different 3 types of noises using each of the above mentioned filtres.
  
  e. Calculates filter performance using the SSIM and PSNR metrics.
  
  f. Plots SSIM and PSNR of different filters into a bar plot for comaprative analysis.
 
## 3. Denoising_Autoencoder.ipynb: 
This jupyter notebook implements a Deep Neural Network (DNN) based denoising autoencoder. The flow of this code is as follows:
  
  a. Loads MNIST data
  
  b. Adds Gaussian, Poisson and SnP noises in MNIST data, to create noisy training and testing images.
  
  c. Creates a DNN autoencoder.
  
  d. Trains the autoencoder on training images.
  
  e. Evaluates the autoencoder on testing images.
  
  f. Measures performance of autoencoder in terms of SSIM and PSNR.
  
## 4. Filtering_mnist_traditional-vs-autoencoder.ipynb:
This jupyter notebook implements traditional filters (Weiner, Median, Bilateral and NLM) on MNIST as well as Natural image data. Performance of MNIST on traditional filters is compared with DNN autoencoder. SSIM and PSNR values are used directly from Denoising_Autoencoder.ipynb file. The flow of this code is as follows:
  
  a. Loads both standard images and MNIST images
  
  b. Applies traditional filters on both standard and MNIST images with 3 types of noises.
  
  c. Measures performance of traditional filters on standard and MNIST images in terms of SSIM and PSNR.
  
  d. Plots SSIM and PSNR performance of traditional filters with the DNN autoencoder results obtained from 'Denoising_Autoencoder.ipynb' for MNIST data.

## 5. 'results':
The results folder contains the different inputs and output images of filters, along with the bar plot results.
