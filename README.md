# SIH 2024

| **Problem Statement ID** | **Problem Statement Title**                                                                                                                                                   |
|--------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1647                     | Development of AI-ML based models for predicting prices of agri-horticultural commodities such as pulses and vegetables (onion, potato, onion)                                 |

| **Description**                                                                                                                                                                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| The Department of Consumer Affairs monitors the daily prices of 22 essential food commodities through 550 price reporting centres across the country. The Department also maintains buffer stock of pulses, viz., gram, tur, urad, moon and masur, and onion for strategic market interventions to stabilize the volatility in prices. Decisions for market interventions such as release of stocks from the buffer are taken on the basis of the price trends and outlook. At present, the analyses of prices are based on the seasonality, historical and emerging trends, market intelligence inputs, crop sowing and production estimates. ARIMA based economic models have also been used to examine and forecast prices of pulses. |

| **Organization**                                            | **Department**                        | **Category** | **Theme**                               |
|-------------------------------------------------------------|---------------------------------------|--------------|-----------------------------------------|
| Ministry of Consumer Affairs, Food and Public Distribution  | Department of Consumer Affairs        | Software     | Agriculture, FoodTech & Rural Development |


# My Solution

### Steps:
1. **Data Acquisition**:
   - You collected the dataset from the Department of Consumer Affairs website ([consumeraffairs.nic.in](https://consumeraffairs.nic.in/)). The dataset includes daily prices of essential food commodities such as pulses (gram, tur, urad, moong, masur) and vegetables (onion, potato).
   
2. **Data Preprocessing**:
   - **Cleaning**: Handled missing or inconsistent values in the dataset.
   - **Feature Engineering**: Added useful features like seasonality, historical trends, crop production estimates, and market intelligence inputs.
   - **Normalization**: Standardized the data for better performance in machine learning models.

3. **Model Selection**:
   - You leveraged **ARIMA** (AutoRegressive Integrated Moving Average) to model time-series data for price prediction based on historical trends.
   - Additionally, you implemented **AI-ML models** such as:
     - **Random Forest** and **XGBoost** for short-term price predictions.
     - **LSTM (Long Short-Term Memory)** for better capturing seasonality and long-term dependencies in price trends.

4. **Training and Validation**:
   - **Split**: The dataset was divided into training and validation sets.
   - **Cross-validation** was used to ensure robustness.
   - Model performance was evaluated using metrics like **Mean Absolute Error (MAE)** and **Root Mean Square Error (RMSE)**.

5. **Buffer Stock Impact Simulation**:
   - Using the trained models, you simulated the effect of releasing buffer stock from the Department's reserves to stabilize prices.
   - Incorporated market intervention scenarios into the prediction model to evaluate policy decisions.

6. **Visualization**:
   - Deployed visualizations to show predicted price trends, seasonal effects, and impacts of market interventions.

7. **Deployment**:
   - The models were designed for integration into a real-time monitoring system to predict future price trends and assist the Department in making informed decisions about market interventions.
