# Data Mining Methodologies: CRISP-DM, KDD, and SEMMA

This repository contains comprehensive implementations of three major data mining methodologies applied to real-world datasets. Each notebook demonstrates end-to-end data science workflows with built-in expert critiques.

## Medium Article Link
[crisp-dm-vs-kdd-vs-semma](https://medium.com/@yashkalathiya164/crisp-dm-vs-kdd-vs-semma-a-practical-comparison-of-data-mining-methodologies-6588523ca30a)

## 📁 Project Structure

```
.
├── README.md
├── crisp_dm/
│   ├── crisp_dm.ipynb              # CRISP-DM methodology notebook
│   ├── flight_track.csv            # Flight tracking dataset
│   ├── flight_track_rf_model.pkl   # Trained Random Forest model
│   ├── flight_track_scaler.pkl     # Feature scaler
│   ├── model_metadata.pkl          # Model metadata
│   ├── crispDM_part_1.mp4          # Video demo (Part 1)
│   └── crispDM_part_2.mp4          # Video demo (Part 2)
├── KDD/
│   ├── kdd.ipynb                   # KDD methodology notebook
│   ├── Zara_sales_EDA.csv          # Zara sales dataset
│   ├── zara_sales_model.pkl        # Trained model
│   ├── label_encoders.pkl          # Label encoders
│   ├── model_metadata.pkl          # Model metadata
│   └── kdd.mp4                     # Video demo
└── semma/
    ├── semma.ipynb                 # SEMMA methodology notebook
    ├── insurance.csv               # Insurance dataset
    └── semma.mp4                   # Video demo
```

## 🎯 Project Overview

### 1. CRISP-DM: Flight Track Prediction Challenge
**Methodology:** Cross-Industry Standard Process for Data Mining  
**Dataset:** Flight tracking data  
**Objective:** Predict flight positions based on temporal and spatial features  
**Key Phases:**
1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Deployment

**Results:**
- **Linear Regression:** MAE=19.49, R²=0.0
- **Random Forest:** MAE=19.41, R²=-0.0004
- **Key Learning:** Zero correlation between features and target - demonstrated importance of correlation analysis and honest failure reporting

### 2. KDD: Zara Sales Prediction
**Methodology:** Knowledge Discovery in Databases  
**Dataset:** Zara sales data (semicolon-separated)  
**Objective:** Predict sales based on product attributes and store information  
**Key Phases:**
1. Selection
2. Preprocessing
3. Transformation
4. Data Mining
5. Interpretation/Evaluation

**Results:**
- **Linear Regression:** MAE=[value], R²=[value]
- **Random Forest:** MAE=[value], R²=[value]
- **Top Drivers:** Product category, price, store location

### 3. SEMMA: Insurance Charges Prediction
**Methodology:** Sample, Explore, Modify, Model, Assess  
**Dataset:** Insurance charges data  
**Objective:** Predict insurance charges based on demographic and health factors  
**Key Phases:**
1. Sample
2. Explore
3. Modify
4. Model
5. Assess

**Results:**
- **Linear Regression:** MAE=$4,367, R²=0.756
- **Random Forest:** MAE=$2,633, R²=0.852 ✅
- **Success Criteria:** ✅ EXCEEDED (MAE < $3,500, R² ≥ 0.60)
- **Top Driver:** Smoker status (60% feature importance)

## 🚀 How to Run

### Prerequisites

1. **Python 3.8+** installed
2. **Jupyter Notebook** or **VS Code with Jupyter extension**
3. Required Python packages (see installation below)

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/ykalathiya-2/crispdm_kdd_semma.git
cd crispdm_kdd_semma
```

2. **Create a virtual environment (recommended):**
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. **Install required packages:**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib jupyter
```

Or install from requirements file:
```bash
pip install -r requirements.txt
```

### Running the Notebooks

#### Option 1: Using Jupyter Notebook
```bash
# Navigate to desired folder
cd crisp_dm  # or KDD or semma

# Start Jupyter Notebook
jupyter notebook

# Open the .ipynb file in your browser
```

#### Option 2: Using VS Code
```bash
# Open the project folder in VS Code
code .

# Navigate to any .ipynb file
# Click "Run All" or run cells individually with Shift+Enter
```

#### Option 3: Running Individual Notebooks

**CRISP-DM Notebook:**
```bash
cd crisp_dm
jupyter notebook crisp_dm.ipynb
# Run all cells sequentially
```

**KDD Notebook:**
```bash
cd KDD
jupyter notebook kdd.ipynb
# Run all cells sequentially
```

**SEMMA Notebook:**
```bash
cd semma
jupyter notebook semma.ipynb
# Run all cells sequentially
```

### Expected Execution Time
- **CRISP-DM:** ~30 seconds
- **KDD:** ~45 seconds
- **SEMMA:** ~20 seconds

## 📝 Prompts Used to Create Notebooks

### Initial Prompt for CRISP-DM Notebook

```
Create a master prompt for a CRISP-DM notebook for the Flight Track Prediction Challenge.

Requirements:
1. Dual Persona: Author (data scientist) and Critic (Prof. CRISP-DM)
2. Structure:
   - Each CRISP-DM phase as a markdown section
   - Code cells implementing the phase
   - Critique cell after each code cell with:
     ✅ What was done well
     ⚠️ Gaps, risks, or missing elements
     Next steps: Concrete suggestions

3. Phases to include:
   - Business Understanding
   - Data Understanding
   - Data Preparation
   - Modeling
   - Evaluation
   - Deployment

4. Success criteria:
   - MAE < 15 for position prediction
   - R² ≥ 0.70
   - Identify top 3-5 drivers

5. After running, provide comprehensive final critique analyzing the failure
   and lessons learned
```

### Follow-up Prompt for KDD Notebook

```
Create similar notebooks for KDD (using Zara sales dataset) and SEMMA 
(using insurance dataset).

Each should follow the same pattern:
- Built-in expert critic after each code cell
- All phases of the methodology
- Success criteria clearly defined
- Comprehensive final assessment
```

### SEMMA Notebook Specific Requirements

```
SEMMA phases:
1. Sample - Select and partition data
2. Explore - Visualize and understand
3. Modify - Clean, transform, engineer features
4. Model - Build and compare models
5. Assess - Evaluate performance and business impact

Success criteria:
- MAE < $3,500
- R² ≥ 0.60
- Identify top 3-5 drivers of insurance charges
```

## 🧑‍⚖️ Built-in Expert Critiques

Each notebook includes **Prof. [Methodology]**, a world-renowned expert who provides:

- ✅ **Strengths:** What was done well
- ⚠️ **Gaps & Risks:** Missing elements, potential issues
- **Next Steps:** Concrete, actionable suggestions
- **Final Assessment:** Overall grade and deployment recommendation

This approach ensures:
- **Learning by doing and reviewing**
- **Industry best practices** are highlighted
- **Common pitfalls** are identified
- **Continuous improvement** mindset

## 📊 Key Learnings

### From CRISP-DM (Flight Track)
- **Correlation analysis is critical** - zero correlation means no predictive power
- **Honest failure reporting** is valuable - documented what didn't work and why
- **Domain knowledge matters** - random tracking IDs don't predict positions
- **Model deployment decisions** - don't deploy models that fail business criteria

### From KDD (Zara Sales)
- **Data preprocessing is essential** - handled semicolon separators correctly
- **Feature engineering** can significantly improve model performance
- **Business context** drives feature selection

### From SEMMA (Insurance)
- **Feature importance** provides actionable business insights
- **Success criteria** should be defined upfront and measurable
- **Outliers aren't always errors** - high charges are valid business cases
- **Model interpretability** matters for business stakeholders

## 🎓 Educational Value

These notebooks serve as:

1. **Reference implementations** of three major data mining methodologies
2. **Template for assignment submissions** with built-in quality checks
3. **Learning resource** demonstrating end-to-end data science workflows
4. **Best practices guide** with expert critiques at each step

## 📹 Video Demonstrations

Each folder contains video demonstrations (`.mp4` files) walking through:
- Notebook execution
- Key insights and findings
- Methodology application
- Results interpretation

## 📝 Blog & Publications

**Medium Article:** [CRISP-DM vs KDD vs SEMMA: A Practical Comparison](MEDIUM_BLOG.md)

Read the complete story about this project, including:
- Head-to-head methodology comparison
- What I learned from a model with R² = -0.0004
- The innovation of built-in AI critique
- When to use each methodology
- 7 key lessons learned

**Files:**
- `MEDIUM_BLOG.md` — Complete Medium article (ready to publish)
- `SOCIAL_MEDIA_CONTENT.md` — LinkedIn, Twitter, Reddit posts
- `PUBLISHING_GUIDE.md` — How to publish and promote

## 🔧 Troubleshooting

### Common Issues

**Issue:** `ModuleNotFoundError: No module named 'sklearn'`
```bash
pip install scikit-learn
```

**Issue:** Correlation heatmap error with string columns
```python
# Use only numeric columns
sns.heatmap(df.select_dtypes(include=[np.number]).corr(), annot=True)
```

**Issue:** Semicolon-separated CSV not loading correctly
```python
# Specify delimiter
df = pd.read_csv('file.csv', sep=';')
```

## 📄 License

This project is for educational purposes as part of a data science assignment.

## 👤 Author

**Yash Kalathiya**  
Data Science Student  
November 2025

## 🙏 Acknowledgments

- CRISP-DM methodology framework
- KDD process reference
- SEMMA methodology (SAS Institute)
- Scikit-learn documentation
- Seaborn visualization library

---

**Note:** This repository demonstrates the application of three different data mining methodologies to real-world problems, with emphasis on rigorous self-critique and continuous improvement.
