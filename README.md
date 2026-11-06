# Bangla Telecom and Mobile-Banking Customer-Care Classification

**Course:** CSC4233 – Natural Language Processing  
**Section:** B | **Group:** G14

## Project Overview
This project classifies Bangla telecom and mobile-banking customer-care sentences into six categories using classical NLP and machine learning techniques.

## Dataset
- **Source:** [Bengali Telecom Customer Care Speech](https://huggingface.co/datasets/kawshikbuet17/bengali-telecom-customer-care-speech)
- **Total Sentences:** 2,682
- **Categories:**
  - `mobile_money`
  - `bank_service`
  - `telecom_sim_pack`
  - `security_otp`
  - `complaint_helpline`
  - `generic_dialogue`

## Methodology
1. Dataset preparation and annotation
2. Exploratory Data Analysis (EDA)
3. Bangla text preprocessing
4. Feature extraction
5. Model training and evaluation
6. Error analysis

**Preprocessing:** Unicode normalization, tokenization, stopword removal, and light stemming.

**Feature Extraction:** Bag of Words, TF-IDF, and Word2Vec.

**Models:** Multinomial Naive Bayes, Logistic Regression, and Linear SVM.

## Best Model Results

**Best Model:** Logistic Regression with BoW (Unigram), C = 5.0.

| Metric | Validation | Test |
|---|---:|---:|
| Accuracy | 94.62% | 94.47% |
| Macro-F1 | 94.31% | 94.11% |

## Technologies Used
- Python
- Google Colab
- Pandas and NumPy
- Scikit-learn
- Gensim
- Matplotlib and Seaborn

## Repository Structure
- `01_Source_Code/` – Research notebook
- `02_Dataset/` – Dataset and annotation files
- `03_Experiment_Results/` – Experimental outputs
- `04_Report/` – Final research paper
- `05_Supplementary_Documents/` – Guidelines and statements
- `06_Figures/` – Research figures

## Team Members

| Member | Name | Student ID |
|---|---|---|
| Member 1 | [Maisha Mahjabin] |
| Member 2 | [Md. Sadat Hossain] |
| Member 3 | [Mishal] | 

## Future Work
Explore transformer-based models such as BanglaBERT, mBERT, and XLM-R for improved classification performance.

## Acknowledgment
We acknowledge the dataset creators and the developers of the open-source libraries used in this project.
