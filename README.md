# 🎓 AI FOR PERSONALIZED ACADEMIC INTERVENTION - Student Risk Prediction & Early Support System

## 📋 Project Track
AI in personalised Learning

## 📋 Project Overview
A machine learning system to predict at-risk students in Python Programming course, enabling early academic interventions.

## 🎯 Problem Statement
Predict which students are at risk of failing Semester End Examination (SEE) based on their CET ranks and Continuous Internal Evaluation (CIE) scores, allowing for timely and personalised academic interventions.

### Real-world Significance
- **Early Identification:** Proactive support before academic failure
- **Resource Optimization:** Focus faculty efforts on students needing most help
- **Data-driven Decisions:** Move from intuition-based to analytics-driven interventions
- **Institutional Impact:** Reduce failure rates and improve learning outcomes

## 📊 Dataset
### Historical Data (Training)
- **Source:** MLR Institute of Technology academic records
- **Period:** 2022-23, 2023-24, 2024-25 academic years
- **Samples:** 2,226 students
- **Features:** CET Rank, CIE-I Score, CIE-II Score, SEE Score
- **Target:** Binary classification (At-Risk: SEE ≤ 39.99)

### 2025-26 Data (Prediction)
- **Structure:** Roll number, Student Name, Department, CET_Rank, CIE_I, CIE_II
- **Samples:** 601 students (current batch for prediction)

## 🏗️ System Architecture

### Data Pipeline
```
Raw Academic Data → Preprocessing → Feature Engineering → Model Training → Prediction → Intervention Recommendations
```

### Key Features Engineered
1. **CET Score Normalization:** Convert ranks to 0-30 scale
2. **Performance Metrics:** CIE averages, improvements, consistency
3. **Risk Indicators:** Flags for declining performance, low scores
4. **Interaction Terms:** CET-CIE interactions for nuanced patterns

### Models Evaluated (7 Algorithms)
1. Logistic Regression
2. Random Forest
3. XGBoost
4. Gradient Boosting
5. Voting Ensemble
6. Stacking Ensemble
7. Neural Network (MLP)

## 📈 Results & Performance

### Best Model: Gradient Boosting
- **Accuracy:** 80.04% (exceeds 80% target)
- **Recall:** 85.81% (identifies most at-risk students)
- **Precision:** 84.97%
- **F1-Score:** 85.39%

### Key Achievements
- ✅ Exceeded 80% accuracy target
- ✅ High recall ensures minimal at-risk students missed
- ✅ Actionable intervention priorities (HIGH/MEDIUM/LOW)
- ✅ Ready for deployment with 2025-26 batch

## 🚀 Quick Start

### File Structure
```
student-risk-prediction/
├── Student_Risk_Prediction_System.ipynb  # Main notebook
├── Total_data.xlsx                        # Training data (2022-25)
├── 2025 Student Data.xlsx                 # 2025-26 prediction data
├── README.md                              # This file
├── requirements.txt                       # Python dependencies
├── 2025_26_Python_Risk_Predictions.csv    # Generated predictions
├── 2025_26_Intervention_List.csv          # Students needing intervention
└── 2025_26_Department_Summary.csv         # Department-wise analysis
```

### Running the Project
1. Upload all files to GitHub repository
2. Open `Student_Risk_Prediction_System.ipynb` in Jupyter/Colab
3. Run all cells (Cell → Run All)
4. Check generated CSV files for predictions

## 📊 Sample Output

### Top At-Risk Students
```
Roll_No      Student_Name      Department  CIE_Avg  Risk_Prob  Risk_Category  Priority
25R21A0501   AKANKASHA V       CSE-A       17.5     0.872      AT-RISK        HIGH
25R21A0502   ANNE HARSHINI     CSE-A       26.5     0.215      NOT AT-RISK    LOW
25R21A0503   ASHRITHA PUPPALA  CSE-A       27.25    0.198      NOT AT-RISK    LOW
```

### Intervention Priority Distribution
- **HIGH:** 85 students (14.1%)
- **MEDIUM:** 167 students (27.8%)
- **LOW:** 349 students (58.1%)

## ⚖️ Ethical Considerations
- Tool for support, not punishment
- Student privacy protection
- Faculty oversight in final decisions
- Regular bias monitoring

## 🔮 Future Enhancements
- Multi-course analysis across first year
- Longitudinal student tracking
- Real-time faculty dashboard
- Mobile alerts for high-risk students

## 📝 Project Report Highlights
- **Methodology:** 7 ML algorithms with hyperparameter optimization
- **Key Insight:** CIE Average is strongest predictor of SEE performance
- **Deployment:** Ready for 2025-26 academic year

## 👥 Target Users
- **Faculty:** Identify at-risk students for targeted support
- **Academic Coordinators:** Monitor batch performance trends
- **Student Counselors:** Proactive counseling for high-risk students

## 📄 License
This project is for academic purposes. Contact the institution for usage permissions.

## 📞 Contact
**Institution:** MLR Institute of Technology, Hyderabad  
**Course:** Python Programming (First Year)  
**Status:** Ready for 2025-26 Deployment

---


*"Data-driven insights for student success"*
