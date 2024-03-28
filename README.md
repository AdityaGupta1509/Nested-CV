# Grouped Time Series Cross-Validation with Machine Learning Models

This repository contains code for performing grouped time series cross-validation and building predictive models using machine learning techniques. The provided Python script demonstrates how to implement a custom cross-validation method for grouped time series data and train different models for forecasting.

## Usage Instructions:

1. **Installation:**
   - Ensure you have Python installed on your system.
   - Install the necessary dependencies using pip:
     ```
     pip install numpy pandas scikit-learn xgboost
     ```

2. **Clone the Repository:**
   - Clone this repository to your local machine:
     ```
     git clone https://github.com/AdityaGupta1509/Nested-CV.git
     ```

3. **Run the Code:**
   - Navigate to the directory containing the downloaded files.
   - Execute the Python script:
     ```
     python model.ipynb
     ```

4. **Understanding the Code:**
   - The script defines a custom cross-validator class `GroupedTimeSeriesSplit` for performing grouped time series cross-validation.
   - It provides functionalities to split the data into training and testing sets while maintaining the temporal order and grouping by a specified column.
   - Sample data from a CSV file (`train.csv`) is loaded into a Pandas DataFrame.
   - Problematic values in the 'capacity' column are identified and replaced with appropriate values.
   - NaN values are handled by replacing them with the median of the respective columns.
   - Machine learning models such as Random Forest and Decision Tree are trained and evaluated using the custom cross-validation method.
   - Evaluation metrics such as Mean Squared Error (MSE) are computed for each model.

5. **Output:**
   - The script outputs the Mean Squared Error (MSE) for each model evaluated using grouped time series cross-validation.

## File Structure:

- `model.ipynb`: The main Python script containing the implementation of grouped time series cross-validation and model training.
- `train.csv`: Sample dataset used for training and evaluation.
- `README.md`: This README file providing instructions and information about the code.

## Additional Notes:

- Feel free to modify the script according to your specific dataset and requirements.
- Experiment with different machine learning models and hyperparameters to improve forecasting accuracy.
- For any issues or questions, please open an issue on the GitHub repository.

## Author:
Aditya Gupta
adityagupta.5391@gmail.com
