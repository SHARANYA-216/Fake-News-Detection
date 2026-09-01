# Fake News Detection Using Machine Learning

## Project Overview

Fake News Detection is a **Machine Learning and Natural Language Processing (NLP)** project that classifies news articles as **Fake or Real** based on their textual content.

The project preprocesses news articles, converts the text into numerical features using **TF-IDF Vectorization**, and applies multiple machine learning classification algorithms to predict whether a given news article is genuine or misleading.

## Features

* Text preprocessing and cleaning
* Removal of unwanted characters, URLs, and noise
* TF-IDF-based text feature extraction
* Training and evaluation of multiple machine learning models
* Prediction of Fake and Real news
* Manual testing of new or unseen news articles
* Comparison of predictions from different classifiers

## Machine Learning Algorithms

The following classification algorithms are implemented:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Gradient Boosting Classifier**
4. **Random Forest Classifier**

The models are trained using features generated through **TF-IDF Vectorization**.

## Project Workflow

```text
News Dataset
     ↓
Data Loading
     ↓
Data Cleaning and Preprocessing
     ↓
Train-Test Split
     ↓
TF-IDF Vectorization
     ↓
Machine Learning Models
     ↓
Model Evaluation
     ↓
Fake / Real Prediction
```

## Dataset

The project uses two CSV files:

* `Fake.csv` – Contains fake news articles
* `True.csv` – Contains real news articles

Each dataset contains textual news information that is used for training and evaluating the classification models.

> **Note:** The dataset files are not included in this repository if they are subject to third-party licensing or distribution restrictions.

## Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Scikit-learn** – Machine learning and model evaluation
* **TF-IDF Vectorizer** – Text feature extraction
* **Matplotlib** – Data visualization
* **Seaborn** – Data visualization
* **Jupyter Notebook** – Development environment

## Project Structure

```text
Fake-News-Detection/
│
├── fakenewsdetect1.ipynb
├── Fake.csv
├── True.csv
├── README.md
└── requirements.txt
```

## Installation

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Navigate to the project directory

```bash
cd Fake-News-Detection
```

### 3. Install the required dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

Or, if a `requirements.txt` file is provided:

```bash
pip install -r requirements.txt
```

## How to Run

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
fakenewsdetect1.ipynb
```

Then select:

**Kernel → Restart & Run All**

Make sure `Fake.csv` and `True.csv` are present in the project directory before running the notebook.

## Making a Prediction

The notebook includes a manual testing function that allows users to enter their own news article.

Example:

```text
NASA announces discovery of a new planet in a distant galaxy
```

The system processes the entered text using the same preprocessing and TF-IDF transformation used during training and generates predictions using the trained classifiers.

The predictions can be compared across:

* Logistic Regression
* Decision Tree
* Gradient Boosting
* Random Forest

## Model Evaluation

The trained models are evaluated using classification performance metrics such as:

* Accuracy
* Precision
* Recall
* F1-Score
* Classification Report

This allows the performance of the different classifiers to be compared.

## Objective

The primary objective of this project is to demonstrate how **Machine Learning and NLP techniques can be applied to automatically identify potentially fake news based on textual patterns**.

## Future Improvements

* Develop a web interface using **Streamlit or React**
* Deploy the trained model as a **REST API using FastAPI**
* Improve accuracy using advanced NLP techniques
* Experiment with deep learning and transformer-based models
* Add real-time news verification using trusted news sources
* Deploy the application to a cloud platform

## Author

**Sharanya Srinivas**

AI and ML Engineering Student

---

If you found this project useful, consider giving the repository a star.
