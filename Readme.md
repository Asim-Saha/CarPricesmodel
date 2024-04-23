Application assignment : 11.1 

**File location:**

## Project Background: 

As part of the UC Berkeley Professional Certificate in Machine Learning and Artificial Intelligence (UC Berkeley, 2022), this assignment is designed to test our new skills. We are to use the Cross Industry Standard Process for Data Mining (CRISP-DM) method (Schröer, et al, 2021) of data analysis, see Figure 1 below, on a dataset of car prices.

**CRISP-DM :**

The CRISP-DM (Cross-Industry Standard Process for Data Mining) approach to data analysis involves six major steps as outlined below:

Understanding the Business: This initial step involves conducting an in-depth analysis of the business objectives and needs. It includes assessing the current situation, defining goals based on insights, and setting up a plan to proceed.

Understanding the Data: In this phase, data is collected from various sources, its format and type are determined, and the data is profiled. Tasks include exploring the data, describing it, and ensuring its quality, accuracy, and validity.

Data Preparation: Careful selection, cleansing, construction, and formatting of the data are carried out in this step. The data is organized for modeling, and information exploration is conducted to identify patterns aligned with business insights.

Modeling: The modeling phase involves selecting modeling techniques, generating test scenarios for validation, building various models, and assessing them to ensure alignment with business objectives

Evaluation: During this phase, the results of the models are evaluated against business intentions. Multiple models are assessed to determine which one best meets the project's goals.

Deployment/Communication: The final step involves presenting the gathered information in a usable manner to stakeholders according to their expectations and business requirements. This phase may vary in complexity based on numerous factors.

**Scope of this Assignment:**

As this is the second Module that involves a practical application of the data analysis, this assignment only covers the first three sections of the CRISP-DM methodology: Understanding the Business, Understanding the Data, Data Preparation, and Modeling.

**Business Objectives :**

The business objective is to assess a database of used cars that contain their selling price and a list of features of the car. By analyzing this data, we can evaluate the price of the vehicle in comparison with the listed features of the car. Using this information, we are to build a model that can be used to evaluate other cars that we may want to sell in the used vehicle lots.

## Data Understanding: 

**Dataset**

The dataset used for this assignment was provided as part of the
assignment in a Comma Separated Values (CSV) format.

**Car attributes**

* 'id' - a unique number assigned to this car,
* 'region' - the region within a state where the vehicle is located.
* 'price' - the current selling price of the car.
* 'year' - the year the vehicle was manufactured.
* 'manufacturer' - the vehicle manufacturer.
* 'model' - the model of the car.
* 'condition' - the condition of the car.
* 'cylinders' - the number of cylinders in the engine of this car.
* 'fuel' - the type of fuel required to operate this car.
* 'odometer' - the current mileage reading on the car's odometer.
* 'title_status' - indicates if there is a clear title to this car.
* 'transmission' - the type of transmission in the car.
* 'VIN' - the vehicle id number assigned to this car.
* 'drive' - whether this is a rear drive or 4 wheel drive vehicle.
* 'size' - the size of the car.
* 'type' - the type of car.
* 'paint_color' - the color of the car.
* 'state' - the U.S. state in which this vehicle is located.

## EDA
I have build two plots to show the visual presentation

1) Made a join plot of between the price and Year

2) Created a Histoplot of the car prices range between 10000 to 50000

## Results and Key Findings
To help guide the modeling process, we derived a requirement for the model to predict within $3,000, on average, of the correct sale price. The modeling thus far did not meet this requirement. The best performance seen thus far has been $3,150, so although we failed to meet the requirement, we got pretty close. The client can use this requirement to build in sufficient margin per transaction such that they obtain profitable sales.

The modeling showed that the 3 most important features in predicting price are the vehicle's year, odometer, and what type of fuel (gas, diesel, electric, etc...). Also important, but to a lesser extent, are the vehicle's type and manufacturer. If a dealer can only obtain just a few features per vehicle, these are the ones to prioritize.

The least important feature was paint color, among those tested. Some features were left out of the modeling entirely, including the VIN, region, and sales ID, which is of course specific to each transaction.



## Next Steps and Recommendations
The next step is to go over these findings with the candidate dealers and understand the suitability of the requirement, and more importantly, the model's performance against it. It might be good enough as is, or it may need additional refinement, in terms of either the model's performance against the requirement, or the requriement itself.