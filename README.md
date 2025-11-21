# Enzyme Function Classification Using Amino Acid Composition  
Machine Learning Final Project — EC1 vs. EC2 Classification

This project tests whether amino acid composition alone can classify enzymes as oxidoreductases (EC 1) or transferases (EC 2). Using curated *E. coli* K-12 proteins from UniProtKB/Swiss-Prot, we compute 20 amino acid frequency features and train three machine learning models to evaluate classification performance.

##  Research Question
Can amino acid composition alone classify EC1 vs. EC2 enzymes better than random?

##  Methods Overview
- Parse FASTA sequences with Biopython  
- Compute amino acid composition (20 features)  
- Balance dataset: 400 EC1, 400 EC2  
- Train/test split (75/25, stratified)  
- Models used: Logistic Regression, SVM (RBF), Random Forest  
- Evaluation: Accuracy, macro F1-score, ROC AUC  
- Visualizations: Confusion matrix, ROC curve, PCA

## Repository Structure

```
enzyme-ml-final-project
│
├── README.md
├── ai_usage.md
├── requirements.txt
│
├── notebooks/
│   └── final_project.ipynb
│
├── data/
│   └── instructions.txt
│
└── figures/
    ├── confusion_matrix.png
    ├── roc_curve.png
    └── pca_plot.png
```
## How to Run

1. Clone the repository:
```bash
git clone https://github.com/Ishaq408013/enzyme-ml-final-project.git
cd enzyme-ml-final-project
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the notebook:
```bash
jupyter notebook notebooks/final_project.ipynb
```

## Reproducibility
## AI Usage
See `ai_usage.md` for documentation on how AI tools assisted in this project.
