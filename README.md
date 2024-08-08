# Machine-Learning-Stock-Prediction

This project aims to predict the next day's S&P 500 stock price movement (up or down) using machine learning techniques. The project leverages historical stock data and employs a Random Forest classifier to make predictions. Additionally, it explores the use of various technical indicators to enhance the model's accuracy.

## Author
Zhihang Cheng

## Technologies Used

- **Python**: The main programming language used for data manipulation, model training, and evaluation.
- **Jupyter Notebook**: An interactive environment for running and documenting the code.
- **pandas**: Used for data manipulation and analysis.
- **yfinance**: A library to fetch historical market data from Yahoo Finance.
- **scikit-learn**: A machine learning library used for model training and evaluation, including Random Forest classifier and precision score metric.
- **matplotlib**: Used for plotting and visualizing data and results.

## Project Workflow

### 1. Data Collection

The historical S&P 500 data is fetched using the `yfinance` library.

### 2. Data Preparation

The data is cleaned and prepared by removing unnecessary columns and creating target variables to indicate if the next day's closing price is higher than today's.

### 3. Initial Model Training

A Random Forest classifier is initially trained and tested on the prepared data. This model serves as a baseline for comparison.

### 4. Model Backtesting

A backtesting function is used to validate the model over different time periods, ensuring that it generalizes well on unseen data.

### 5. Adding New Predictors

New predictors based on various moving averages and trends are added to the model to enhance its performance. These technical indicators aim to capture more complex patterns in the stock data.

### 6. Model Evaluation

The model's performance is evaluated using precision as the metric. The precision score indicates the proportion of true positive predictions among all positive predictions.

## Results

- **Baseline Precision**: The initial model achieved a precision of approximately 53.51%.
- **Enhanced Model Precision**: With the addition of new predictors, the Random Forest model achieved a precision of approximately 57.52%, indicating a significant improvement over the baseline model.

## Conclusion

By incorporating additional technical indicators and refining the model, we successfully improved the precision of stock movement predictions. The results demonstrate the effectiveness of using machine learning techniques and feature engineering in financial market prediction.

## How to Run

1. **Install the necessary Python packages**:
   ```bash
   pip install yfinance pandas scikit-learn matplotlib
2. **Run the Jupyter Notebook to execute the code step-by-step**



## Future Improvements

1. **Incorporate Data from Other Exchanges**:
   - Consider integrating data from stock exchanges in other countries to enhance the model's robustness and predictive power. This could provide a more global perspective on market movements.

2. **Key Stocks and Sectors Analysis**:
   - Analyze key stocks and sectors within the S&P 500 to identify specific drivers of index movements. This can help in understanding the influence of major companies and industry trends on the overall market.

3. **Incorporate Financial News**:
   - Use sentiment analysis on financial news and reports to include external factors that might affect stock prices. This can add another layer of information that purely historical price data cannot provide.

4. **Hourly Predictions**:
   - Shift from daily-based predictions to hour-based predictions to capture more granular market movements. This would require high-frequency data and could potentially provide more timely and actionable insights.

By implementing these improvements, the model can become more comprehensive and accurate, potentially leading to better investment strategies and decision-making.