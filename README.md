# Data-Preprocessing-Peer-16
# Customer Spending Prediction Pipeline
A machine learning pipeline for predicting customer spending behavior using transactional and social media data.

---

## Project Overview
This project implements a complete ML pipeline to:
1. **Augment** transactional data with synthetic samples
2. **Merge** heterogeneous datasets using ID mapping
3. Perform **data quality checks**
4. Predict customer spending using **XGBoost/Random Forest**

Key Features:
- Automated missing value imputation
- Feature engineering with TF-IDF
- Transitive dataset merging
- Model performance visualization

---

## Repository Structure
```
.
├── notebook/
│   ├── Data-Preprocessing-Peer-16
│   
├── data/
│   ├── raw/ (initial datasets)
│   ├── processed/ (augmented/merged data)
│   └── final/ (ML-ready data)
├── models/
│   └── best_spending_predictor.pkl
├── reports/
│   ├── technical_report.pdf
│   └── visualizations/ (plots)
├── requirements.txt
└── README.md
```

---

## Installation
1. Clone repository:
```bash
git clone https://github.com/dntwaritag/Data-Preprocessing-Peer-16.git
cd customer-spending-prediction
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```
**Key Libraries:**
- Python 3.9+
- pandas
- scikit-learn
- XGBoost
- matplotlib
- jupyter

---

## Usage
1. **Data Augmentation**:
```Collab
Run Part1_Data_Augmentation.ipynb
```
2. **Dataset Merging**:
```Collab
Run Part2_Dataset_Merging.ipynb
```
3. **Data Quality Checks**:
```Collab
Run Part3_Data_Quality.ipynb
```
4. **ML Model Training**:
```Collab
Run Bonus_ML_Model.ipynb
```

---

## Datasets
1. **id_mapping.csv**  
   - Maps legacy customer IDs to new IDs
   - Columns: `customer_id_legacy`, `customer_id_new`

2. **customer_transactions.csv**  
   - Transaction records with purchase details  
   - Columns: `customer_id_legacy`, `transaction_id`, `purchase_amount`, etc.

3. **customer_social_profiles.csv**  
   - Social media engagement metrics  
   - Columns: `customer_id_new`, `engagement_score`, `purchase_interest_score`, etc.

---

## Bonus Challenge (ML Model)
**Implementation:**
- Trained XGBoost and Random Forest models
- Achieved **R² score of 0.85** on test data

**To Reproduce:**
1. Ensure final dataset exists (`final_dataset_ready_group16.csv`)
2. Run:
```bash
jupyter notebook Bonus_ML_Model.ipynb
```

**Output:**
- Model performance metrics (MAE/RMSE/R²)
- Feature importance plots
- Saved model (`best_spending_predictor.pkl`)

---

## Team Contributions
| Member         | Role                                      |
|----------------|-------------------------------------------|
| Denys Ntwaritaganzwa    | Data cleaning , augmentation & report writing |
| Aubin Ntwali     | Dataset merging , conflict resolution &  ML modeling |
| Anissa Ouedraogo    | Feature engineering & quality checks     |

---

## Video Presentation
Link to the team [presentation](https://drive.google.com/file/d/1Q4HFPhRVcuH6_kXvqhyiitEidKpTQhzu/view?usp=sharing) 

---

## Report
Link to the team [pdf Document](https://docs.google.com/document/d/1S1298S2L7PVEqkzBLG8wxnMzwkkO0O8awZ0lkbRkBrU/edit?usp=sharing)  

---
## License
This project is licensed under the [MIT License](LICENSE).

---

## Contact
For questions, contact:  
Denys Ntwaritaganzwa - d.ntwaritag@alustudent.com  
Aubin Ntwali - a.ntwali@alustudent.com                                                                                                                                                    
Anissa Ouedraogo - a.ouedraogo@alustudent.com           


```
