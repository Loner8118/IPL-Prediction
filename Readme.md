🏏 IPL Match Winner Prediction (Machine Learning Project)

📌 Overview
Developed an end-to-end machine learning system to predict IPL match outcomes using historical data from 2008–2025. The project focuses on leveraging team performance, match conditions, and player statistics to model match results and evaluate predictive accuracy on unseen seasons.

🎯 Objectives
Build a robust prediction pipeline for IPL match outcomes
Perform advanced feature engineering using historical and player-level data
Compare multiple ML models and evaluate performance on future matches
Understand limitations of predictive modeling in real-world sports analytics

🛠️ Tech Stack
Programming: Python
Libraries: Pandas, NumPy, Scikit-learn, XGBoost
Visualization: Matplotlib, Seaborn
Tools: Jupyter Notebook

⚙️ Methodology
1. Data Preprocessing
Cleaned and standardized team names across seasons
Handled missing values and inconsistent records
Ensured dataset compatibility across different years

2. Feature Engineering
Created meaningful features to improve model performance:

Team Metrics:
Win percentage
Recent form (last 5 matches)
Match Context Features:
Toss winner & decision
Venue encoding
Batting first advantage
Head-to-Head Analysis:
Historical win ratio between teams
Player-Level Features:
Average batting runs
Strike rate
Bowling wickets
Economy rate

3. Encoding
Applied Label Encoding on categorical features
Handled unseen labels in 2025 dataset using safe encoding strategy

4. Train-Test Strategy
Training Set: 2008–2023
Validation Set: 2024
Prediction Set: 2025
This ensures realistic evaluation on future unseen data.

5. Model Training
Trained and compared:
Random Forest Classifier
XGBoost Classifier
Best model selected based on validation accuracy.

📊 Results
🔹 Validation Performance (2024)
Random Forest Accuracy: 49.3%
XGBoost Accuracy: 46.5%
🔹 2025 Prediction Performance
Random Forest Accuracy: 52.7%
XGBoost Accuracy: 52.7%

👉 The near-random accuracy reflects the high unpredictability of T20 cricket, highlighting limitations of data-driven models in dynamic environments.

📁 Outputs
ipl_2025_predictions.csv → Predicted winners
model_summary.csv → Model comparison
feature_importance.csv → Key influencing features

📂 Project Structure
├── data/
│   ├── matches.csv
│   ├── deliveries.csv
│   └── 2025/
│       ├── matches.csv
│       ├── ipl_batsman.csv
│       └── ipl_bowler.csv
├── notebooks/
│   ├── Prediction.csv
│   submission/
│   ├── model_summary.csv
│   └── feature_importance.csv
├── requirements.txt
└── README.md

🚀 How to Run the Project
1. Clone the repository
git clone <your-repo-link>
cd <project-folder>

2. Install dependencies
pip install -r requirements.txt

3. Run Jupyter Notebook
jupyter notebook
Run all cells step by step.

🚧 Challenges
Handling missing and inconsistent data across seasons
Encoding categorical variables with unseen future values
Extracting meaningful insights from noisy player statistics
Achieving high accuracy due to randomness in match outcomes

💡 Key Learnings
Importance of feature engineering in ML pipelines
Real-world datasets require extensive preprocessing
Model performance depends heavily on feature quality
Sports analytics involves high uncertainty and external factors

🔮 Future Scope
Integrate real-time player and match data
Include weather and pitch conditions
Apply deep learning models
Build a live prediction web app using Flask

🏁 Conclusion
This project demonstrates a complete machine learning workflow—from raw data preprocessing to model evaluation and future predictions. It highlights both the potential and limitations of ML in sports analytics, especially in highly dynamic environments like IPL.

👨‍💻 Author-
Tanish Akre
Computer Engineering Student