# 🏈 University Football Injury Prediction (UFIP)  

## 📌 Project Overview  
This project leverages the **University Football Injury Prediction Dataset (UFIP)** to build machine learning models that predict the likelihood of a university football player sustaining an injury in the next academic season.  

The dataset provides comprehensive physical, fitness, lifestyle, and football-related metrics of **800 Chinese university football players**, making it a valuable resource for **sports science research, injury prevention, and applied machine learning**.  

---

## 📊 Dataset Details  
- **Samples:** 800 players  
- **Features:** 18 input features + 1 target label  
- **Target:** `Injury_Next_Season` (Binary classification → `0 = No Injury`, `1 = Injury`)  
- **Balance:** Well-balanced dataset  
- **Age Range:** 18–24 years (typical university students)  

---

## 🏃‍♂️ Feature Categories  

**Physical Characteristics (4 features)**  
- Age, Height, Weight, BMI  

**Football-Specific Metrics (4 features)**  
- Playing Position, Training Hours/Week, Matches Played, Injury History  

**Physical Fitness Assessment (6 features)**  
- Knee Strength, Hamstring Flexibility, Reaction Time, Balance, Sprint Speed, Agility  

**Lifestyle Factors (3 features)**  
- Sleep Hours, Stress Level, Nutrition Quality  

**Training Compliance (1 feature)**  
- Warm-up Routine Adherence (`0 = Poor`, `1 = Good`)  

---

## 🎯 Target Variable  
**`Injury_Next_Season`**  
- Binary classification outcome  
- Injury defined as ≥7 consecutive days of absence due to training/competition injury  
- Verified via **medical center records & coaching staff reports**  

---

## 🔬 Data Quality & Validation  
- **Collection Period:** First 4 weeks of each academic year  
- **Validation:** Medical records + coach reports + surveys  
- **Quality Control:** Sports medicine professional review  
- **Missing Data:** Minimal (cross-verified)  

---

## 🚀 Applications  
- **Sports Medicine Research:** Identify key injury risk factors  
- **Preventive Healthcare:** Develop injury prevention strategies  
- **University Sports Management:** Athlete risk assessment  
- **Machine Learning:** Benchmark healthcare classification models  

---

## ⚙️ Workflow / Pipeline  

The notebook follows a structured **ML pipeline**:  

1. **Data Understanding & Exploration**  
   - Import libraries (pandas, numpy, matplotlib, seaborn, scikit-learn, etc.)  
   - Load dataset into pandas DataFrame  
   - Explore feature distributions, summary statistics, and correlations  

2. **Data Preprocessing**  
   - Handle missing values (if any)  
   - Encode categorical variables (e.g., Playing Position, Warm-up Routine Adherence)  
   - Scale/normalize numerical features  
   - Train-test split with stratification  

3. **Exploratory Data Analysis (EDA)**  
   - Visualizations of physical, lifestyle, and football-specific features  
   - Injury distribution across different factors (e.g., position, training hours, stress level)  
   - Boxplots, histograms, and correlation heatmaps  

4. **Model Training & Evaluation**  
   - Classical ML models: Logistic Regression, Random Forest, SVM, XGBoost  
   - Evaluation metrics: Accuracy, Precision, Recall, F1-Score, AUC-ROC  
   - Cross-validation with stratified sampling  

5. **Model Comparison**  
   - Compare results across models using key metrics  
   - Identify best-performing algorithm(s) for injury prediction  

6. **Insights & Recommendations**  
   - Highlight key risk factors  
   - Suggest preventive measures for student athletes  

---

## 📈 Suggested Machine Learning Approaches  
- **Classical Models:** Logistic Regression, Random Forest, SVM, XGBoost  
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score, AUC-ROC  
- **Validation:** Cross-validation with stratified sampling  

---

## 🏆 Research Value  
This dataset uniquely bridges **sports science** and **machine learning**, providing:  
- Insights into **university-level athlete injury prediction**  
- A benchmark dataset for **healthcare classification models**  
- Opportunities to design **data-driven prevention strategies**  

---

## 🛠️ How to Use This Repository  
1. Clone the repo:  
   ```bash
   git clone https://github.com/your-username/UFIP.git
   cd UFIP
2. Install dependencies: ```bash
   pip install -r requirements.txt
3. Open the notebook:
   jupyter notebook UFIP.ipynb
4. Run cells sequentially to reproduce the analysis.

---
🤝 Contributions are welcome!
- Fork the repo
- Create a new branch (git checkout -b feature-name)
- Commit changes (git commit -m "Add feature")
- Push to your branch and open a Pull Request
