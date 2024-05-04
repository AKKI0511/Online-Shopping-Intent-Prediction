# Online Shopping Intent Predictor

This Python project implements an online shopping intent predictor using a k-nearest neighbor classifier (k=1) to predict whether a visitor will generate revenue (make a purchase) based on various features related to their browsing behavior. The project uses the scikit-learn library for machine learning tasks.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/AKKI0511/Online-Shopping-Intent-Prediction.git
   cd Online-Shopping-Intent-Prediction
   ```

2. Run the predictor:

   ```bash
   python shopping.py shopping.csv
   ```

   Replace `shopping.csv` with the path to your CSV data file containing the shopping behavior data.

## Features

The predictor uses the following features to make predictions:
- Administrative
- Administrative Duration
- Informational
- Informational Duration
- Product Related
- Product Related Duration
- Bounce Rates
- Exit Rates
- Page Values
- Special Day
- Month (indexed from 0 to 11 for January to December)
- Operating Systems
- Browser
- Region
- Traffic Type
- Visitor Type (0 for not returning, 1 for returning)
- Weekend (0 if false, 1 if true)

## Data Format

The data should be provided in a CSV format with columns representing the features mentioned above, along with a column indicating whether revenue was generated (1 for true, 0 for false).

## Training and Evaluation

The data is split into training and test sets using a test size of 40%. The k-nearest neighbor classifier is trained on the training set, and predictions are made on the test set. The sensitivity (true positive rate) and specificity (true negative rate) of the model are then calculated to evaluate its performance.

## Dependencies

- scikit-learn (for machine learning tasks)
- pandas (for data manipulation)

Install dependencies using:

```bash
pip install scikit-learn pandas
```

## Output

The predictor prints the following results:
- Number of correct predictions
- Number of incorrect predictions
- True Positive Rate (Sensitivity)
- True Negative Rate (Specificity)

- Example:

![image](https://github.com/AKKI0511/Online-Shopping-Intent-Prediction/assets/120317569/009811ca-8132-4f6c-851c-8255aeb30d95)


## Acknowledgements

This project utilizes scikit-learn's k-nearest neighbor classifier for predictive modeling and showcases how to evaluate a machine learning model's performance in a binary classification task.

