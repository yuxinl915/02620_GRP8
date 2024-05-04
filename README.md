# 02620_GRP8
## Introduction
This project contains the code for course 02620 for Group 8. Breast cancer is the most commonly diagnosed cancer among women in the U.S. [1]. Since 1990s, clinicians have used fine needle aspirate (FNA) as a minimally invasive diagnostic alternative to full biopsies. Malignant cell are identified based on increased size and shape abnormality. The WBCD is a statically imaged collection of such samples, classified by oncologists into malignant (‘M’) or benign (‘B’) [2]. Several models have successfully used WBCD to predict patient diagnosis [3]. However, a common scenario during true cancer detection is to have more aspirate samples than clinician-assigned labels. Extra costs must be spent to determine the diagnosis of unlabeled samples further. There is, therefore, a need to identify the sample in which our current model is most likely to
improve if given its true label, for which we should query. To reflect this, we nominate the optimal classifier for WBCD and extend it with an active learning approach, which efficiently updates the model based on its uncertainty regarding unlabeled data.

## Environment Setup
Clone the repository and install the required packages:
```bash
git clone https://github.com/yuxinl915/02620_GRP8.git
cd 02620_GRP8.git
pip install -r requirements.txt
```

## Run the code
knn.ipynb: all relevant work with our self-implemneted kNN classifier;

NaiveBayes.ipynb: all relevant work with our self-implemneted Naive Bayes classifier;

normality_test.ipynb: all relevant work with exploring whether the features following normal distribution;

results.ipynb: all relevant work with the comparisons between methods and plots;

SVM_active_learning.ipynb: all relevant work with the Support Vector Machine (SVM) and active learning strategies; they are in one file because we chose SVM as the base learner in active learning.