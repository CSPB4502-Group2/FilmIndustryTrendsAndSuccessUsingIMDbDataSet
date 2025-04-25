# CSCI-4502 Data Mining Project

## Project Title
**Film Industry Trends & Success Prediction Using IMDb Data**

## Group 02
This README.md file is updated for Part 6 submission.

## Team Members
- Nathan Harris  
- Mayumi Shimobe  

## Project Description
We leverage the public IMDb datasets (title.basics and title.ratings) along with box‑office data to investigate which movie attributes—such as runtime, release year, genre, and vote counts—drive audience ratings and commercial performance. Through thorough exploratory data analysis, feature engineering, and a suite of predictive models, we aim to answer: 

1. **What factors most strongly influence a movie’s IMDb rating?**  
2. **Can we accurately predict a movie’s rating (continuous) or classify its success (top 20% rating) using only basic metadata?**  
3. **How do linear models compare with tree‑based ensembles (Random Forests, Gradient Boosting) in this context?**

## Code Files
All of code files upto Part 3 has been found in a foler `DataIntegration`.
The main source code for this project can be found in `imdb_movie_success_prediction.ipynb`.

## Key Findings & Answers
- **Univariate & Multivariate Insights:** IMDb ratings follow a roughly Gaussian distribution (peak ~6–7), while vote counts are extremely right‑skewed. Pairwise correlations among features and genres are close to zero, suggesting weak linear relationships.  
- **Regression Results:**  
  - *Linear Regression* achieved RMSE ≈ 0.946, R² ≈ 0.105, explaining only 10.5% of rating variance.  
  - *Random Forest Regressor* improved to RMSE ≈ 1.135, R² ≈ 0.270.  
  - *Gradient Boosted Trees* further boosted performance to RMSE ≈ 1.117, R² ≈ 0.293.  
- **Classification Results (Top 20% “Successful” films):**  
  - *Logistic Regression* hit 79% accuracy but 0% recall on the minority “successful” class.  
  - *Random Forest Classifier* achieved 56% accuracy with 87% recall (but only 30% precision).  
  - *Gradient Boosting Classifier* reached 80% accuracy with 7% recall and 67% precision.  

These results highlight the challenges of severe class imbalance and the benefits of nonlinear, ensemble methods for capturing complex patterns in sparse metadata.

## Application of This Knowledge
Studios and streaming platforms can integrate our predictive pipeline—ranging from data ingestion through model scoring—to inform green‑lighting decisions, marketing spend allocation, release timing, and content curation. Marketers can focus campaigns on attributes our models identify as high‑impact, while recommendation engines can blend these predictions with collaborative filters to surface high‑potential titles to targeted audiences.

## Project Presentation
We’ve recorded a ~5 minute group presentation covering:
- Project motivation & questions
- Data preparation & warehousing
- Exploratory analysis
- Regression & classification models
- Key insights & applications

You can stream the Zoom recording here (passcode: `&JWp3m1@`):
**[02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part6_Video](https://cuboulder.zoom.us/rec/share/sXJLGgcAvDlX5qvMWx88h38uu2SEjh0mE_0mge0gJvutPYITIR42HpaTp3t277jp.oUVHgQOh1y0KfkdA?startTime=1745612852000)**

The presentation slides are here:
**[Download Slide Deck `02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part6.pdf` (PDF)](02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part6.pdf)**

## Final Project Paper
Detailed methodology, results, and discussion can be found in our final report:  
**[Download the Final Report (PDF)](02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part4.pdf)**

## Previous Reports
Below are previous reports:
**[Download the Part1 Report (PDF)](02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part1.pdf)**
**[Download the Part2 Report (PDF)](02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part2.pdf)**
**[Download the Part3 Report (PDF)](02_FilmIndustryTrendsAndSuccessUsingIMDbDataSet_Part3.pdf)**

