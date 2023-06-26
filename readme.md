# Fuel Price Analysis and Prediction

This repository contains the code and datasets for analyzing and predicting fuel prices, specifically Brent Oil, Crude Oil, Natural Gas, and Heating Oil. The project focuses on creating models to predict the closing prices of these fuels based on their opening, highest, and lowest prices.

## Dataset

The dataset used for analysis and prediction is stored in the `./datasets/` directory. The original dataset is divided into four separate files, each containing the prices for a specific fuel type: Brent Oil, Crude Oil, Natural Gas, and Heating Oil. Additionally, a modified dataset is available, which combines the prices of all the fuels into a single file for comparative analysis.

### Dataset Structure

The original dataset files are structured as follows:

```
Symbol,Date,Open,High,Low,Close,Volume,Currency
Brent Oil,2000-01-04,23.9,24.7,23.89,24.39,32509,USD
Brent Oil,2000-01-05,24.25,24.37,23.7,23.73,30310,USD
```

The modified dataset file combines the prices of all fuels into a single file, organized by date:

```
Date,OpenBrent,HighBrent,LowBrent,CloseBrent,VolumeBrent,OpenCrude,HighCrude,LowCrude,CloseCrude,VolumeCrude,OpenHeating,HighHeating,LowHeating,CloseHeating,VolumeHeating,OpenNatural,HighNatural,LowNatural,CloseNatural,VolumeNatural
2000-01-04,23.9,24.7,23.89,24.39,32509,25.2,25.69,24.71,25.55,74788,0.672,0.683,0.654,0.6778,25311,2.13,2.2,2.13,2.176,30152
2000-01-05,24.25,24.37,23.7,23.73,30310,25.5,25.61,24.87,24.91,70944,0.679,0.679,0.665,0.6655,18691,2.18,2.2,2.125,2.168,27946
```

## Notebooks

The `notebooks` directory contains Jupyter notebooks used for data analysis and model training. These notebooks provide a step-by-step guide on how the analysis was performed and the models were trained.

### Notebook Descriptions

1. `Data_Exploration.ipynb`: This notebook explores the original dataset, performing various data analysis techniques such as statistical analysis, visualization, and correlation analysis. It provides insights into the individual fuel prices and their relationships.

2. `Model_Training_Brent_Oil.ipynb`: This notebook focuses on training a predictive model for Brent Oil prices using the opening, highest, and lowest prices of Brent Oil as input features. It includes data preprocessing, model selection, training, and evaluation.

3. `Model_Training_Crude_Oil.ipynb`: This notebook trains a predictive model for Crude Oil prices using the opening, highest, and lowest prices of Crude Oil. It follows a similar approach to the Brent Oil model.

4. `Model_Training_Natural_Gas.ipynb`: This notebook trains a predictive model for Natural Gas prices using the opening, highest, and lowest prices of Natural Gas. It follows a similar approach to the Brent Oil and Crude Oil models.

5. `Model_Training_Heating_Oil.ipynb`: This notebook trains a predictive model for Heating Oil prices using the opening, highest, and lowest prices of Heating Oil. It follows a similar approach to the other fuel models.

6. `Price_Comparison.ipynb`: This notebook compares the prices of Brent Oil, Crude Oil, Natural Gas, and Heating Oil in a parallel manner. It analyzes the correlation between the prices and identifies any trends or patterns.

## Models

Trained models for predicting the average Brent Oil and Heating Oil prices based on the Crude Oil prices are stored in the `models` directory. These models leverage the opening, closing, highest, and lowest prices of Crude Oil to make predictions.

## Usage

To use this repository, follow the steps below:

1. Clone the repository to your local machine.
2. Navigate to the `datasets` directory to access the original and modified datasets.
3. Explore the `notebooks` directory to understand the data analysis and model training process.
4. If desired, run the notebooks in a Jupyter environment to reproduce the analysis and train the models.
5. The trained models are available in the `models` directory. You can load these models and use them for predicting the average Brent Oil and Heating Oil prices based on Crude Oil prices.

Please note that this project assumes basic knowledge of data analysis and machine learning techniques. It is recommended to have a Python environment with necessary dependencies installed.

## License

The code and datasets in this repository are provided under the [MIT License](LICENSE). You are free to use, modify, and distribute the code and datasets for personal and commercial purposes.

## Acknowledgments

If you use this project or find it helpful, it would be appreciated if you could acknowledge it by citing this repository or providing a link to it. Additionally, any contributions or improvements to the project are welcome through pull requests.
