# Optimal Vehicle Recommendation Engine

## Overview

The Optimal Vehicle Recommendation Engine is a data-driven car recommendation system designed to help customers find vehicles that align with their preferences and needs. By analyzing vehicle attributes, user reviews, and leveraging machine learning models, the tool offers personalized vehicle recommendations across different customer profiles.

## Project Goals

The tool aims to:
- Build vehicle profiles based on customer preferences and needs.
- Use machine learning to classify vehicles into groups representing diverse customer profiles.
- Offer customers curated recommendations based on their unique profile and vehicle attributes.

## Project Process

The project is divided into four main phases:

1. **Organize**: Planning the project structure and defining key milestones.
2. **Collect**: Gathering vehicle data, including attributes and reviews, primarily from TrueCar.
3. **Analyze**: Conducting data analysis to find patterns and trends.
4. **Formulate**: Developing customer profiles and generating recommendations.

## Tools and Technologies

This project used a range of tools and technologies:

- **Data Collection and Processing**: Excel, Oracle SQL
- **Data Analysis and Machine Learning**: Python (Sentiment Analysis, Data Processing), Orange3 (Clustering)
- **Data Visualization and Profiling**: Orange3

## Data Summary

The dataset comprises 13 attributes across over 250 vehicle models from 20+ brands, sourced from TrueCar. Key vehicle attributes include:

- Numerical: MSRP, MPG (City and Highway), Engine Size, etc.
- Categorical: Vehicle Type, Drive Type, Brand, etc.

## Methodology

1. **Data Pre-Processing**:
   - Conducted feature selection to remove highly correlated variables (e.g., city and highway MPG, MSRP and Starting Market Average).
   - Applied Principal Component Analysis (PCA) to reduce dimensions, capturing 23% of the variance with two components.

2. **Clustering**:
   - Employed K-Means Clustering to segment data into four clusters based on the main components.
   - Evaluated clusters using Silhouette Score (0.441), determining an optimal number of four clusters to represent customer segments.

3. **Customer Profile Formulation**:
   Defined profiles for recommendation based on cluster results:
   - **Luxury Enthusiast**: Prefers premium vehicles with advanced features, e.g., BMW M3, Porsche Cayenne.
   - **Economical Commuter**: Seeks fuel efficiency and affordability, e.g., Kia K5, Honda Civic.
   - **Dynamic Driver**: Prioritizes performance and versatility, e.g., Toyota Tundra, Mazda CX9.
   - **High-End Motorist**: Looks for a blend of luxury and performance, e.g., Volvo S60, Audi S3.

## Future Enhancements

- Expand the dataset to include more vehicle brands, models, and attributes.
- Incorporate customer reviews and a feedback questionnaire to improve recommendations.
- Integrate financial information for monthly payment projections and financing options.
- Develop a web application interface that tailors recommendations based on demographics and preferences.

## Conclusion

The Optimal Vehicle Selection Tool utilizes machine learning clustering to deliver customer-centric vehicle recommendations. The project successfully grouped vehicles into meaningful clusters and identified attributes that align with different customer profiles. Future improvements aim to further personalize the recommendations and enhance the tool's usability.
