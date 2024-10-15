
# Breast Cancer Patient Status Prediction

This project is focused on predicting the status of breast cancer patients based on various clinical and biological features using machine learning.

## Dataset

The dataset used for this project is `BRCA.csv`, containing various details such as age, gender, protein levels, tumor stage, histology, and status of estrogen receptors, progesterone receptors, and HER2.

## Features

The key features used in the model are:
- Age
- Gender
- Protein1, Protein2, Protein3, Protein4
- Tumor Stage
- Histology
- ER Status (Estrogen Receptor)
- PR Status (Progesterone Receptor)
- HER2 Status
- Type of Surgery

The target variable is:
- Patient Status (whether the patient has recovered or not)

## Steps

1. **Data Preprocessing**: 
   - Null values are removed.
   - Categorical variables are mapped to numerical values.
   
2. **Exploratory Data Analysis (EDA)**: 
   - Visualizations are created to show the distribution of tumor stages, histology, and types of surgeries using pie charts.

3. **Modeling**:
   - A Support Vector Machine (SVM) classifier is used to predict the patient status.
   - The dataset is split into training and test sets (90% training, 10% testing).
   
4. **Prediction**:
   - A sample prediction is made using a set of patient features.

## How to Run

1. Clone the repository or download the code.
2. Install the required libraries:
   ```bash
   pip install pandas numpy scikit-learn plotly
   ```
3. Place the dataset `BRCA.csv` in the same directory as the code.
4. Run the code to preprocess the data, visualize it, and train the model.
5. Use the sample `features` array for testing the prediction.

## Results

The model can predict the status of patients based on the provided clinical features. Example prediction:
- `features = [[36.0, 1, 0.080353, 0.42638, 0.54715, 0.273680, 3, 1, 1, 1, 2, 2]]`
  - Prediction: `[1]` (patient status)

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- plotly

## License

This project is licensed under the MIT License.
