# Best Buy Canada Review Sentiment Analysis

## 1. Project Overview
This project analyzes customer reviews for the refurbished
Excellent Apple iPhone 14 128GB Midnight Unlocked on Best Buy Canada.

The goal is to understand customer sentiment using Python and VADER
sentiment analysis.

## 2. Data Collection
- Source: Best Buy Canada product review page
- Product code: 16553704
- Product URL: https://www.bestbuy.ca/en-ca/product/refurbished-excellent-apple-iphone-14-128gb-midnight-unlocked/16553704
- Total reviews analyzed: 50
- Collection method: Reviews were collected manually from publicly
  available product reviews after automated requests were reset.

## 3. Data Fields
The dataset includes primary key, title, review text, date, rating,
source, and reviewer name. Sentiment results include a sentiment label
and compound score.

## 4. Sentiment Analysis Method
VADER was used to calculate a compound sentiment score for each review:
- Positive: compound score >= 0.05
- Neutral: compound score > -0.05 and < 0.05
- Negative: compound score <= -0.05

## 5. Results
| Sentiment | Number of reviews |
|---|---:|
| Positive | 39 |
| Neutral | 1 |
| Negative | 10 |
| Total | 50 |

Average star rating: 3.46 out of 5.

## 6. Data Quality
- Total records: 50
- Unique review IDs: 50
- Missing review titles: 0
- Missing review text: 0
- Duplicate review IDs: 0

## 7. Challenges
Automated requests to the Best Buy Canada website were reset.
Reviews were therefore collected manually from the publicly accessible
product page. This approach took additional time and required checking
the records for completeness and duplicate IDs.

## 8. Limitations
The dataset contains 50 reviews for one product, so it may not
represent all Best Buy customers or products. VADER is a
rule-based sentiment tool and may misinterpret sarcasm, context,
or product-specific language. Sentiment labels reflect review text,
not necessarily the star rating.

## 9. Deliverables
- Notebook: bestbuy_reviews.ipynb
- Original dataset: data/bestbuy_reviews.csv
- Sentiment CSV: data/bestbuy_reviews_with_sentiment.csv
- Sentiment Excel file: data/bestbuy_reviews_with_sentiment.xlsx
- Sentiment chart: data/sentiment_chart.png
- This report: sentiment_analysis_report.md

## 10. Conclusion
The sentiment analysis categorizes the collected customer reviews
into positive, neutral, and negative groups. These results can help
stakeholders understand customer feedback and identify areas that may
need attention.
