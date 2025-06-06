Project: Employee Sentiment Analysis
This project analyzes a dataset of employee email messages to assess sentiment, identify trends, and flag potential flight risks. The analysis involves sentiment labeling using NLP, exploratory data analysis, monthly employee scoring, and predictive modeling.
The full, detailed analysis and implementation can be found in the sentiment_analysis.ipynb notebook. A comprehensive report is available in the Final Report.docx file.
Key Findings & Summary
Employees Identified as Flight Risk (7)
The following employees have been identified as potential flight risks based on the criteria of sending 4 or more negative emails within a rolling 30-day period.
bobette.riner@ipgdirect.com
eric.bass@enron.com
john.arnold@enron.com
johnny.palmer@enron.com
kayne.coulter@enron.com
patti.thompson@enron.com
sally.beck@enron.com
Employee Sentiment Ranking
Monthly rankings were generated to identify the top 3 most positive and top 3 most negative employees based on their aggregated sentiment scores. These detailed monthly lists provide insights into sentiment fluctuations over time and can be found in the main notebook and the final report.
Overall Sentiment Distribution
The dataset of 2,191 messages was analyzed using the VADER sentiment library. The overall sentiment is predominantly positive:
Positive: 1574 messages (71.8%)
Neutral: 444 messages (20.3%)
Negative: 173 messages (7.9%)
While negative sentiment is the smallest category, its concentration among specific employees is a key indicator for the flight risk analysis.
Predictive Model Insights
A linear regression model was developed to predict sentiment scores based on features like message length, word count, and monthly message frequency.
The model achieved an R-squared (R²) value of 0.15, indicating that these simple features explain only 15% of the variance in sentiment scores.
This suggests that a linear model with basic metadata features is too simplistic to accurately capture the complexity of sentiment.
Recommendations
For Management/HR:
Focus immediate attention on the 7 employees identified as flight risks. Proactive engagement could help address underlying issues and improve retention.
Review the monthly negative sentiment rankings in the full report to identify other employees who may be trending negatively over time.
For Future Analysis:
To build a more powerful predictive model, more advanced NLP features should be incorporated, such as TF-IDF, n-grams, or word embeddings (e.g., Word2Vec, BERT).
Exploring non-linear models (e.g., Gradient Boosting, Random Forest) may also yield better predictive performance.
