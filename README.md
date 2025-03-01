# AZN_OIL_Relationship_Predictor

## Overview
The **AZN_OIL_Relationship_Predictor** is a machine learning model designed to analyze and predict the relationship between Brent crude oil prices and the Azerbaijani Manat (AZN) exchange rate. Given the significant impact of oil prices on Azerbaijan's economy, this model aims to provide insights into potential currency fluctuations based on historical data trends.

## Features
- **Data-Driven Insights**: Analyzes historical oil prices and exchange rate data.
- **Predictive Modeling**: Uses machine learning algorithms to forecast AZN/USD exchange rate movements.
- **Visualization Tools**: Generates graphs comparing actual and predicted values.
- **Customizable Parameters**: Allows fine-tuning for different datasets and models.

## Installation
To use this predictor, first clone the repository and install the required dependencies:

```sh
git clone https://github.com/alimovabdulla/AZN_OIL_Relationship_Predictor.git
cd AZN_OIL_Relationship_Predictor
pip install -r requirements.txt
```

## Usage
### 1. Data Preparation
Ensure your dataset includes historical oil prices and AZN/USD exchange rates. The expected format:

| Date       | Oil Price (USD) | AZN/USD Exchange Rate |
|------------|---------------|-----------------------|
| 2025-02-28 | 74.89         | 1.7000               |
| 2025-02-27 | 74.50         | 1.7000               |

### 2. Running the Model
Execute the script to train the model and make predictions:

```sh
python predictor.py
```

### 3. Visualizing Results
The script will generate a scatter plot comparing actual vs. predicted values:

```python
import matplotlib.pyplot as plt
plt.scatter(y_test, preds, s=20, marker='x')
plt.plot([min(y_test), max(y_test)], [min(y_test), max(y_test)], color='red', linestyle='--')
plt.xlabel("Actual Values")
plt.ylabel("Predicted Values")
plt.show()
```

## Use Cases
- **Economic Forecasting**: Helps policymakers predict currency fluctuations.
- **Investment Strategy**: Assists traders in making informed financial decisions.
- **Risk Management**: Supports businesses in hedging against currency risks related to oil price changes.

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests to enhance the model.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries, please contact [your email or GitHub profile].

