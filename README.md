# Predicting Malnutrition in Children Using CNN Architectures 
This project aims to apply deep learning and address the issue of malnutrition in such places where resources are limited. Convolutional neural networks (CNNs) and its following architectures—VGG16, VGG19, and ResNet18—were trained on a dataset of labelled images to classify images into ‘healthy’ and ‘malnourished’ and automates classification of malnourished and healthy individuals. 

## Objectives
1. To conduct a comprehensive review on background, obstacles, and necessities associated with detecting malnutrition in children through image analysis.
2. To preprocess the dataset of images and standardize them for easy submission.
3. To leverage use of various CNN architectures such as VGG16, VGG19, and ResNet-18 for deep learning based classification.
4. To train the architectures on labelled data and customise layers accordingly to experiment.
5. To conduct experimentation of above models and compare metrics such as performance, accuracy, detection rate, etc. of each individual model and determine which aligns best with the given dataset.

## Running the notebook
To run the notebook on your local machine or in Google Colab and use the provided datasets, follow the steps below:

### 1. Download the datasets
Given are the [malnourished](https://drive.google.com/drive/folders/1W9cpubFkGT8nEG_CuiU_arMQVpQ3N5MJ?usp=drive_link) and [healthy](https://drive.google.com/drive/folders/1eQY6Z4PXlUT59Sf8Hq_nEW4hoT-7CChK?usp=drive_link) datasets, download both folders and save to a folder to your drive or local machine.

### 2. Set up your local environment
Unless you are planning to run this on your google colab, ensure you have Python and the required dependencies installed (refer to the requirements section in this README). Open your preferred Python IDE or environment (VS Code, PyCharm, or terminal)

### 3. Specify the local directory path
For Google Colab, replace the code
```
data_dir = '/content/drive/My Drive/'
```
with
```
data_dir = '/content/drive/location/'
```
where location is the folder wherein the datasets have been saved. 

To run locally, replace the code
```
data_dir = '/content/drive/My Drive/'
```
with
```
data_dir = 'your_location/'
```
where your_location is the path on your computer where malnourished and healthy folders are stored. For example:
On Windows: data_dir = 'C:/Users/YourName/Documents/datasets/'
On macOS/Linux: data_dir = '/Users/YourName/datasets/'

### 4. Adjust the notebook 
Only do the following if running locally, otherwise leave as is.
Use the updated data_dir variable in your data loading and processing code and remove or comment out any code specific to Colab or Google Drive, such as:
```
from google.colab import drive
drive.mount('/content/drive')
```

### 5. Run the notebook as a Python script
You can now run the notebook’s code cells as Python scripts in your environment, ensuring that all file paths reference your local directory and not the Colab default.

## Requirements 
This is not required for those that want to run this on colab, as all packages are already readily available.
To run the code and reproduce the workflow described above, please ensure you have the following dependencies installed in your local Python environment:

Python
Python 3.7 or above is recommended. Note that Python 3.13 does not support Tensorflow.

Python Packages
Install these packages via pip. Below is a sample requirements.txt entry:

```
numpy
matplotlib
tensorflow
keras
keras-hub
scikit-learn
```

If you encounter missing package errors, install the relevant packages with `pip install <package-name>`.

## Results 

|     Model     |    Accuracy   |   Precision   |     Recall (healthy)    |    F1-score (healthy)   |  Recall (malnourished)  | F1-score (malnourished) |
| ------------- | ------------- | ------------- | ----------------------- | ----------------------- | ----------------------- | ----------------------- |  
|     VGG-16    |      0.89     |      0.90     |           0.64          |           0.75          |           0.97          |           0.93          |
|     VGG-19    |      0.87     |      0.82     |           0.64          |           0.72          |           0.95          |           0.91          |
|   ResNet-50   |      0.93     |      0.92     |           0.79          |           0.85          |           0.97          |           0.95          |


