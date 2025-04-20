# 🔥 Fire Propagation Stage 1 – Project Summary

## 📌 Title

**Fulfilling the Initial Spread Index: A Physically-Informed Model for Predicting Fire Occurrence Using Latent Cluster Structure and Correlation Dynamics**

## 📄 Abstract

This project investigates the mechanisms of forest fire occurrence using a physics-aligned machine learning approach. By leveraging physical variables such as ISI, FFMC, DMC, DC, and derived fire indices like BUI and FWI, we construct a neural network that respects the principles of fire propagation.

The model introduces two latent dimensions—**Positive_Cluster** and **Negative_Cluster**—generated through unsupervised KMeans clustering. These clusters represent aggregated fire-spread accelerators and suppressors. Variables are filtered based on their correlation to fire occurrence (|r| > 0.3), and the model is trained on this reduced feature set for better interpretability and physical alignment.

Experiments show that on structured datasets like the Algerian fire dataset, the model achieves **perfect classification (1.00 precision/recall)**. When applied to the UCI Cleaned_Algerian_Forest_Fire_Data.csv dataset, the model maintains high fire recall despite noisier inputs, underscoring the importance of structural physical data in fire modeling.

## ✅ Conclusion

The presented architecture successfully fulfills and extends the utility of the Initial Spread Index (ISI) by embedding it within a physically interpretable neural framework. The model proves that fire occurrence can be accurately predicted when physical variables and latent propagation structure are respected.

- **Scientific relevance**: Demonstrates how real-world operational metrics like ISI can be completed and clarified through machine learning.
- **Practical value**: Offers high recall fire detection in structured environments and resilient early-warning behavior in low-structure data.
- **Next steps**: Extend modeling to simulate multi-stage propagation and fire spread rate based on geographic and temporal features.

This work sets the stage for physically honest fire modeling using interpretable machine learning.