# 🔥 Fire Propagation Stage 1 — Fire Occurrence Prediction

This project builds a **physics-informed machine learning model** to detect and predict the **occurrence of forest fires**, using physical fire indices such as ISI, FFMC, BUI, and FWI. The approach combines:

- 🔍 **Correlation filtering** of physical variables
- 🧠 **Unsupervised clustering** into positive and negative fire signal dimensions
- 🧠 **Neural network modeling** using PyTorch
- ✅ High accuracy on structured fire datasets (e.g., Algeria)

## 📁 Contents

- `Fire Propagation Stage 1 - Fire Occurence.ipynb`  
  Main notebook containing full pipeline from raw data to model evaluation.

- **Required Data File**:
  `Cleaned_Algerian_Forest_Fire_Data.csv` (from UCI Machine Learning Repository)

## ⚙️ Instructions

1. Clone this repository or download the `.ipynb` notebook.
2. Place `Cleaned_Algerian_Forest_Fire_Data.csv` in the **same folder** as the notebook.
3. ⚠️ Update the **file path** in the notebook if needed:
   ```python
   pd.read_csv("Cleaned_Algerian_Forest_Fire_Data.csv")  # Change this if your file path differs
   ```
4. Run the notebook end-to-end in **Jupyter** or **JupyterLab**.

## 📊 Model Highlights

- Derives `BUI` and `FWI` using known fire index equations
- Applies cluster-based latent inputs
- Learns propagation likelihood from structured correlations
- Recall on fire occurrence: **1.00** (100%)  
  Accuracy: **up to 96%** on Algerian data; **~55%** on UCI

## 📄 License

MIT License — you are free to reuse, extend, or build upon this work.

---

**Scientific Note**:  
This stage focuses only on **binary fire occurrence**. Future stages may expand to **fire spread modeling**, rate prediction, or geographic simulation.