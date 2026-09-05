# A/B Testing & Statistical Analysis

## Project Overview
This project applies **statistical hypothesis testing** to validate A/B test results using the Kaggle `ab_data.csv` dataset.  
The goal is to determine whether the new landing page (Treatment) performs significantly better than the old page (Control) in terms of conversion rates.  
We also calculate confidence intervals, effect sizes, and provide actionable business recommendations.

---

## Learning Objectives
- Design and analyze A/B tests with statistical rigor  
- Perform hypothesis testing (Chi-Square test for conversion rates)  
- Interpret p-values and confidence intervals correctly  
- Measure practical significance using effect size (Cohen’s h)  
- Translate statistical findings into business insights  

---

## Dataset Information
- **Source:** Kaggle – A/B Testing Dataset (`ab_data.csv`)  
- **Columns:**
  - `user_id`: Unique identifier  
  - `group`: Control or Treatment assignment  
  - `landing_page`: Page shown (old vs new)  
  - `converted`: Binary outcome (0 = no conversion, 1 = conversion)  

---

## Methodology
1. **Data Exploration**
   - Checked sample sizes for Control vs Treatment groups  
   - Calculated overall conversion rate  
   - Verified balance between groups  

2. **Hypothesis Testing**
   - Performed Chi-Square test to compare conversion rates  
   - Null Hypothesis (H0): No difference between Control and Treatment conversion rates  
   - Alternative Hypothesis (H1): Treatment conversion rate is different from Control  

3. **Confidence Intervals**
   - Calculated 95% confidence intervals for conversion rates in each group  

4. **Effect Size**
   - Measured Cohen’s h to assess practical significance  

5. **Business Insights**
   - Compared conversion rates  
   - Recommended rollout only if Treatment group shows statistically significant improvement  

---

## Results (Mock Dataset Example)
- **Control Conversion Rate:** 40%  
- **Treatment Conversion Rate:** 60%  
- **Chi-Square p-value:** 0.5271 (not significant)  
- **Cohen’s h:** 0.40 (medium effect size)  
- **Recommendation:** No rollout — difference not statistically significant  

---

## Deliverables
- Jupyter Notebook with all analysis steps  
- Statistical summary (Chi-Square test, confidence intervals, effect size)  
- Business recommendation report  
- Optional: Customer segmentation extension using clustering  

---

## Tools & Libraries
- Python  
- Pandas, NumPy  
- SciPy (stats)  
- Matplotlib, Seaborn  
