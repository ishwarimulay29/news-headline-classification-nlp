# News Headline Classification using NLP

This project focuses on classifying news headlines from *Fox News* and *NBC News* using a variety of natural language processing techniques. Our primary goal is to detect the *source* of a headline using its text alone — a step toward understanding media framing and bias through machine learning.

## 📰 Project Overview

We experimented with both classical ML models and deep learning models to build robust text classifiers:
- Logistic Regression
- Random Forest
- Support Vector Machines (SVM)
- Fine-tuned BERT transformer models

Our best model, *Weighted BERT, achieved **91% accuracy* on the validation set and effectively predicted sources for *1,173 unlabeled news headlines*.

## ⚙️ Key Features

- *Binary Classification Task*: Fox News vs NBC News
- *Data*: 3,805 labeled headlines + 1,173 unlabeled
- *Preprocessing*: Regex cleaning, stopword removal, TF-IDF vectorization
- *Evaluation*: Accuracy, F1-score, Confusion Matrix

## 🛠️ Technologies Used

- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- HuggingFace Transformers
- TF-IDF, Logistic Regression, SVM, Random Forest
- BERT (bert-base-uncased)
- Jupyter Notebook

## 📁 Project Structure

| File | Description |
|------|-------------|
| AML_project.ipynb | Code for data cleaning, model training, and evaluation |
| AML_Final_Report.pdf | Final report with methodology and results |
| AML_Presentation.pptx.pdf | Project summary slides |
| Applied_ML_News.pdf | Extended documentation and planning |
| requirements.txt | Python package dependencies |
| .gitignore | Ignoring system and Python cache files |

## 📌 Results

| Model              | Accuracy |
|-------------------|----------|
| Logistic Regression (TF-IDF) | 83% |
| Random Forest      | 80% |
| Linear SVM         | 84% |
| *BERT (Fine-tuned)*        | *91%* |

Final test prediction results:
- Fox News: 1,092 headlines
- NBC News: 81 headlines

## ⚠️ Limitations

- Imbalanced dataset (more Fox headlines)
- Only two sources considered (binary classification)
- Limited to headline text; no full-article context
- Black-box nature of BERT reduces explainability

## 🌱 Future Work

- Add more news sources for multiclass classification
- Integrate SHAP/LIME for model explainability
- Explore temporal framing or bias drift
- Use full news articles for better semantic modeling
