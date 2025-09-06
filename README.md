# Advertisement Click Prediction using Logistic Regression  

## Overview  
This project applies Logistic Regression, a supervised machine learning algorithm, to predict whether a user will click on an online advertisement.  
From a business perspective, the ability to anticipate ad clicks is critical for optimizing marketing campaigns, reducing wasted budget, and maximizing Return on Investment (ROI).  
The project demonstrates how data preprocessing, modeling, and evaluation can be combined to deliver actionable business insights for digital marketing teams.  

## Dataset  
The dataset contains consumer-level information including:  
- Daily Time Spent on Site (minutes)  
- Age (years)  
- Area Income (average income of user’s area)  
- Daily Internet Usage (minutes)  
- Ad Topic Line (headline of the ad)  
- City and Country  
- Male (gender flag)  
- Timestamp (time of interaction)  
- Clicked on Ad (target: 0 = No, 1 = Yes)  

The dataset enables a direct link between demographic, behavioral, and contextual features and the likelihood of clicking on an ad.  

## Methodology  
### Data Preprocessing  
- Cleaned and structured categorical & numerical variables.  
- Split data into training and test sets.  

### Model Selection  
- Applied Logistic Regression due to its interpretability and strong performance on binary classification tasks.  
- Hyperparameter tuning with cross-validation ensured optimal performance.  

### Evaluation Metrics  
- Accuracy  
- Precision, Recall, F1-score  
- Confusion Matrix  

These metrics were chosen to evaluate not only correctness but also business-critical errors (e.g., predicting non-clickers as clickers).  

## Key Findings  
**Age is a critical driver**  
- Younger users (below ~35) tend to spend more time online but are less likely to click ads.  
- Older users (40+) show higher click rates, even with moderate internet usage.  
- Business Action: Ads with persuasive or need-based messaging should target older segments. Younger users may need more engaging, interactive ad formats.  

**Internet Usage as a filter**  
- Very high daily internet usage correlates with lower ad clicks (likely ad fatigue or banner blindness).  
- Moderate usage customers engage more.  
- Business Action: Avoid overspending ad budget on “always-online” profiles; instead, target balanced users for higher ROI.  

**Income vs. Clicks**  
- High-income areas don’t always translate to higher click-through. Many high-income customers ignore ads, possibly due to selective buying behavior.  
- Business Action: For affluent customers, campaigns should highlight exclusivity, premium offers, or lifestyle alignment.  

**Model Reliability**  
- Accuracy: 96–97% (train and test very close → no overfitting).  
- Precision & Recall ~0.96 → The model not only predicts accurately but also minimizes wasted targeting.  
- Business Action: Marketing teams can confidently use predictions to focus spend only on likely clickers.  

## Business Value  
- Optimized Budget Allocation: By predicting non-clickers upfront, marketing teams avoid wasting impressions, reallocating spend to more promising audiences.  
- Improved Campaign Design: Segment-specific insights (e.g., older users = higher clicks, younger users = lower clicks) allow tailored ad creatives.  
- Revenue Growth Potential: Even a small % improvement in click prediction accuracy can translate into significant cost savings and higher conversions at scale.  
- Strategic Decision-Making: Data-driven evidence helps prioritize campaigns toward audiences that convert, rather than broad generic targeting.  

## Model Performance Summary  

| Metric     | Train Set | Test Set |
|------------|-----------|----------|
| Accuracy   | 97.14%    | 96.67%   |
| Precision  | ~0.97     | ~0.96    |
| Recall     | ~0.97     | ~0.96    |
| F1-score   | ~0.97     | ~0.96    |

Insight: Training and test scores are nearly identical → the model generalizes well and is business-ready.  

## Future Directions  
### Campaign Personalization  
- Run A/B tests on ad creatives for “older likely-clickers” vs. “younger less-engaged users”.  
- Use behavioral targeting (time of day, device type).  

### Model Extensions  
- Compare with ensemble models (Random Forest, Gradient Boosting).  
- Integrate real-time clickstream data for live targeting.  

### Dashboard for Marketing Teams  
- Deploy model outputs into an interactive dashboard for campaign managers.  

## Conclusion  
This project demonstrates that predictive modeling can directly enhance digital marketing ROI when paired with business interpretation.  
We identified which customer groups drive ad engagement.  
We built a reliable predictive model with over 96% accuracy.  
We translated outputs into clear actions:  
- Target older, moderately active internet users.  
- Avoid overspending on heavy internet users.  
- Design premium/exclusive campaigns for affluent customers.  

By bridging data science and business insights, this project shows how companies can spend smarter, convert better, and grow faster.  
