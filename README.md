# Predicting Bulldozer Sale Prices

This project leverages machine learning techniques to predict the sale prices of bulldozers using historical auction data. The primary goal is to develop a model that minimizes the Root Mean Squared Logarithmic Error (RMSLE) between predicted and actual prices.

## Project Structure

### 1. Problem Definition
> How well can we predict the future sale price of a bulldozer given its characteristics and historical sales data?

### 2. Dataset
The dataset is sourced from the Kaggle competition "Bluebook for Bulldozers." It consists of three main files:
- **Train.csv**: Data up to 2011 for training the model.
- **Valid.csv**: Data from January 2012 to April 2012, used for validation.
- **Test.csv**: Data from May 2012 to November 2012, used for final evaluation (not available during training).

### 3. Evaluation Metric
The evaluation metric for this project is **Root Mean Squared Logarithmic Error (RMSLE)**. The goal is to minimize this metric to improve model performance.

For more details on evaluation, refer to [Kaggle Bluebook for Bulldozers Evaluation](https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation).

### 4. Features
A detailed feature dictionary is available [here](https://docs.google.com/spreadsheets/d/18ly-bLR8sbDJLITkWG7ozKm8l3RyieQ2Fpgix-beSYI/edit?usp=sharing).

## Steps to Reproduce

### Prerequisites
Ensure you have the following installed:
- Python (3.8 or above)
- Jupyter Notebook
- Required libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `yaml`, `bokeh`

### Repository Structure
The repository contains:
- **Notebook File**: `Bulldozer_Sales_Price_Pred_Project.ipynb`
- **Configuration File**: `config.yaml`

### Setup
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Add the dataset files to the project directory as specified in `config.yaml`.

### Running the Project
1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Bulldozer_Sales_Price_Pred_Project.ipynb
   ```
2. Execute the cells sequentially to:
   - Load and explore the dataset.
   - Perform feature engineering and preprocessing.
   - Train and evaluate machine learning models.

## Key Components

### Data Loading
The datasets are read using paths specified in `config.yaml`. This ensures modularity and easy updates to dataset paths.

### Feature Engineering
Data is cleaned and preprocessed to handle missing values, encode categorical variables, and derive new features where applicable.

### Model Training
Machine learning models are trained to predict bulldozer prices. Techniques like cross-validation and hyperparameter tuning are employed to optimize performance.

### Model Evaluation
The performance of the models is evaluated using the RMSLE metric on the validation dataset.

## References
- [Bluebook for Bulldozers on Kaggle](https://www.kaggle.com/c/bluebook-for-bulldozers)
- [Evaluation Metric Explanation](https://www.kaggle.com/c/bluebook-for-bulldozers/overview/evaluation)


---

This project demonstrates a practical approach to solving regression problems with real-world datasets. Feel free to adapt and extend it for other use cases!

