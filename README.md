# NYU Tandon Spring 2023 Data Science Bootcamp

## Project: Real-world data science project simulation

### Dataset: Bike Sharing Dataset

#### Objective:

Gain hands-on experience in data collection, feature engineering, modeling, visualization, and reporting.

#### Dataset Details:

- Hourly and daily count of rental bikes between 2011 and 2012 in Capital bikeshare system.
- Contains weather and seasonal information.

#### Project Requirements:

- Study the data and come up with possible problem statements.
- Test different models and kinds of analysis (e.g., regression, classification).
- Formulate questions to be tested with hypothesis testing.
- Support findings with appropriate visualizations and result summaries.

#### Key Dates:

Confirm presentation date (TBD) and individual participation by TBD.

#### Contact Information:

Email: datasciencebootcamp@nyu.edu
Reach out to instructors on Slack or email for questions.

#### Addressed Problem Statements:

- Predict the daily demand for bike rentals using weather and seasonal information.
- Identify factors such as weekdays, season, temperature, humidity, and wind speed that significantly affect the daily demand for bike rentals and quantify their impact.
- Determine if certain days of the week or seasons have consistently higher or lower bike rental demand, and identify possible reasons for these patterns.
- Analyze the impact of weather conditions, such as temperature, humidity, and wind speed, on daily bike rental demand. 

#### Insights and Patterns:

Sure! Here's a summary of the insights and patterns from the different analyses conducted:

##### Exploratory Data Analysis (EDA)

- Bike rentals steadily increased from January to June, peaked in July, and then gradually decreased through December.
- Bike rentals were highest on weekdays and lowest on weekends.
- Bike rentals peaked during the hours of 12 pm and 6 pm.

##### Random Forest Model

- The Random Forest model was able to accurately predict bike rental counts with an R-squared value of 0.85.
- Features such as temperature, humidity, and hour of the day had the most significant impact on the bike rental count.
- The Random Forest model indicated that temperature was the most important feature in predicting bike rentals.

##### Time Series Analysis

- The ADF test indicated that the time series data was stationary and suitable for time series analysis.
- The ACF and PACF plots indicated that an ARIMA model with a seasonal component was suitable for the time series data.
- The ARIMA model was able to accurately predict the bike rental count for the test data set with a mean squared error of 4373847.32.
- The 20-day moving average of the actual data showed a steady increase in bike rentals from January to June, peaking in July, and then a gradual decrease through December.

##### Comparing Random Forest and Time Series Models

- Both the Random Forest and ARIMA models were able to accurately predict the bike rental count for the test data set.
- The Random Forest model was able to capture more of the short-term fluctuations in the bike rental count, while the ARIMA model was better at capturing the overall trend of increasing bike rentals during the summer months.

Overall, the analyses showed that both the Random Forest and ARIMA models were able to accurately predict bike rentals, with each model having its own strengths in capturing different aspects of the data. Additionally, the EDA revealed some key patterns in bike rental behavior, such as higher rentals during weekdays and peak rentals during midday hours.


#### Steps for Regression and Classification Approach:

##### Data Exploration and Preparation:

- Load and explore the dataset to understand its structure, features, and any missing values.
- Perform data cleaning, handling missing values, and any necessary transformations.

##### Feature Engineering:

- Create new features or modify existing ones, if needed, to improve the predictive power of the model.
- Determine the relevant features for your regression or classification problem using techniques like correlation analysis or feature selection methods.

##### Data Splitting:

- Split the dataset into training and testing sets, typically using a 70:30 or 80:20 ratio.

##### Regression Problem:

- Train various regression models (e.g., linear regression, decision tree, random forest, gradient boosting) on the training data.
- Evaluate each model's performance on the testing data using appropriate metrics, such as Mean Absolute Error (MAE), Mean Squared Error (MSE), or R-squared.
- Fine-tune the best-performing model using hyperparameter tuning techniques, such as grid search or random search.

##### Classification Problem:

- Define thresholds for low, medium, and high demand categories based on the distribution of bike rentals.
- Train various classification models (e.g., logistic regression, decision tree, random forest, gradient boosting) on the training data.
- Evaluate each model's performance on the testing data using appropriate metrics, such as accuracy, precision, recall, or F1-score.
- Fine-tune the best-performing model.

##### Visualizations and Result Summaries:
- Create visualizations to help convey the patterns, relationships, and insights discovered during the analysis.
- Summarize the findings in a clear, concise manner, highlighting the key insights and their implications for bike-sharing systems.
- Reporting and Presentation:
- Compile the findings, visualizations, and result summaries into a coherent report or presentation.
