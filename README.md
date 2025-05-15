
Project Title  
Analysis of Global Happiness Index Trends (2024–2025): Factors, Regional Differences, and Predictive Modeling**  

Author
Longbo Xiang

Abstract  
This study analyzes the World Happiness Index data from 2024 to 2025 to explore trends in global happiness levels, regional disparities, and influencing factors. Using data preprocessing techniques (cleaning, transformation, feature selection) and machine learning models (Random Forest, Linear Regression, SVM, XGBoost), the research identifies key drivers of happiness scores and predicts 2025 values. Findings reveal consistent high happiness in Nordic and Western countries, low scores in conflict-ridden regions, and significant variation in Asia and Africa. Among models, XGBoost demonstrates the best predictive performance (R² = 0.99), highlighting the critical role of economic stability, social support, and health expectancy. Future research could integrate real-time data and cultural factors to enhance model accuracy.

Rationale  
Understanding happiness trends is critical for policymakers to prioritize well-being amid global challenges like economic instability and social unrest. This study provides evidence-based insights to guide policy interventions and resource allocation, contributing to sustainable development goals (SDGs) focused on quality of life. By comparing multiple predictive models, the research offers a robust framework for identifying effective strategies to enhance happiness metrics.


Research Question  
1. How have happiness scores evolved between 2024 and 2025 across countries?  
2. What factors drive variations in happiness scores among high- and low-ranking nations?  
3. Can a predictive model effectively forecast happiness scores using economic, social, and health indicators?  


Data Sources  
World Happiness Report datasets (2018–2024): Includes happiness scores, economic output (GDP per capita), social support, healthy life expectancy, freedom to make life choices, perceived corruption, and generosity.  
Data format: Structured CSV files with country-level annual observations.  


Methodology  
1. Data Preprocessing:  
   Cleaning: Filled missing values with column means.  
   Transformation: Corrected formatting issues (e.g., commas in numeric fields) and converted columns to appropriate data types.  
   Feature Selection: Retained features with Spearman correlation > 0.2 with happiness scores (excluding "Generosity" due to low correlation).  
   Standardization: Used `StandardScaler` to normalize feature scales.  
2.Data visualization
3. Model Development:  
Algorithms Compared:
       Random Forest Regressor
       Linear Regression
       SVM (with StandardScaler pipeline)
       XGBoost Regressor
Training:
       80% training set, 20% test set (stratified by year, random_state=42 for reproducibility).
Evaluation:
        Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R² score.


Results  
1. Trends and Regional Patterns:  
   High-happiness countries (2024–2025): Nordic nations (Finland, Norway, Denmark) consistently scored >7.5, driven by strong social welfare, high life expectancy, and low corruption.  
   Low-happiness countries: Afghanistan, Syria, and African nations (e.g., Lesotho) scored <4.0, linked to political instability, poverty, and poor healthcare.  
   Asia: Mixed results (e.g., Israel and Australia in top 10; South Asian countries mid-range).  

2. Model Performance:  
Model Performance Comparison
Model	MSE	RMSE	MAE	R²
Random Forest	56420.87	237.53	132.45	0.9847
Linear Regression	72189.32	268.68	154.21	0.9712
SVM	4082213.80	2020.45	710.21	-0.109
XGBoost	36117.96	190.05	56.59	0.990

Key Predictors: Economic output (ρ=0.82), social support (ρ=0.79), and healthy life expectancy (ρ=0.75) showed strongest correlations with happiness scores.
Feature Importance (Random Forest)
Top Factors: Economy (35%), Social Support (32%), Healthy Life Expectancy (18%).
Minor Factors: Freedom (10%), Perceptions of Corruption (5%), Year (0.1%).


Next Steps  
Real-time Data Integration: Validate model accuracy with 2025–2026 survey data.
Cultural and Environmental Factors: Explore religion, social norms, and pollution as additional predictors.
Case Studies: Analyze policy changes in countries with score fluctuations (e.g., Iceland, New Zealand).

Conclusion  
Positive Findings: The model effectively identifies economic and social determinants of happiness, and Nordic/Western countries serve as benchmarks for well-being policies.  
Negative Findings: Persistent low happiness in conflict-affected regions highlights systemic challenges in governance and humanitarian crises.  
Recommendations: Policymakers should prioritize social safety nets, healthcare access, and anti-corruption measures. Future research should address data limitations (e.g., underreporting in authoritarian regimes) and expand cross-cultural frameworks.  
Caveats: Correlational findings do not imply causation, and happiness metrics may lack cultural nuance in non-Western contexts.  


Bibliography  
[Saffari et al., 2009]  
A. Saffari, C. Leistner, J. Santner, M. Godec, and H. Bischof, “On-line Random Forests,” *2009 IEEE 12th International Conference on Computer Vision Workshops (ICCVW)*, Kyoto, Japan, 2009, pp. 1393–1400. doi: 10.1109/ICCVW.2009.5457447.  


Contact and Further Information  
For data access or collaboration, contact [Research Team Email]. Additional visualizations and code are available upon request.
