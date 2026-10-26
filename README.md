# AIT620 Final Project — Call Center Duration Prediction

## Project Overview
This project applies machine learning techniques to estimate call center conversation duration using transcript-derived features.

The project was developed as part of the AIT620 Artificial Intelligence course at the University of the Potomac.

## Dataset
**Source:** [AIxBlock — 92k Real World Call Center Scripts (English)](https://huggingface.co/datasets/AIxBlock/92k-real-world-call-center-scripts-english)

The analysis uses 3,239 JSON records, with 3,167 records retained after data cleaning.

**License notice:** The dataset is provided for research and AI model development. Commercial use, resale, and redistribution are prohibited. The original dataset is not included in this repository.

## Machine Learning Models
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

## Results

| Model | MAE (seconds) | RMSE (seconds) | R² |
|---|---:|---:|---:|
| Linear Regression | 79.30 | 118.97 | 0.9296 |
| Gradient Boosting | 80.09 | 122.76 | 0.9250 |
| Random Forest | 83.24 | 148.89 | 0.8897 |

Linear Regression achieved the best performance on the test dataset.

## How to Run

1. Download the original dataset from the Hugging Face source, subject to its license.
2. Extract the JSON files into a local folder named `data` in the project directory.
3. Install the required Python libraries:

   `pip install jupyter pandas numpy scikit-learn matplotlib seaborn`

4. Open `AIT620_Final_CallCenterEN.ipynb` in Jupyter Notebook.
5. Run all cells.

## Limitations
The model uses features derived from completed call transcripts. Therefore, its results should not be interpreted as a real-time prediction of call duration before a call begins.

## Author
Zolzaya Arild

AIT620 — Artificial Intelligence

University of the Potomac
