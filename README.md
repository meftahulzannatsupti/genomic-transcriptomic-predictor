# 🧬 Gene Expression Prediction Using Deep Learning

This project investigates the prediction of gene expression levels using advanced deep learning models, focusing on genomics applications. We compare the performance of **Deep Neural Networks (DNN)**, **Long Short-Term Memory (LSTM)** networks, and **Gated Recurrent Units (GRU)**, with a special emphasis on **attention-enhanced architectures**.

---

## 📊 Project Summary

- **Objective:** Predict gene expression values using a dataset of the top 50 most variable genes.
- **Models Used:**  
  - Deep Neural Network (DNN)  
  - Long Short-Term Memory (LSTM)  
  - Gated Recurrent Units (GRU)  
  - Attention-based LSTM and GRU variants
- **Evaluation Metrics:** MAE, RMSE, MSE, R²  
- **Best Model:** Attention-LSTM  
  - RMSE: **0.0107**, MAE: **0.0078** for single target genes  
  - RMSE: **0.1651**, MAE: **0.1040** for top 50 genes

---

## 🧠 Deep Learning Architecture Overview

- **DNN** was constructed using multiple dense layers with ReLU activations, enabling the model to learn complex nonlinear relationships.
- **LSTM** and **GRU** were applied despite the dataset being non-temporal, to capture latent temporal-like dependencies in gene interactions.
- **Attention Mechanism** was integrated into the LSTM and GRU models to focus on the most critical gene features, significantly improving prediction performance.

---

## 🛠️ Techniques & Methods

- Dimensionality Reduction  
- Feature Selection (Top 50 most variable genes by variance)  
- Model Evaluation via Cross-Validation  
- Custom Attention Layer Implementation in TensorFlow/Keras  
- Error Analysis using MAE, RMSE, and R²

---

## 📁 Files

- `gene_expression_predictor.ipynb` — Model training, evaluation, and visualization
- `README.md` — Project documentation
- `requirements.txt` — Required libraries and versions (TensorFlow, NumPy, etc.)

---

## 🧪 Results

| Model         | RMSE (Top 50) | MAE (Top 50) | RMSE (Single) | MAE (Single) | R² |
|---------------|---------------|---------------|----------------|----------------|----|
| DNN           | > 0.20        | > 0.15        | -              | -              | -  |
| GRU           | 0.22          | 0.13          | -              | -              | -  |
| **LSTM + Attention** | **0.1651**      | **0.1040**      | **0.0107**       | **0.0078**       | **~0.999** |

The **attention-enhanced LSTM** clearly outperformed the others in both single-target and multi-gene prediction tasks.

---

## 🧬 Applications

- **Genomics & Transcriptomics**  
- **Drug Discovery**  
- **Personalized Medicine**  
- **Gene Editing Simulations**

---

## 👤 Author

**Meftahul Zannat**  
MSc AI & Data Science — University of Hull  
📧 [meftahulzannat3598@gmail.com](mailto:meftahulzannat3598@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/meftahul-zannat-susupti98)  
🔗 [GitHub](https://github.com/meftahulzannatsupti)

---

## 📌 Notes

- This project is academic and exploratory; further improvements could include hyperparameter tuning, larger datasets, and deployment via Streamlit or Flask.
