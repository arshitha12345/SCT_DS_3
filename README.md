# Bank Marketing Decision Tree Classifier

## Project Description  
This project demonstrates a machine learning model built to predict whether a bank customer will subscribe to a term deposit, using demographic and behavioural data. The model is implemented using a Decision Tree Classifier trained on the Bank Marketing Dataset from the UCI Machine Learning Repository.

---

## Dataset  
- **Name:** Bank Marketing Dataset  
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)  
- **Target variable:** `y` — whether the client subscribed to a term deposit (`yes` / `no`)  
- **Features:**  
  - Demographic: age, job, marital, education  
  - Financial: balance, housing loan, personal loan  
  - Campaign-related: contact type, duration, number of contacts, previous outcome  

---

## Approach  
1. Loaded and preprocessed the dataset (handled categorical variables with label encoding).  
2. Split the data into training and testing sets (70% / 30%).  
3. Trained a **Decision Tree Classifier** using `scikit-learn` (criterion = entropy, max_depth = 5).  
4. Evaluated the model using accuracy, classification report, and confusion matrix.  
5. Visualized the trained tree to interpret decision paths and feature importance.

---

## Results  
- **Accuracy:** ~89.7%  
- **Precision (Yes class):** 0.58  
- **Recall (Yes class):** 0.32  
- **F1-Score (Yes class):** 0.41  

The model performs well in predicting clients who are unlikely to subscribe but shows limited recall for positive responses.  
The `duration` feature was identified as the most influential factor in determining the outcome.

---



## Files in this Repository  
| File | Description |
|------|--------------|
| `bank.csv` | Dataset used for model training |
| `bank_marketing_decision_tree.ipynb` | Google Colab notebook with complete workflow |
| `output.png` | Visualization of the trained decision tree |
| `README.md` | Project documentation |

---

## How to Run  
1. Open the notebook `bank_marketing_decision_tree.ipynb` in **Google Colab**.  
2. Upload the dataset file `bank.csv` when prompted.  
3. Run all cells sequentially to:
   - Load and preprocess data  
   - Train the Decision Tree model  
   - Evaluate model performance  
   - Generate and view the decision tree visualization  

---

## Citation  
> [Moro et al., 2011] S. Moro, R. Laureano, and P. Cortez.  
> *Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology.*  
> European Simulation and Modelling Conference (ESM’2011), Guimarães, Portugal.

---

