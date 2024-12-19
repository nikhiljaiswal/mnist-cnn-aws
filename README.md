# 🤖 MNIST CNN Model AWS

A step by step improvement of CNN model for MNIST digit classification along with execution in the cloud (AWS)

## 🏗 Model Architecture ️

The model follows a carefully designed architecture with the following key components:


## 🎯 Model Requirements
- Parameters: < 8,000
- Accuracy: > 99.4% on test set
- Training: < 15 epochs


## 🚀 Quick Start

###  Training & Testing

##### Train & Test the model:

- There are different Jupyter Notebook files based on the analysis and improvements

- Execute each Jupyter Notebook file to train and test the model performance

## Different Models

### Model 1: The Skeleton

**Reference:** **[Model_1](path/to/model.ipynb)**  

**Target:**  
Get the basic skeleton right.  

- **Parameters:** < 8000 parameters  
- **Epochs:** ≤ 15  

**Results:**  
- **Parameters:** 5.73k  
- **Best Train Accuracy:** 99.14%  
- **Best Test Accuracy:** 99.29%  

**Analysis:**  
The model is lighter; however, we can increase its capacity to fit under 8k parameters.  

---

### Model 2: Increase the Capacity

**Reference:** **[Model_3](path/to/model.ipynb)**

**Target:**  
Increase model capacity by adding more layers.  

**Results:**  
- **Parameters:** 7.3k  
- **Best Train Accuracy:** 99.27%  
- **Best Test Accuracy:** 99.33%  

**Analysis:**  
The model is not overfitting.  
We can add image augmentation techniques to further improve test accuracy.  

---

### Model 3: Image Augmentation

**Reference:** **[Model_3](path/to/model.ipynb)**

**Target:**  
Add image augmentation techniques such as rotation, translation, scaling, etc.  

**Results:**  
- **Parameters:** 7.3k  
- **Best Train Accuracy:** 98.97%  
- **Best Test Accuracy:** 99.46%  

**Analysis:**  
The model is underfitting now, which is acceptable as the training data has been made harder.  
The test accuracy improvement indicates that the test data contained some transformation differences compared to the training dataset.  


## 🔄 AWS Training

Created a Notebook Instance on AWS SageMaker & executed **Model_3**

- #### Notebook Instance Creation
![Training Logs](images/aws_instance_creation.png)

- #### Model Training Logs
![Training Logs](images/aws_training.png)




