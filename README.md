# Tax Fraud Detection for New York Property Data

## Overview  
This project addresses the critical issue of property tax fraud within New York City's property database. Tax fraud, such as underreporting property values, misclassifying property types, or manipulating property characteristics, leads to significant revenue losses and an unfair tax burden on compliant property owners.  
This project employs advanced data cleaning, variable creation, dimensionality reduction, and anomaly detection techniques to identify potentially fraudulent properties.

## Key Features  
- **Comprehensive Data Cleaning**: Imputation of missing values for key attributes like ZIP codes, full market values, and lot dimensions.  
- **Advanced Variable Creation**: Generation of size variables, value ratios, and standardized metrics for anomaly detection.  
- **Dimensionality Reduction**: Use of Principal Component Analysis (PCA) to optimize computational efficiency and data interpretability.  
- **Anomaly Detection Algorithms**: Implementation of Isolation Forest and Local Outlier Factor (LOF) to detect outliers.  
- **Combined Scoring Mechanism**: Standardization and integration of results from multiple algorithms for robust fraud detection.  

## Data Description  
The dataset consists of property valuation and assessment data for 1,070,994 properties in New York City during the 2010/11 assessment period. Attributes include borough codes, tax classes, property values, and physical dimensions.

## Project Workflow  
1. **Data Cleaning**  
   - Removed government-owned properties irrelevant for fraud detection.
   - Imputed missing ZIP codes, property dimensions, and valuation fields using grouped averages.
   - Ensured consistency in all fields for subsequent analysis.

2. **Variable Creation**  
   - Created new metrics such as lot area, building volume, and value ratios.
   - Standardized variables using group averages for ZIP codes and tax classes.

3. **Dimensionality Reduction**  
   - Applied Principal Component Analysis (PCA) to reduce the dataset to 10 components while retaining 90% of the variance.

4. **Anomaly Detection**  
   - Used Isolation Forest and LOF to identify anomalous property records.
   - Combined and standardized anomaly scores from both algorithms for enhanced robustness.

5. **Result Analysis**  
   - Examined top flagged properties with high fraud scores.
   - Identified significant irregularities, including inconsistent valuation metrics and unusual size-value ratios.

## Results  
- Several properties exhibited high fraud scores, warranting further investigation.  
- Case studies highlighted discrepancies in reported characteristics, such as unusual valuation ratios and size inconsistencies.  
- Recommendations were made to refine thresholds, incorporate additional data, and develop a user-friendly interface for city authorities.

## Future Enhancements  
- Refining anomaly detection thresholds based on expert feedback.  
- Incorporating additional data sources, such as recent sales records and permits.  
- Developing an interactive dashboard for better visualization and decision-making.  

## Tools and Technologies  
- **Programming Languages**: Python  
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **Techniques**: PCA, Isolation Forest, Local Outlier Factor 
