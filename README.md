
Project Title  
Analysis of Global Happiness Index Trends (2024–2025): Factors, Regional Differences, and Predictive Modeling**  

Author
Longbo Xiang

Abstract  
This study analyzes the World Happiness Index data from 2024 to 2025 to explore trends in global happiness levels, regional disparities, and influencing factors. Using data preprocessing techniques (cleaning, transformation, feature selection) and a Random Forest regression model, the research identifies key drivers of happiness scores and predicts 2025 values. Findings reveal consistent high happiness in Nordic and Western countries, low scores in conflict-ridden regions, and significant variation in Asia and Africa. The model demonstrates moderate predictive performance, highlighting the importance of economic stability, social support, and health expectancy. Future research could incorporate real-time data and expand cultural factors.  


Rationale  
Understanding happiness trends is critical for policymakers to prioritize well-being amid global challenges like economic instability and social unrest. This study provides evidence-based insights to guide policy interventions and resource allocation, contributing to sustainable development goals (SDGs) focused on quality of life.  


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

2. Model Development:  
   Algorithm: Random Forest Regressor with 100 estimators.  
   Training: 80% training set, 20% test set (stratified by year, `random_state=42` for reproducibility).  
   Evaluation: Mean Squared Error (MSE) and R² score to measure prediction accuracy.  


Results  
1. Trends and Regional Patterns:  
   High-happiness countries (2024–2025): Nordic nations (Finland, Norway, Denmark) consistently scored >7.5, driven by strong social welfare, high life expectancy, and low corruption.  
   Low-happiness countries: Afghanistan, Syria, and African nations (e.g., Lesotho) scored <4.0, linked to political instability, poverty, and poor healthcare.  
   Asia: Mixed results (e.g., Israel and Australia in top 10; South Asian countries mid-range).  

2. Model Performance:  
   MSE: 0.32 (lower error indicates better fit).  
   R²: 0.78 (model explains 78% of happiness score variance).  
   Key predictors: Economic output (GDP per capita, ρ=0.82), social support (ρ=0.79), and healthy life expectancy (ρ=0.75) showed strongest correlations.  


Next Steps  
1. Incorporate real-time data (e.g., 2025–2026 surveys) to validate model accuracy.  
2. Explore cultural factors (e.g., religion, social norms) and environmental indicators (e.g., pollution) as additional predictors.  
3. Conduct case studies on countries with significant score fluctuations (e.g., analyze policy changes in Iceland or New Zealand).  


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
