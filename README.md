# Water Quality Analysis and Prediction using Machine Learning

This research aims to create a predictive model for water quality, offering an efficient alternative to costly and time-consuming laboratory methods. It's vital for maintaining the quality of surface water, which is a primary source of drinking water and essential for ecological balance.


## Overview
This reserach focuses on the water quality of Delaware River basin which provides water to Philadelphia and New York City. About 6.4 billion gallons of water is withdrawn everyday. It was once a polluted waterbody that is on the road to recovery. 

  
## Approaches & Methods 

- *Data collection*: Global River Water Archive (https://zenodo.org/record/5097437#.YyuqunbMKUl) and United States Geological Survey Catalog (https://www.sciencebase.gov/catalog/item/5e010424e4b0b207aa033d8c) - containing daily values of water parameter variables - dissolved oxygen, fecal coliform, pH, specific conductance, temperature, turbidity, nitrogen, phosphates, alkalinity, chloride & suspended solids.
- The Water Quality Index (WQI) is calculated using these parameters, which is the target variable
- The workflow 
![Workflow](https://github.com/swethasubu93/Analytical-Processing/assets/109064336/8259509f-e1b1-44a9-872d-20b29dd560aa)
- *Data Preprocessing & Integration*:
    - Unneccesary columns dropped
    - column names changed for uniformity
    - datasets are integrated
    - uniform naming convention maintained
    - maintained uniform unit of measure
    - dataset is pivoted
    - handled misisng values by interpolation & median techniques
    - correlation analysis and PCA.
- *Model Development*:
  - Models trained - SVM, Decision Tree, XGBoost, Artificial Neural Network
  - The model input were of three types - features after 1) PCA , 2) correlation analysis and 3) all parameters.


## Results 

- It is seen that the models with all 14 parameters as input have outperformed the other two types.  
- The XGBoost model gave the best performance at 94% validation accuracy and 78% testing accuracy for model with all 14 parameters as input.
- Decision Tree is the second best at 60% testing accuracy (for all 14 parameters as input).

## 🔗 Contributors & Credits
Supreetha Naik https://github.com/supreetn

Sushmita Joshi https://github.com/sushmita3105

Madhura Pandit https://github.com/madhurapandit

Swetha Subramanian https://github.com/swethasubu93
