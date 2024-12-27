# Arabic Text Classification Using Logistic Regression

This project focuses on classifying Arabic text into various categories using a Logistic Regression model. It also incorporates a rule-based classifier as a baseline. The dataset is structured with text files organized in folders based on their categories.

---

## Table of Contents
- [Getting Started](#getting-started)
- [Data Preprocessing](#data-preprocessing)
- [Classification Models](#classification-models)
  - [Rule-Based Classifier](#rule-based-classifier)
  - [Logistic Regression](#logistic-regression)
- [Team Members](#team-members)

---

## Getting Started

### Prerequisites
Ensure you have the following libraries installed:
- `os`
- `pandas`
- `nltk`
- `scikit-learn`

You can install them using:

pip install -r requirements.txt

## Dataset Structure
The dataset should be organized as follows:

/main_folder
    /category1
        file1.txt
        file2.txt
    /category2
        file3.txt
        file4.txt
Each folder name represents a category, and the text files within it are the documents.

## Data Preprocessing

## Text Cleaning
The preprocessText function performs:

Removal of special characters and diacritics.
Tokenization and filtering of stopwords.
Conversion to a clean text format for modeling.
Label Encoding
Categories are encoded into numeric labels using LabelEncoder.

## Classification Models

Rule-Based Classifier
A dictionary-based classifier uses predefined keywords for each category. This is useful as a baseline model for comparison.

Example:

text = "الاقتصاد والبنوك"
predicted_category = Dictionary_based_Classifier(text)
print(predicted_category)  # Output: 'Finance'
Performance

## A classification report is generated for evaluation.

Logistic Regression
A pipeline using TfidfVectorizer and LogisticRegression is built for classification. The model achieves high accuracy on test data.

## Training

pipeLine.fit(X_train, y_train)
Evaluation

Accuracy and classification reports are provided for detailed analysis.

## Team Members

Rayan Beshawri
Abdulaziz Dawood
Ahmed Salem
Hassan Kalantan
