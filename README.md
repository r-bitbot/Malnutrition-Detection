# Predicting Malnutrition in Children Using CNN Architectures 
This project aims to apply deep learning and address the issue of malnutrition in such places where resources are limited. Convolutional neural networks (CNNs) and its following architectures—VGG16, VGG19, and ResNet18—were trained on a dataset of labelled images to classify images into ‘healthy’ and ‘malnourished’ and automates classification of malnourished and healthy individuals. 

## Objectives
1. To conduct a comprehensive review on background, obstacles, and necessities associated with detecting malnutrition in children through image analysis.
2. To preprocess the dataset of images and standardize them for easy submission.
3. To leverage use of various CNN architectures such as VGG16, VGG19, and ResNet-18 for deep learning based classification.
4. To train the architectures on labelled data and customise layers accordingly to experiment.
5. To conduct experimentation of above models and compare metrics such as performance, accuracy, detection rate, etc. of each individual model and determine which aligns best with the given dataset.

## Running the notebook locally
To run the notebook on your local machine and use the provided datasets, follow the steps below:

### 1. Download the datasets
Given are the [malnourished](https://drive.google.com/drive/folders/1W9cpubFkGT8nEG_CuiU_arMQVpQ3N5MJ?usp=drive_link) and [healthy](https://drive.google.com/drive/folders/1eQY6Z4PXlUT59Sf8Hq_nEW4hoT-7CChK?usp=drive_link) datasets, download both folders and save to a folder on your local machine.

### 2. Set up your local environment
Unless you are planning to run this on your google colab, ensure you have Python and the required dependencies installed (refer to the requirements section in this README). Open your preferred Python IDE or environment (VS Code, PyCharm, or terminal)

### 3. Specify the local directory path
For Google Colab, replace the code
' ' '
data_dir = '/content/drive/My Drive/'
' ' '
with
'''
data_dir = '/content/drive/location/'
'''
where location is the folder wherein the datasets have been saved. 

To run locally, replace the code
'''
data_dir = '/content/drive/My Drive/'
'''
with
'''
data_dir = 'your_location/'
'''
where your_location is the path on your computer where malnourished and healthy folders are stored. For example:
On Windows: data_dir = 'C:/Users/YourName/Documents/datasets/'
On macOS/Linux: data_dir = '/Users/YourName/datasets/'

### 4. Adjust the notebook 
Only do the following if running locally, otherwise leave as is.
Use the updated data_dir variable in your data loading and processing code and remove or comment out any code specific to Colab or Google Drive, such as:
'''
from google.colab import drive
drive.mount('/content/drive')
'''

### 5. Run the notebook as a Python script
You can now run the notebook’s code cells as Python scripts in your environment, ensuring that all file paths reference your local directory and not the Colab default.
