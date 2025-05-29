
# 📧Spam Ham: Separating the Good from the Spam

Spam Ham is a text classification project that utilizes Natural Language Processing (NLP) and Machine Learning to differentiate between spam and legitimate messages. It leverages TF-IDF vectorization and Logistic Regression for effective classification, complemented by data visualization and model evaluation for insightful analysis.





## 📁 Dataset Description
This project utilizes a dataset formatted as a structured file. Each message is labeled with:

1. Overview 
- this dataset consists of 5,171 text message, categorized as spam or ham (non-spam)
- It is designed for Natural Language Processing (NLP) tasks, particularly spam classification using machine learning.

2. Structure & Features
- Total Rows: 5,171 messages.
- Spam Messages: 1,499 instances labeled as spam.
- Ham Messages: 3,672 instances labeled as non-spam.
- Key Columns:
- `text` – Contains the actual message content.
- `label` – Indicates whether the message is Spam (1) or Ham (0).


3.  Label Distribution
- The dataset contains approximately 28.99% spam messages and 71.01% ham messages.
- A visualization of spam vs. ham proportions can be useful (e.g., bar chart or pie chart).

4. Preprocessing & Data Cleaning
- Messages may undergo cleaning steps like lowercasing, punctuation removal, stopword filtering to improve classification
- Feature extraction techniques such as TF-IDF, word embeddings, or Bag-of-Words can be applied.
## 📊Visualization
1. Spam vs. Ham Distribution (Pie Chart)
- Displays the overall proportion of spam and ham messages.
- Helps in understanding the dataset imbalance, which can influence model performance.
- A clear percentage breakdown provides insights into how prevalent spam messages are.

2. Spam and Ham Count (Count Plot)
- Shows the absolute count of spam vs. ham messages.
- Helps visualize dataset composition in terms of individual message occurrences.
- Useful for understanding whether a balanced dataset is available for training.

3. Message Length Distribution (Histogram)
- Analyzes how the length of spam and ham messages differ.
- Helps determine whether spam messages tend to be shorter or longer compared to ham.
- A Kernel Density Estimation (KDE) curve adds smooth visualization to spot trends.

4. Most Common Words in Spam & Ham (Count Word Plot)
- Identifies frequently appearing words in spam vs. ham messages.
- Helps reveal spam-triggering words such as "free," "win," "offer," etc.
- Supports feature engineering by highlighting terms that strongly indicate spam.
## 🧠 Machine Learning Pipeline

  1. data preparation
   - cleaning and preprocesssing text.
   - Feature extraction using NLP techniques ( e.g., TF-IDF)
  2. Model Development 
  - Dataset split into training and testing sets.
  - Applied model algorithms such as [your algorithm, e.g., Logistic Regression]
  3. Model Evaluation 
  - preformance metrics: accuracy, precision, recall,F1-scrose 
  - Visual preformance indicators (e.g., confusion matrix).
  4. Usage in Model Training
- The dataset can be split into training and testing sets for machine learning models.
- Common algorithms used include Logistic Regression, Naive Bayes, and Neural Networks for spam filtering
## 🧪 Example Use Case
```python 
import pandas as pd
def predict_email(email):
    # Some logic to classify the email as spam or ham
    return "spam"  # Example return value
new_email = "Get cheap watches and discount medicines now!"
result = predict_email(new_email)
print("Prediction:", result)