# Customer Review Text Analysis – Home Appliances

## Project Overview

This project was developed as part of the Data Analytics Specialist Internship at Yuva Intern.

The objective is to analyse customer reviews using Natural Language Processing (NLP), identify major complaint themes, understand customer dissatisfaction and provide actionable business recommendations.

## Dataset

- Original reviews: 5,000
- Cleaned reviews: 4,363
- Data period: April 2006 – March 2023
- Product category: Home Appliances
- Labelled validation sample: 300 reviews

## Tools and Technologies

- Python
- Google Colab
- Pandas and NumPy
- NLTK
- VADER Sentiment Analysis
- Gensim LDA
- Scikit-learn
- Matplotlib
- WordCloud

## Project Methodology

1. Data collection and exploratory analysis
2. Text normalisation and tokenisation
3. Duplicate and spam-like review removal
4. Domain-specific stop word handling
5. Lemmatisation
6. VADER sentiment analysis
7. Sentiment validation against star ratings
8. LDA topic modelling and coherence evaluation
9. Complaint theme ranking and trend analysis
10. Label-based validation and supervised classification
11. Business recommendations and reporting

## Key Findings

| Priority | Complaint Theme | Reviews | Negative Reviews |
|---|---|---:|---:|
| 1 | Washing and Cleaning Performance | 644 | 31.8% |
| 2 | Product Fit and Stove Accessories | 500 | 20.8% |
| 3 | Coffee Filters and Brewing Quality | 908 | 10.5% |
| 4 | Replacement Parts and Installation | 1878 | 4.9% |
| 5 | Ice Maker and Freezer Performance | 433 | 10.9% |

Negative reviews are defined as reviews with 1–2 star ratings.

Washing and cleaning performance is the highest-priority theme because of its high negative review percentage and increasing negative rating trend.

## Model Evaluation

| Metric | Actual Result |
|---|---:|
| VADER accuracy against ratings | 79.3% |
| LDA coherence score | 0.4658 |
| Held-out label agreement | 50.0% |
| Overall label agreement | 46.7% |
| Supervised classifier accuracy | 59.7% |

The LDA coherence score exceeded the target of 0.45. However, the held-out agreement did not achieve the required 75% target.

## Business Recommendations

- Prioritise washing and cleaning performance investigations.
- Improve product compatibility information and sizing guides.
- Investigate coffee filter quality and brewing consistency.
- Improve replacement part installation instructions.
- Monitor ice maker and freezer performance complaints.

## Project Deliverables

- [Improved Analysis Notebook](Customer_Review_Text_Analysis_Improved.ipynb)
- [Two-Page Business Insight Report](Customer_Review_Two_Page_Insight_Report.pdf)
- [Labelled Review Dataset](manual_labelling_reviewed.csv)
- [Analysis Outputs and Visualisations](review_analysis_outputs%20%282%29.zip)

## How to Run the Project

1. Download the improved Jupyter notebook.
2. Open the notebook in Google Colab.
3. Install the required libraries using the setup cell.
4. Follow the dataset loading instructions.
5. Execute the notebook cells sequentially.
6. Upload the labelled CSV during the validation stage.
7. Export the generated analysis outputs.

## Limitations

- VADER may misinterpret sarcasm and mixed sentiments.
- LDA topics can overlap across product categories.
- Labelled classes are imbalanced.
- AI-assisted labels require independent human verification.
- The 75% agreement target was not achieved.
- Word clouds and trend charts currently cover the three highest-priority themes.
- Observed associations do not establish the causes of declining ratings.

## Conclusion

This project demonstrates how NLP and machine learning can transform unstructured customer feedback into actionable business insights. The findings provide an exploratory framework for prioritising product improvements and identifying customer dissatisfaction.

Further model refinement and independent validation are required before operational deployment.

## Internship

Data Analytics Specialist Internship – Yuva Intern

