Smoking Status Prediction using Blended Deep Learning

#Team Info:
22471A0517 — Duggi Sampath Kumar ( [LinkedIn](https://www.linkedin.com/in/sampath-kumar-duggi-b73b2b379?utm_source=share_via&utm_content=profile&utm_medium=member_android) )
Work Done: Data preprocessing, EDA, documentation
22471A0513 — Chirumala Charan Teja ([LinkedIn](
 ))
Work Done: Feature engineering, model implementation (ESN, GoogleNet)
22471A0522 — Garikapudi Prudhviraj( [LinkedIn](https://www.linkedin.com/in/prudhvi-garikapudi-1748a8356?utm_source=share_via&utm_content=profile&utm_medium=member_android))

Work Done: Deployment, testing, UI
Abstract

Cardiovascular diseases (CVD) are one of the leading causes of death worldwide, and smoking is a major contributing factor. However, many individuals conceal their smoking habits, making early detection difficult.

This project proposes a blended deep learning model to predict hidden smoking behavior using bio-signal data. The system integrates multiple deep learning architectures—Echo State Network (ESN) and GoogleNet as base learners, and AlexNet as a meta-classifier.

Advanced preprocessing techniques such as Robust Scaling, Random Forest feature selection, and Borderline-SMOTE are applied to improve model performance. The model achieves approximately 92% accuracy and provides explainability using SHAP (Shapley Additive Explanations), making it suitable for healthcare decision support systems.

Paper Reference (Inspiration)

👉 [A Blended Deep Learning Approach for Hidden Prediction of Smoking Status to Reduce the Risk of Cardiovascular Disease
– Gaddam Saranya et al.](Paper URL here)

Original IEEE-style research paper used as inspiration for the model.

Our Improvement Over Existing Paper
Enhanced preprocessing pipeline for better data quality
Improved feature selection using optimized Random Forest tuning
Better handling of class imbalance using improved SMOTE techniques
Hyperparameter tuning for improved model stability
Added detailed visualization (EDA, ROC, confusion matrix)
Improved explainability using SHAP plots
Designed system for real-world deployment (web/app integration)
About the Project
🔍 What the Project Does

This project predicts whether a person is:

Smoker (1)
Non-Smoker (0)
using health and bio-signal data.
🎯 Why It Is Useful
Helps in early detection of cardiovascular disease risk
Identifies hidden smokers who do not self-report
Supports doctors in preventive healthcare
Can be integrated into smart healthcare systems
⚙️ Workflow
Input Data → Data Preprocessing → Feature Selection → 
Class Balancing → Model Training → 
Blended Model (ESN + GoogleNet → AlexNet) → Output Prediction
Dataset Used

👉 [Smoking Prediction Dataset (Kaggle)](Dataset URL)

📊 Dataset Details:
300,000+ records
40+ features
Target: Smoking (0 = No, 1 = Yes)
📌 Features Include:
Age
BMI
Blood Pressure
Cholesterol Levels
Glucose
Hemoglobin
Dependencies Used
Python
NumPy
Pandas
Scikit-learn
TensorFlow / PyTorch
Matplotlib
Seaborn
SHAP
EDA & Preprocessing
Removed missing values and duplicates
Applied Robust Scaling to handle outliers
Performed Random Forest Feature Selection
Balanced dataset using Borderline-SMOTE
Normalized and transformed data for better model input
Model Training Info
🧠 Model Architecture
Base Models:
Echo State Network (ESN)
GoogleNet
Meta Model:
AlexNet
⚙️ Training Strategy
10-Fold Cross Validation
Ensemble Learning (Blending)
Hyperparameter tuning
Model Testing / Evaluation
📊 Metrics Used:
Accuracy
Precision
Recall
F1-score
📉 Additional Evaluation:
Confusion Matrix
ROC Curve
Probability Distribution Analysis
SHAP Explainability
Results
✅ Accuracy: ~92%
✅ High precision and recall
✅ Effective detection of hidden smokers
✅ Balanced performance across dataset
Limitations & Future Work
❌ Limitations:
Prediction probabilities are very close (low confidence spread)
ROC curve indicates possible classification limitations
High computational complexity
Requires large dataset
🔮 Future Work:
Use Transformer-based models
Improve probability confidence separation
Integrate real-time wearable data
Deploy in healthcare applications
Optimize model for faster inference
Deployment Info
💻 Deployment Options:
Web App using Flask / Streamlit
Mobile App integration
Cloud-based API
🌐 Real-World Applications:
Hospitals
Health monitoring systems
Wearable devices
Smart healthcare platforms
