# DRAP – Drug Repurposing Analytics Platform

A lightweight, technical project demonstrating an end-to-end cheminformatics + ML workflow for early-stage drug repurposing.  
Built using SMILES-based descriptor generation (RDKit) and QSAR modeling (Random Forest).

---

## 📌 Objective
Create a reproducible pipeline that:
- Reads molecular SMILES
- Generates basic molecular descriptors
- Builds a regression QSAR model to predict activity
- Saves the trained model for future use

---

## 📁 Project Structure
```
drap-drug-repurposing/
│
├── data/
│     ├── sample_molecules.csv
│     └── descriptors_dataset.csv
│
├── notebooks/
│     ├── 01_data_loading.ipynb
│     ├── 02_descriptor_generation.ipynb
│     └── 03_qsar_model.ipynb
│
├── src/
│     └── qsar_model.pkl
│
└── README.md
```

---

## 🔧 Tech Stack
- Python  
- RDKit  
- Pandas, NumPy  
- Scikit-Learn  
- Jupyter Notebook  
- Joblib  
- GitHub for version control  

---

## ▶️ Setup Instructions

### **1. Create and activate environment**
```bash
conda create -n drap python=3.11
conda activate drap
```

### **2. Install dependencies**
```bash
conda install -c conda-forge rdkit
pip install pandas numpy scikit-learn joblib jupyter
```

### **3. Launch Jupyter Notebook**
```bash
jupyter notebook
```

### **4. Run notebooks sequentially**
1. `01_data_loading.ipynb`  
2. `02_descriptor_generation.ipynb`  
3. `03_qsar_model.ipynb`  

---

## 📊 Output (Phase 1)
- Descriptor dataset generated using RDKit  
- Random Forest QSAR model trained  
- Model saved as:  
```
src/qsar_model.pkl
```

---

## 🔜 Future Enhancements
- Add molecular docking (AutoDock Vina)  
- Combine QSAR + Docking into unified scorecard  
- Build Streamlit or Power BI dashboard  
- Add FastAPI endpoint for “Predict activity from SMILES”  

---
