# IMDB Movie Reviews: Exploratory Data Analysis (EDA)

## 📌 Project Overview
The entertainment industry heavily relies on user reviews to gauge audience reception, but manually reading thousands of reviews to determine overall sentiment is impossible at scale. This project performs a comprehensive Exploratory Data Analysis (EDA) on a dataset of 50,000 IMDB movie reviews. 

The primary objective is to clean the data, engineer numerical text features, and extract statistical insights to prepare this unstructured text data for advanced Natural Language Processing (NLP) and predictive machine learning models.

## 🗂️ Project Structure
This repository follows standard data science structural practices:

```text
EDA_Project/
│
├── Dataset/
│   └── IMDB Dataset.csv 
│
├── Notebooks/
│   └── EDA.ipynb
│
├── Images/
│   ├── sentiment_distribution.png
│   ├── word_count_histogram.png
│   ├── correlation_heatmap.png
│
├── Report/
│   └── EDA_Report.docx
└── README.md

📊 Key Insights & Findings
Perfect Class Balance: The dataset contains exactly 50% positive and 50% negative reviews, eliminating the need for synthetic data balancing techniques like SMOTE.

Right-Skewed Engagement: The vast majority of users write short reviews (100–200 words), but a highly engaged minority writes massive essays (up to 2,470 words), resulting in over 1,189 statistical outliers.

Sentiment Independence: Review length does not correlate with sentiment. Positive and negative reviews share a nearly identical median length of ~173 words.

Consistent Linguistic Complexity: The average word length remains completely stable (approx. 5.4 characters) across the entire dataset, regardless of how long or short the review is.

High Multicollinearity: There is a near-perfect positive correlation (1.00) between word_count and char_count, indicating that one should be dropped during linear model training to prevent overfitting.

🛠️ Tools & Technologies
Language: Python 3

Data Manipulation: Pandas, NumPy

Statistical Analysis: SciPy (Z-score anomaly detection)

Data Visualization: Matplotlib, Seaborn, WordCloud

🚀 Local Setup & Installation
To run this analysis locally on your Linux machine, follow these terminal commands:

Clone the repository:

Bash
git clone [https://github.com/](https://github.com/)[your-username]/[your-repo-name].git
cd [your-repo-name]
Create and activate a virtual environment:

Bash
python3 -m venv venv
source venv/bin/activate
Install required dependencies:

Bash
pip install pandas numpy scipy matplotlib seaborn wordcloud
Download the Dataset:
Place the IMDB Dataset.csv into the 01_Dataset/ directory before running the scripts.

🔮 Future Work
The structured data from this EDA is now ready for the next phase of the pipeline:

Text Vectorization: Implementing TF-IDF and Word Embeddings (Word2Vec/GloVe).

Baseline Modeling: Training Logistic Regression and Naive Bayes classifiers.

Deep Learning: Fine-tuning transformer models (like BERT) for state-of-the-art sentiment classification.

Author: Dudekula Riyaz
Academic Focus: Computer Science