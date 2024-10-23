# SemEval-2022-Task-4: Patronizing and Condescending Language Detection

This repository contains code and resources for the task of detecting patronizing and condescending language (PCL) in text. The task was part of the SemEval 2022 competition (Task 4, Subtask 1). The goal is to build a binary classification model to predict whether a given text contains PCL.

## Project Objective
Our primary aim is to train a model that surpasses the RoBERTa-base baseline model, which achieved an F1 score of 0.48 on the dev set and 0.49 on the test set. This project explores multiple models, data pre-processing techniques, augmentation strategies, and hyperparameter tuning to improve detection of PCL in the dataset.

## Dataset
The dataset used for training and testing is the **Don't Patronize Me!** dataset, which consists of English news paragraphs from 20 countries. Each paragraph discusses a vulnerable community (e.g., migrants, women, disabled) and is annotated for the presence of patronizing language.

- **Training set**: Annotated paragraphs with binary PCL labels.
- **Dev set**: Public set with available labels for evaluation.
- **Test set**: Private set without labels (evaluated by competition organizers).

## Structure of the Repository

### 1. Main Notebook
- **Purpose**: Train the best model (DeBERTa, BoW, TF-IDF) on the dataset and generate predictions for dev and test sets.
- **Focus**: Primary focus on question 2.a, 2.b, and 2.d from the coursework specification.

### 2. Pre-Processing Notebook
- **Purpose**: Handle data cleaning, tokenization, and feature extraction. Models are also trained here using different pre-processing techniques.
- **Focus**: Supports the implementation of question 2.c and 2.d.

### 3. Pre-Processing Script (`pre-process.py`)
- **Purpose**: Implements an alternative data pre-processing strategy.
- **Focus**: Supports the exploration of pre-processing techniques for question 2.c and 2.d.

### 4. Augmentation Notebook
- **Purpose**: Apply data augmentation techniques to enrich the dataset and improve model generalization.
- **Focus**: Implements augmentation techniques in line with question 2.c and 2.d.

### 5. Sampling Notebook
- **Purpose**: Experiment with different sampling strategies (e.g., upsampling, downsampling) to address the class imbalance.
- **Focus**: Supports question 2.c and 2.d.

### 6. Hypertuning Notebook
- **Purpose**: Perform hyperparameter tuning to optimize model performance.
- **Focus**: Addresses question 2.e (hyperparameter tuning).

### 7. Analysis Notebook
- **Purpose**: Analyze the model's performance and answer analytical questions.
- **Focus**: Addresses question 3 (analysis of model performance).

### 8. Q1 Notebook
- **Purpose**: Dedicated notebook to address the first question from the coursework specification.
- **Focus**: Question 1.

### 9. Scheduler Notebook
- **Purpose**: Implements a learning rate scheduler to explore its impact on model performance.
- **Focus**: Experimentation with scheduling strategies for question 2.b.

## How to Use the Repository
1. Clone the repository: `git clone https://github.com/your-repo-url`
2. Install dependencies: `pip install -r requirements.txt`
3. Follow the notebooks in the order of their listing above for a complete workflow from data pre-processing to model training and evaluation.

## Results
- **F1 Score**: The final model (DeBERTa) achieved an F1 score of **0.58** on the dev set, outperforming the RoBERTa-base baseline.
- Detailed results and analysis are included in the analysis notebook and the final report.

## Report
For a detailed explanation of the methodology, model performance, and analysis, refer to the [report]().

## References
- [SemEval 2022 Task 4](https://sites.google.com/view/pcl-detection-semeval2022/)
- [Don't Patronize Me! Dataset](https://github.com/CRLala/NLPLabs-2024/tree/main/Dont_Patronize_Me_Trainingset)

## Contributors
- Michael Hollins 
- Vinayak Modi 
- Kangle Yuan

