# ⚽ Soccer Transfer Market Player Value Prediction

## 📌 Project Overview

This project applies machine learning techniques to predict the market value of professional soccer players using historical data from Transfermarkt, FBref, and FIFA 21. With soccer transfers involving millions of dollars, accurately valuing players is a critical task for clubs, scouts, and agents. This project builds a predictive regression model that uses over 400 features related to player performance, demographics, and team context across multiple seasons (2017–2020).


## 💼 Business Problem

The transfer market is notoriously complex and often influenced by subjective judgments, hype, or incomplete information. The goal of this project is to build a data-driven model that estimates player market value more objectively. Accurate value prediction can help clubs make smarter financial decisions, reduce transfer risk, and identify undervalued talent.


## 🧠 Research Question

> Can machine learning accurately predict a professional soccer player's market value using performance metrics, physical attributes, and demographic data?


## 📊 Datasets

- **Transfermarkt + FBref Combined Dataset (2017–2020)**  
  > Player appearances, goals, assists, minutes, nationality, position, and market value  
  [Source: Kaggle](https://www.kaggle.com/kriegsmaschine/soccer-players-values-and-their-statistics)

- **FIFA 21 Dataset**  
  > Over 100 player attributes including Attacking, Skills, Mentality, and GK stats  
  Used for context and possible enrichment


## 🔍 Methods

- **Data Cleaning & Preparation**: Handling missing values, feature engineering, encoding categorical variables
- **EDA**: Histograms, boxplots, violin plots, and correlation analysis to uncover patterns
- **Modeling**:
  - Baseline Models: Linear Regression, SVR, Decision Tree, Random Forest, KNN, Gradient Boosting, Gaussian Process
  - Final Model: Tuned Gradient Boosting Regressor using RandomizedSearchCV
- **Evaluation Metrics**: R², RMSE, MAE, residual plots


## 🧪 Results

The **final tuned Gradient Boosting model** achieved:

- **R² Score**: 0.789
- **RMSE**: ~9.05 million
- **MAE**: ~5.19 million
- **Best Parameters**: `n_estimators=300`, `max_depth=5`, `learning_rate=0.1`, `subsample=0.6`

This indicates the model is able to explain nearly 79% of the variance in player market value—an effective outcome for such a subjective domain.


## ⚖️ Ethical Considerations

- Potential for **bias** in nationality, race, or league exposure
- **Privacy concerns** related to salary and performance data
- Need for **transparency** in model interpretation and feature importance
- Risk of misuse in contract negotiations or talent judgment


## 🧩 Challenges Faced

- Handling **outliers** and skewed value distributions
- Managing **multicollinearity** among over 400 features
- Ensuring generalizability to future seasons
- Dealing with **incomplete or inconsistent** real-world data


## 📚 References

- [Kaggle Dataset – Soccer Players Values and Stats](https://www.kaggle.com/kriegsmaschine/soccer-players-values-and-their-statistics)
- [Transfermarkt.com](https://www.transfermarkt.com)
- [FBref.com](https://fbref.com)
- [FIFA 21 Dataset (via Kaggle)](https://www.kaggle.com/stefanoleone992/fifa-21-complete-player-dataset)
- Aurélien Géron – *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow*


## 🚀 Future Improvements

- Integrate real-time player form, injury data, or contract duration
- Build a web dashboard or API for real-time predictions
- Explore deep learning methods for sequential season modeling


## 🧠 Author

**Pragathi Porawakara Arachchige**  
Final Project for DSC680 – Applied Data Science Capstone  
📅 Updated: July 2025  

---

