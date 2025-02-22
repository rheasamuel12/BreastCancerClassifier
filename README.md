# BreastCancerClassifier

## Overview  
This project aims to predict whether a breast cancer patient will experience a recurrence of the cancer. My goal is to fit 3 different classification models to predict recurrence outcomes. 

## Dataset Description  
### Independent Features (Predictors)  
- **Age**: Age group
- **Menopause**: Menopausal status
- **Tumor-size**: Size of the tumor.  
- **Inv-nodes**: Range of involved lymph nodes  
- **Node-caps**: Presence of node capsule.  
- **Deg-malig**: Degree of malignancy
- **Breast**: Breast affected
- **Breast-quad**: Quadrant of the breast affected
- **Irradiat**: Presence of radiation therapy 

### Dependent Variable 
- **Class**: Recurrence status of cancer:  
  - `recurrence-events`
  - `no-recurrence-events` 

## Data Preparation  
1. **Handling Data** – Identified and processed null values in tumor size and lymph node involvement. Dropped duplicate values
2. **One-Hot Encoding** – Converted categorical features into binary columns for model compatibility.  
3. **Splitting the Data** – Ensured reproducibility and maintained class balance in training and test sets.  

## Model Training and Performance 
- Implemented classification models: KNN, KNN using GridSearchCV, and Linear classification.  
- Evaluated performance using accuracy, precision, recall, and F1-score.  


## Usage  
Clone the repository and run the provided scripts to preprocess the data and train models:  
```bash
git clone <repository-url>
cd breast-cancer-prediction
python train_model.py
