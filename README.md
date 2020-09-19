# Plagiarism Project, Machine Learning Deployment

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Project Overview

In this project, we build a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

This project is broken down into three main notebooks:

**Notebook 1: Data Exploration**
* Loading in the corpus of plagiarism text data.
* Exploring the existing data features and the data distribution.
* This first notebook is **not** required in final project submission.

**Notebook 2: Feature Engineering**

* Clean and pre-process the text data.
* Defining features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Selecting "good" features, by analyzing the correlations between different features.
* Creating train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Your Model in SageMaker**

* Uploading our train/test feature data to S3.
* Defining a binary classification model and a training script.
* Training our model and deploy it using SageMaker.
* Evaluating our deployed classifier.

---

Please see the [README](https://github.com/udacity/ML_SageMaker_Studies/tree/master/README.md) in the root directory for instructions on setting up a SageMaker notebook and downloading the project files (as well as the other notebooks).

