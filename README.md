# Linear Regression: MovieLens 20M Dataset

**Course:** Data Analysis with Python  
**Institution:** National Economics University (NEU) – Faculty of Data Science and Artificial Intelligence (FDA)  
**Academic Adviser:** Trần Đức Minh  

## Research Team
| Name | Student ID |
| :--- | :--- |
| Nguyễn Hoàng Hải | 11252782 |
| Hoàng Trung Kiên | 11254023 |
| Trần Ngọc Mai | 11255185 |

## Project Overview
This project predicts the average community rating (`avg_rating`) of movies from the **MovieLens 20M Dataset** using intrinsic metadata, community tagging activity, and Tag Genome semantic relevance scores. After out-of-core chunked aggregation and data cleaning, the final modeling dataset contains **15,451 movies** and **26 leakage-free predictors**.

## Model Performance (Test Set)
| Model | MAE | RMSE | $R^2$ |
| :--- | :---: | :---: | :---: |
| Baseline (Mean) | 0.3945 | 0.4997 | -0.0001 |
| Linear Regression | 0.2817 | 0.3760 | 0.4337 |
| Random Forest | 0.2638 | 0.3613 | 0.4773 |
| **XGBoost (Best)** | **0.2572** | **0.3524** | **0.5026** |

## Repository Structure
- `MIDTERM_DA.pdf`: Full project report.
- `midterm_code.ipynb`: Complete Python pipeline (Data Inspection, Chunked Aggregation, Cleaning, EDA, Modeling & Evaluation).
- `feature_cols.json` & `target_col.json`: Selected feature list and target variable configuration.
- `fig*.png / *.jpg`: Visualizations and diagnostic charts used in the report.
