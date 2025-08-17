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
  `Cleaned_Algerian_Forest_Fire_Data.csv` (available in the repository, it is a cleaned version of 'algerian+forest+fires+dataset' from UCI Machine Learning Repository)

## ⚙️ Instructions

1. Clone this repository or download the `.ipynb` notebook.
2. Place `Cleaned_Algerian_Forest_Fire_Data.csv` in the **same folder** as the notebook.
3. ⚠️ Update the **file path** in the notebook if needed:
   ```python
   pd.read_csv("Cleaned_Algerian_Forest_Fire_Data.csv")  # Change this if your file path differs
   ```
4. Run the notebook end-to-end in **Jupyter** or **JupyterLab**.

## 📊 Model Highlights

- Applies cluster-based latent inputs
- Learns propagation likelihood from structured correlations
- Accuracy on fire occurrence / non-occurence: **1.00** (100%)  

## 📄 License

MIT License — you are free to reuse, extend, or build upon this work.

---

**Scientific Note**:  
This stage focuses only on **binary fire occurrence**. Future stages may expand to **fire spread modeling**, rate prediction, or geographic simulation.---

## 📦 Dataset Acknowledgment

This study is based on the **Algerian Forest Fires Dataset**  
📥 [Available via UCI Repository](https://archive.ics.uci.edu/ml/datasets/Algerian+Forest+Fires+Dataset+)

The dataset includes meteorological and fire data from two regions in Algeria (Sidi-Bel Abbes and Bejaia) between June and September 2012.  
➤ `Cleaned_Algerian_Forest_Fire_Data.csv`

---

## 📖 Citation

If you use this repository or model in academic work:

```
@misc{dewmini2025firestage1,
  title={Physics-Informed Fire Prediction – Stage 1: Fire Occurrence},
  author={Dewmini Gunasekera},
  year={2025},
  note={GitHub repository},
  url={https://github.com/dewminigunasekera/physics-informed-fire-prediction-occurrence}
}
```
