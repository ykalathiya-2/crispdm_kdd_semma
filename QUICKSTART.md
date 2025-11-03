# Quick Start Guide

## 🚀 Get Started in 3 Steps

### Step 1: Setup Environment
```bash
# Clone and navigate
git clone https://github.com/ykalathiya-2/crispdm_kdd_semma.git
cd crispdm_kdd_semma

# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Step 2: Choose Your Methodology

Pick one of the three methodologies to explore:

#### 🔵 CRISP-DM (Flight Tracking)
```bash
cd crisp_dm
jupyter notebook crisp_dm.ipynb
```
**What you'll learn:** How to handle model failures, importance of correlation analysis

#### 🟢 KDD (Zara Sales)
```bash
cd KDD
jupyter notebook kdd.ipynb
```
**What you'll learn:** Data preprocessing, feature engineering, business insights

#### 🟡 SEMMA (Insurance Charges)
```bash
cd semma
jupyter notebook semma.ipynb
```
**What you'll learn:** Complete successful workflow, feature importance, deployment readiness

### Step 3: Run and Learn

1. **Run All Cells:** Click "Cell" → "Run All" or use Shift+Enter for each cell
2. **Read Critiques:** After each code cell, read Prof. [Methodology]'s feedback
3. **Understand Results:** Check model performance against success criteria
4. **Apply Learnings:** Use insights for your own projects

## 💡 Pro Tips

- **Start with SEMMA** - it's the most successful implementation
- **Read critiques carefully** - they contain valuable insights
- **Compare methodologies** - see how each approach handles similar problems
- **Watch videos** - each folder has .mp4 demonstrations

## 📊 Expected Results

| Methodology | Dataset | Best Model | MAE | R² | Success? |
|------------|---------|------------|-----|-----|----------|
| CRISP-DM | Flight Track | Random Forest | 19.41 | -0.0004 | ❌ No |
| KDD | Zara Sales | Random Forest | TBD | TBD | ✅ Yes |
| SEMMA | Insurance | Random Forest | $2,633 | 0.852 | ✅ Yes |

## 🆘 Need Help?

- Check `README.md` for detailed documentation
- Review troubleshooting section
- Examine code comments in notebooks
- Watch video demonstrations

## 🎯 Success Indicators

You're on the right track if you see:
- ✅ All cells execute without errors
- ✅ Visualizations display correctly
- ✅ Model metrics are calculated
- ✅ Critique sections appear after code cells
- ✅ Final assessment provides grades

Happy Data Mining! 🎓
