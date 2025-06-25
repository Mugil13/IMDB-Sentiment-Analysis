[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mugil13/IMDB-Sentiment-Analysis/blob/main/IMDB_Reviews_2_0.ipynb)
[![View on GCP](https://img.shields.io/badge/Live%20Demo-GCP-blue)](https://model1-456105.el.r.appspot.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

# IMDB Movie Reviews - Sentiment Analysis

**IMDB Movie Reviews - Sentiment Analysis** is an end-to-end project that demonstrates text classification using real world movie review data. This project contains multiple machine learning algorithms, ensemble strategies, and automated hyperparameter tuning to achieve optimal performance making it a standout showcase for applied NLP and ML techniques.

---

## Table of Contents
1. [Features](#features)
2. [Dataset & Preprocessing](#dataset--preprocessing)
3. [Models & Techniques](#models--techniques)
4. [Evaluation & Results](#evaluation--results)
5. [Demo & Deployment](#demo--deployment)
6. [Getting Started](#getting-started)
7. [Authors](#authors)
8. [License](#license)

---

## Features
- **10+ ML models used:** Bernoulli Naive Bayes, Logistic Regression, SVM, Decision Tree, Random Forest, AdaBoost, XGBoost.
- **Ensemble Learning:** Implement a Voting Classifier that aggregates predictions for improved stability.
- **Hyperparameter Tuning:** Utilize RandomizedSearchCV and GridSearchCV to find optimal parameters for each model.
- **Evaluation Metrics:** Evaluate using Accuracy, MCC, Precision, Recall, F1-Score, Cohen's Kappa, Confusion Matrix, and Classification Reports.

---

## Dataset & Preprocessing
1. **Source:** 50,000 IMDB movie reviews labeled as positive or negative. (equal split)
2. **Cleaning:** Lowercasing, HTML tag removal, punctuation stripping.
3. **Tokenization & Vectorization:** Convert text to numerical features using TF-IDF with n-gram support.
4. **Train/Test Split:** 80/20 split to assess model generalization.

---

## Models & Techniques
| Model                | Hyperparameters Tuned         |
|----------------------|-------------------------------|
| Bernoulli Naive Bayes| `alpha`                       |
| Logistic Regression  | `C`, `penalty`, `solver`      |
| SVM                  | `C`, `kernel`, `gamma`        |
| Decision Tree        | `max_depth`, `min_samples_split`|
| Random Forest        | `n_estimators`, `max_depth`   |
| AdaBoost             | `n_estimators`, `learning_rate` |
| XGBoost              | `n_estimators`, `max_depth`, `eta` |
| Voting Classifier    | `voting` (hard/soft)          |
| Gradient Boosting    | `n_estimators`                |
| kNN                  |                               |  

---

## Evaluation & Results
- Display detailed classification reports for each model.
- Confusion matrix visualizations.
- Performance metrics comparison in tabular and chart formats.

*For full results and plots, see the notebook.*

---

## Demo & Deployment
- **Colab Notebook:** Execute all steps in order given in the colab notebook. Click the badge above to open it.
- **Live Demo:** Deployed on Google Cloud Platform. Visit the demo link above.

---

## Getting Started
1. **Clone the repository**
   ```bash
   git clone https://github.com/Mugil13/IMDB-Sentiment-Analysis.git
   cd IMDB-Sentiment-Analysis

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run locally**
   ```bash
   jupyter notebook IMDB_Reviews_2_0.ipynb
   ```

---

## Authors

* **Mugilkrishna D U** - [@Mugil13](https://github.com/Mugil13)
* **Neha Shanmitha S** - [@NehaShanmitha](https://github.com/NehaShanmitha)

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
