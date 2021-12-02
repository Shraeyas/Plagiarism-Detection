# Plagiarism-Detection
---
### This repository contains the code for detecting plagiarism in documents.

##### The code for the deployed server is present [HERE](https://github.com/Shraeyas/Plagiarism-Detection-Server-Deployment)

##### The Code for the android application is present [HERE](https://github.com/Shraeyas/Plagiarism-Detection-Android)

---

### The description of various notebooks (in brief) is below.

### Part-1-Preprocessing.ipynb : 
```
Performed pre-processing of the data.
1. Grabbed the raw text of all the files
2. Performed Pre-processing on the data
   a. Remove Stopwords
   b. Remove any special characters
   c. Convert the sentence to Lowercase
   d. Tokenize the sentence
   e. Perform Stemming
   f. Remove words that contain only digits
```

### Part-2-Model_Building.ipynb : 
```
1. Grabbed the data processed in Part-1
2. Converted all data to TaggedDocuments for Doc2Vec
3. Trained the model using the Tagged data
4. Saved the model file on disk for future use
```
### Part-3-Test-The-Model.ipynb :
```
1. Testing the models Performance
```
---

### Inference with Pre-Trained model
```
There is a pre-trained Doc2Vec model present which has been trained on 20Newsgroups dataset.
Part-3-Test-The-Model.ipynb file can be referred if you wish to inference on the pre-trained model.
```
---
### Training your own model

##### The Pre-Processing in Part-1-Preprocessing.ipynb has been done for the 20Newsgroups dataset.
##### To train your own model (on 20Newsgroups dataset), follow these steps :
```
1. Clone the repository (duh).
2. Create 3 folders, rename them to "dataset_20news", "dataset_test", "models" and "dataset_processed"
3. Download the Original 20 Newsgroups data set from http://qwone.com/~jason/20Newsgroups/ and extract it to the "dataset_20news" folder.
The folder structure should look like :
    dataset_20news
    |___ 20_newsgroups
       |___...
       |___ comp.graphics
       |___ comp.os.ms-windows.misc
       |___ sci.space
       |___...
4. Follow the steps in Part-1 and Part-2 Notebooks.
```