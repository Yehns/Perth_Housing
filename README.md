# Perth_Housing
DAY 1: Mon 22 May 2023
Topic: Predicting Perth house prices based on housing data
Team: Jens Weiman, Paul Roberts, Dale Hancke

DAY 2: Tues 23 May 2023
Analysis of data sources
Look for problem statements and possible solutions
Decide on tools
Create deck

DAY 3: Thurs 25 May 2023
Analytics

DAY 4: Mon 29 May 2023
Analytics

DAY 5: Tues 30 May 2023
Wrap-up and prep for presentation

DAY 6: Thurs 1 June 2023
Presentation

**EXAMINATION OF THE PERTH HOUSING MARKET:**

The purpose of this exercise was to pull out some interesting findings around the Perth housing market data.  The elements chosen for this exercise relate to visualisations of the data via maps, calculations which could be used for predictive analysis of the cost of housing in Perth, and some machine learning visualisation of a suburb.

The data was extracted from Kaggle: based on the Perth housing market data https://www.kaggle.com/datasets/syuzai/perth-house-prices. 
The data was good, with a few errors (NUL values 999 values for garages, which were replaced with zero's and NaN for build year being tweaked to address the issue). As these anomalies were very small, they had very little impact to the data.

  Technologies used: Python, Pandas, Tableau, Sklearn

**TRAINING A MODEL TO PREDICT THE COST OF HOUSES IN PERTH**

Here the data was imported into a DataFrame (DF) and using looping, a new DF with relevant data per suburb was established. Using scaling, and running the data to test and train the model, linear regression outputs were established. This helped generate the inputs for a DataFrame with an "r2" score in it, highlighting predicted housing prices. This model could be used by Estate Agents and prospective house-buyers going forward.

Version 3 of the model improves on the earlier models by breaking each suburb down into groups based on the land area for the property. This greatly improved the accuracy of the predictions. Further improvements will be needed to identify and handle outlying properties (ones that don't fit in with the rest of the suburb).

**MAPPING OF DATA WITH KEY INFORMATION**

The following Tableau Dashboards provide a visual representation of the data collected. Focused mainly on median house prices, but includes measures such as variance and STD of house prices in Perth. The data provdes an analysis based primarily price, and accessibility to Perth CBD.

**USING MACHINE LEARNING PER SUBURB**

Here the suburb with the most amount of data was chosen – Bertram. This data was set up as a DataFrame then reduced to incorporate some key elements in deciding on a house: price, room numbers (bathrooms, garages), size (land and house square-meterage). Using the K-method, the outcome showed that using 3 clusters would make sense if doing further analysis.

![image](https://github.com/Yehns/Perth_Housing/assets/118644844/25c04a3a-6e4e-416d-9a87-e4c3b03d2504)

![image](https://github.com/Yehns/Perth_Housing/assets/118644844/b97f780a-2c9e-4494-8388-2a8776998938)


