# Amazon Employee Review Analysis with NLP

This project applies natural language processing (NLP) techniques to analyze Amazon employee reviews, uncovering themes related to leadership, company culture, and employee attrition. It combines sentiment analysis, topic modeling, and semantic similarity using both rule-based and deep learning approaches. A custom fine-tuned BERT sentiment classifier was also developed for improved prediction accuracy.

---

## 🧠 Project Summary

- **Goal**: Derive insights from large-scale employee reviews to support organizational strategy.
- **Approach**:
  - Collected and cleaned review text data
  - Applied sentiment analysis using VADER and BERT
  - Extracted latent themes using BERTopic
  - Measured semantic similarity across themes using sentence embeddings
  - Fine-tuned a BERT classifier with PyTorch for domain-specific sentiment scoring
  - Structured results for cross-sectional analysis by department and location

---

## 📁 Project Structure

```

amazon-employee-review-nlp/
│
├── notebooks/
│   ├── vader\_sentiment\_analysis.ipynb     # Rule-based sentiment scoring
│   ├── bertopic\_modeling.ipynb            # Topic modeling on reviews
│   └── bert\_finetuning\_sentiment.ipynb    # BERT classifier fine-tuning with PyTorch
│
├── data/
│   ├── raw\_reviews.csv                    # Raw scraped or downloaded reviews
│   └── processed\_reviews.csv              # Cleaned and labeled dataset
│
├── sql/
│   └── review\_summary\_queries.sql         # SQL queries for department/location aggregation
│
├── requirements.txt                       # Python dependencies
└── README.md                              # Project documentation

````

---

## ⚙️ Technologies Used

- **Python**
  - pandas, nltk, scikit-learn, seaborn, matplotlib
- **NLP Libraries**
  - VADER (SentimentIntensityAnalyzer)
  - BERTopic (Topic Modeling)
  - SentenceTransformers (BERT Embeddings)
  - PyTorch (BERT fine-tuning)
- **SQL**
  - For structured analysis and aggregation by department and location

---

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/amazon-employee-review-nlp.git
cd amazon-employee-review-nlp
````

2. Install required Python packages:

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

1. **VADER Sentiment Analysis**
   Run `vader_sentiment_analysis.ipynb` to apply rule-based sentiment scoring.

2. **Topic Modeling with BERTopic**
   Use `bertopic_modeling.ipynb` to extract discussion themes.

3. **BERT Sentiment Fine-Tuning**
   Train and evaluate a fine-tuned BERT classifier using `bert_finetuning_sentiment.ipynb`.

4. **Structured Analysis with SQL**
   Use the SQL scripts in the `sql/` folder to analyze sentiment and topic trends by department or location.

---

## 📊 Key Features

* **Multi-method Sentiment Analysis**: Compare traditional rule-based methods with transformer-based models.
* **Topic Discovery**: Extract key topics across thousands of reviews.
* **Semantic Similarity**: Group similar reviews to understand cultural and leadership signals.
* **Fine-tuned Classifier**: Custom BERT model optimized for employee review sentiment.
* **SQL Integration**: Structure NLP outputs for business intelligence-style queries.

---

## 🔍 Insights & Use Cases

* Track recurring concerns related to leadership or culture
* Identify departments with declining sentiment trends
* Compare sentiment across locations or job levels
* Enhance HR analytics with unstructured review data

---

## 📈 Sample KPIs & Metrics

| Metric                 | Description                                             |
| ---------------------- | ------------------------------------------------------- |
| Review Sentiment Score | Numerical score from VADER or BERT sentiment classifier |
| Top Topics             | Extracted themes using BERTopic                         |
| Similarity Clusters    | Groups of semantically related review content           |
| Sentiment by Location  | Aggregated review sentiment per region or office        |

---

## 🛠️ Future Enhancements

* Add temporal analysis to track sentiment changes over time
* Integrate dashboard (Tableau/Power BI) for stakeholder reporting
* Deploy as an API to process live review feeds

---

## 📄 License

This project is intended for educational and research purposes.

---

## 👤 Author

**Anthony Baptiste**
[LinkedIn](https://www.linkedin.com/in/anthony-baptiste00)
[Portfolio](https://antbap23.github.io/portfolio)


