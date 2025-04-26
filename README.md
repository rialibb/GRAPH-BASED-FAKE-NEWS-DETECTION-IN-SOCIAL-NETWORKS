# GRAPH-BASED-FAKE-NEWS-DETECTION-IN-SOCIAL-NETWORKS

## 📚 Project Overview

This project was conducted as part of the MLNS Final Project.  
It aims to **detect rumours in Twitter conversations** by modeling discussions as **graph-structured data**.  
We implement and compare two different approaches:
- A **Machine Learning (ML)** pipeline with hand-crafted features and classical classifiers.
- A **Deep Learning (DL)** pipeline using **Graph Neural Networks (GNNs)**.

We systematically explore **data preprocessing**, **feature engineering**, **model design**, **hyperparameter tuning**, and **evaluation** strategies to tackle the rumour detection challenge under **class imbalance**.

---

## 📁 Repository Structure

```
├── ML_Approach.ipynb      # Notebook for the Machine Learning pipeline
├── DL_Approach.ipynb      # Notebook for the Deep Learning (GNN) pipeline
├── README.md              # Project README file
├── report.pdf             # Final report (submitted via GradeScope)
└── requirements.txt       # necessary libraries of the project

```

---

## 📝 Dataset

The dataset used is the **PHEME Rumour Detection Dataset**, which consists of tree-structured Twitter conversations annotated as rumours or non-rumours.

- Public link to download the dataset: [PHEME Dataset on Figshare](https://figshare.com/articles/dataset/PHEME_dataset_for_Rumour_Detection_and_Veracity_Classification/6392078)
- Please refer to the report for detailed data preprocessing steps.

---

## 🧐 Methodology

- **Machine Learning (ML) Pipeline**:
  - Feature extraction (tweet metadata, text embeddings, graph statistics).
  - Feature selection (low variance elimination, correlation-based filtering, multicollinearity reduction).
  - Hyperparameter tuning using **Bayesian Optimization** with **Optuna**.
  - Models tested: Random Forest, Support Vector Machine (SVM), Gradient Boosting.

- **Deep Learning (DL) Pipeline**:
  - Node embeddings using RoBERTa.
  - Graph modeling of conversations.
  - Graph Attention Networks (**GAT**) as classifier.
  - Weighted loss and learning rate scheduling to address class imbalance.

---

## 🚀 How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/rialibb/GRAPH-BASED-FAKE-NEWS-DETECTION-IN-SOCIAL-NETWORKS.git
   cd GRAPH-BASED-FAKE-NEWS-DETECTION-IN-SOCIAL-NETWORKS
   ```

2. **Install required libraries** (recommended: use a virtual environment):

   ```bash
   pip install -r requirements.txt
   ```

3. **Download the dataset** from [this link](https://figshare.com/articles/dataset/PHEME_dataset_for_Rumour_Detection_and_Veracity_Classification/6392078) and place it in the `data/` directory.

4. **Run the notebooks**:

   - For the ML approach: Open and run `ML_Approach.ipynb`
   - For the DL approach: Open and run `DL_Approach.ipynb`

---

## ✨ Acknowledgements

- **PHEME Dataset**: [Zubiaga et al., 2016]
- **Optuna** for Bayesian optimization [Akiba et al., 2019]
- **Graph Attention Networks (GAT)** [Veličković et al., 2018]

---

## 💑 License

This project is for educational purposes only as part of the MLNS course project.

---

# 🔥 Quick Note
If you find the project interesting, feel free to star ⭐ the repository!

