# Project Name : DeepFake Detection with ViT (Vision Transformer) pre-trained model

This Project utilizes a pre-trained model called ViT Transformer to detect a DeepFake Images. We did some tuning parameter since the limitations of available resources.

# Dataset use:

Source from Kaggle: https://www.kaggle.com/datasets/manjilkarki/deepfake-and-real-images

# Requirements
- Google Colab
- Kaggle API Key (For Downloading Dataset)

# Setup Instructions
We're running this in Google Colab thats why we need to apply this code on our .ipynb file

# 1. Upload your Kaggle.json file
	Firstly you need to upload the Kaggle API Key. You can get this file from the Kaggle's Account (Account > API > Create New API Tokens).
	This file will consist an information about your profile in Kaggle
	

Code Python:
from google.colab import files
files.upload()

# 2. Setup Kaggle API
	Once Uploaded, you can access the API on Kaggle and let Google Colab to download the dataset directly on the local environments in Colab, run this following command.

Code Python:
!mkdir -p ~/.kaggle
!mv kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

# 3. Download the Dataset.
	Once Setup is completed, you can run this code to download the dataset on the local environment on Google Colab

Code Python:
!kaggle datasets download manjilkarki/deepfake-and-real-images

# 4. Don't Forget to unzip the dataset

Code Python:
!unzip deepfake-and-real-images.zip

# NOTE: Run those code on your google colab!.
