# Phase_4_Group_2_Project

# Chicago Car Crash Data

##  Predicting the Primary Contributory Cause 

## By: Cindy, Stephen & Vincent (Group 2)

There have been accidents occuring in Chicago. These accidents have resulted in severe injuries, damaged properties and even, loss of life. This has led to an increased outcry on a need for action to be taken. This has prompted the establishment of a `Road and Safety Committee`. This committee would like to known what are the main contributors of accidents in the area.


This project uses publicly available data from the City of Chicago to build a predictive model that determines the primary contributory cause of traffic accidents. Leveraging data from three datasets (Crashes, People, Vehicles), the model applies feature engineering and interpretable machine learning techniques to both predict and explain accident causes.

## Data Source

The source for the datasets came from the City of Chicago Website. There were three datasets that we observed, "Traffic Crashes - Crashes", "Traffic Crashes - Vehicle", and "Traffic Crashes - People". Then we merged them into one database. 

Column names and descriptions can be found here; 

Traffic Crashes - Crashes: https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if

Traffic Crashes - Vehicle: https://data.cityofchicago.org/Transportation/Traffic-Crashes-Vehicles/68nd-jvt3

Traffic Crashes - People:
https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d

## Methodology 

Machine Learning Approach

We applied machine learning techniques to uncover patterns in accident data, aiming to better understand the key factors contributing to accidents.

### Model Used: XGBoost

- **Type**: Gradient Boosted Decision Trees  
- **Purpose**: Learns from historical accident data to predict likely causes  
- **Advantages**: High accuracy, strong performance, and interpretability

### Training & Testing

- **Training Data**: 70% of the dataset  
- **Testing Data**: 30% of the dataset  
- This split helps us ensure that the model performs reliably in real-world scenarios.

### Model Performance

- **Training Accuracy**: 67.11%  
- **Validation Accuracy**: 65.73%  
- The consistency between training and validation accuracy indicates good generalization to unseen data.


## Feature Importance

The XGBoost model identified the following as the most influential features contributing to accident prediction:

| Feature                   | Importance Score |
|---------------------------|------------------|
| **Driver Action**         | 131.79           |
| Secondary Cause           | 78.17            |
| Roadway Surface Condition | 46.08            |
| Physical Condition        | 36.73            |
| Unit Type                 | 32.48            |

### Interpretation

- **Driver Action** is by far the most influential factor, reinforcing the conclusion that human behavior is the leading contributor to accidents in Chicago.
- **Secondary causes** and **road conditions** also play significant roles, though to a lesser extent.
- The model’s feature importance distribution supports targeted interventions, especially those aimed at improving driver behavior and awareness.


###  Key Insight

> **Driver action** emerged as the leading cause of accidents, as identified by the model.


## Conclusion

This insight underscores the critical role human behavior plays in road safety. It opens the door for impactful interventions, such as:

- Launching public awareness and educational campaigns  
- Enforcing stricter driving laws  
- Integrating technology like driver-monitoring systems  
- Promoting safer driving habits through policy and design

By combining data-driven insights with practical initiatives, the committee can take meaningful steps to reduce accidents and enhance transportation safety.
