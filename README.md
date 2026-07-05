# 🎬 IMDB Sentiment Analysis: Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Manipulation-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib/Seaborn](https://img.shields.io/badge/Matplotlib_&_Seaborn-Data_Viz-FF6F00?style=for-the-badge&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 📖 Project Overview

How do you quantify human opinion? This project dives into a dataset of **50,000 IMDB movie reviews** to extract structural and statistical meaning from unstructured text.

Before deploying advanced Natural Language Processing (NLP) models, it is critical to understand the data's underlying architecture. This Exploratory Data Analysis (EDA) pipeline cleans the text, engineers quantitative features, handles statistical anomalies, and visualizes linguistic patterns to establish a pristine foundation for machine learning classification.

## 🎯 Key Objectives

- **Data Integrity:** Detect and resolve null values and duplicate records to prevent target leakage.
- **Feature Engineering:** Transform qualitative text strings into quantitative metrics (`word_count`, `char_count`, `avg_word_length`).
- **Statistical Profiling:** Identify central tendencies, variances, and extreme outliers using Z-score mathematics.
- **Visual Storytelling:** Map the relationship between structural text features and user sentiment (Positive vs. Negative).

## 💡 Core Discoveries

1. **The Volume Myth:** Review length is **not** an indicator of sentiment. Positive and negative reviews share a nearly identical median length (~173 words).
2. **Consistent Vocabulary:** Regardless of a review's total length or sentiment, the average word length remains highly stable across the dataset (approx. 5.4 characters).
3. **Perfect Balance:** The dataset maintains a 50/50 split between positive and negative sentiments, eliminating the need for complex, computationally expensive resampling techniques like SMOTE.
4. **Engagement Extremes:** While most users write short reviews, a passionately engaged minority writes essays exceeding 2,000 words, resulting in over 1,180 statistical outliers.

## 📂 Repository Architecture

````text
📦 IMDB-EDA-Project
 ┣ 📂 01_Dataset
 ┃ ┗ 📜 IMDB Dataset.csv (Not uploaded due to GitHub size limits)
 ┣ 📂 02_Notebooks
 ┃ ┗ 📜 EDA_Analysis.py
 ┣ 📂 03_Images
 ┃ ┣ 🖼️ sentiment_distribution.png
 ┃ ┣ 🖼️ word_count_histogram.png
 ┃ ┣ 🖼️ correlation_heatmap.png
 ┃ ┗ 🖼️ wordclouds.png
 ┣ 📂 04_Report
 ┃ ┗ 📜 EDA_Report.docx (Complete 21-section analysis)
 ┗ 📜 README.md

## 🚀 Getting Started (Linux / Pop!_OS)

To reproduce this analysis locally, run the following commands in your terminal:

### 1. Clone the repository:
```bash
git clone https://github.com/codemage05/EDA_Project.git
cd EDA_Project
````

### 2. Set up the virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies:

```bash
pip install pandas numpy scipy matplotlib seaborn wordcloud
```

### 4. Execute:

Ensure your `.csv` dataset is placed inside the `Dataset/` folder, then run your notebook or Python script.

## ⏭️ Next Steps

This EDA sets the stage for the predictive modeling phase, which will include:

- Applying TF-IDF and Word2Vec for semantic vectorization.
- Training baseline classifiers (Logistic Regression, Naive Bayes).
- Exploring transformer-based architectures for advanced sentiment prediction.

## 👨‍💻 Author & Information

- **Author:** Dudekula Riyaz
- **Academic Year:**  Computer Science
- **Institution:** Geethanjali College of Engineering and Technology (GCET)
