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

### Data Splitting:

- Split the dataset into training and testing sets, typically using a 70:30 or 80:20 ratio.

### Regression Problem:

- Train various regression models (e.g., linear regression, decision tree, random forest, gradient boosting) on the training data.
- Evaluate each model's performance on the testing data using appropriate metrics, such as Mean Absolute Error (MAE), Mean Squared Error (MSE), or R-squared.
- Fine-tune the best-performing model using hyperparameter tuning techniques, such as grid search or random search.

### Classification Problem:

- Define thresholds for low, medium, and high demand categories based on the distribution of bike rentals.
- Train various classification models (e.g., logistic regression, decision tree, random forest, gradient boosting) on the training data.
- Evaluate each model's performance on the testing data using appropriate metrics, such as accuracy, precision, recall, or F1-score.
- Fine-tune the best-performing model.

### Visualizations and Result Summaries:

- Create visualizations to help convey the patterns, relationships, and insights discovered during the analysis.
- Summarize the findings in a clear, concise manner, highlighting the key insights and their implications for bike-sharing systems.

### Reporting and Presentation:

- Compile the findings, visualizations, and result summaries into a coherent report or presentation.
- Communicate the findings to stakeholders in a clear and concise manner, highlighting the most important insights and recommendations for bike-sharing systems.
- Solicit feedback from stakeholders and use it to improve future analyses and projects.

### Future Work:

- Explore the use of more advanced modeling techniques, such as deep learning or Bayesian methods, to improve the accuracy and robustness of the models.
- Collect more data, such as demographic or location-based information, to provide more context and insights into the bike-sharing system.
- Investigate the impact of external factors, such as events or holidays, on bike rental demand and incorporate them into the models.
- Develop a real-time prediction system that can adjust to changing conditions and provide timely recommendations for bike-sharing system operators.

# Glossary of Statistics Terms with Context

- **Random Forest**: A machine learning model that uses multiple decision trees to make predictions by averaging their individual predictions. It is known for its accuracy, robustness, and ability to handle complex data. In this project, the Random Forest model is used to predict the daily demand for bike rentals using weather and seasonal information.

- **Time Series Analysis**: The study of data points collected at regular intervals over time to understand underlying trends, seasonality, and other patterns. In this project, time series analysis is used to analyze the daily bike rental demand and identify patterns in the data.

- **ARIMA (AutoRegressive Integrated Moving Average)**: A linear time series model that combines autoregressive (AR), differencing (I), and moving average (MA) components to predict future values based on past observations. In this project, the ARIMA model is used to forecast the daily demand for bike rentals using historical data.

- **Autocorrelation**: A measure of how a series is correlated with its own past values. It shows the strength and direction of the relationship between the current observation and its previous observations. In this project, autocorrelation is used to determine the appropriate order for the AR and MA components in the ARIMA model.

- **Partial Autocorrelation**: A measure of the correlation between an observation and its previous observations, after accounting for the effects of all intervening observations. It helps identify the direct relationship between observations, excluding the influence of other intervening observations. In this project, partial autocorrelation is used to determine the appropriate order for the AR component in the ARIMA model.

- **Mean Squared Error (MSE)**: A measure of the average squared difference between the actual values and the predicted values. It is commonly used to evaluate the performance of regression models. In this project, MSE is used to evaluate the performance of the ARIMA model in predicting bike rental demand.

- **Augmented Dickey-Fuller (ADF) Test**: A statistical test used to determine whether a time series is stationary or not. Stationarity is a key assumption for many time series models, including ARIMA. In this project, the ADF test is used to check the stationarity of the daily bike rental demand data.

- **Autoregressive (AR) Component**: A part of the ARIMA model that uses the past values of the time series to predict the future values. In this project, the AR component is used to model the relationship between the current bike rental demand and its past values.

- **Differencing (I) Component**: A part of the ARIMA model that involves subtracting the previous value from the current value to make the time series stationary. In this project, differencing is used to make the daily bike rental demand data stationary, which is a requirement for the ARIMA model.

- **Moving Average (MA) Component**: A part of the ARIMA model that uses the past error terms to predict the future values. In this project, the MA component is used to model the relationship between the current bike rental demand and the past error terms.

- **ACF (Autocorrelation Function) Plot**: A plot that shows the autocorrelation coefficients for different lags. It helps identify the appropriate order for the AR and MA components in an ARIMA model. In this project, the ACF plot is used to determine the optimal order for the ARIMA model.

- **PACF (Partial Autocorrelation Function) Plot**: A plot that shows the partial autocorrelation coefficients for different lags. It helps identify the appropriate order for the AR component in an ARIMA model. In this project, the PACF plot is used to determine the optimal order for the AR component

