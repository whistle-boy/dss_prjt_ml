# SOCAR Auto Insurance Fraud Prediction

The project carried out as part of 15th Data Science School.
The project hopes contribute to the auto industry by reducing auto insurance fraud.


About Data
The car crash data provided by SOCAR, a leading car sharing service in South Korea. 
The data set consist of 16,000 car crash cases with 35 columns.

Performance Evaluation Standard

- The baseline was determined by using Class 14's performance.
  - accuracy 0.493, precision 0.003, recall 0.714 
  
- Extremly imbalanced data
  - only 41 cases were fraud out of 16,000 cases. If cases are predicted as "no fraud", accuracy wil be 0.997.
  - Thus, precision and recall scores was also used to accurately evaluate the performance. 


Content

- Data Exploration
- Data Preprocessing
- Modeling
- Performance Evaluation
- Conclusion


Data Exploration
- 33 features did not show signifcant corellation
- extreme data imbalance

PreProcessing
- attempted various preprocessing methods, but the performance did not improve significantly
- The preprocessing resulted the best peformance is ..
