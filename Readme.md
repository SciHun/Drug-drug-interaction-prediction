🧠Predicting Drug Interactions and Side Effects: A Novel ML-Based Approach for New Molecules


I collaborated on this study with my final-term pharmacy students, 👩‍🔬Ayse Meliha Varol and 👩‍🔬Hacer Ince. They actively contributed by writing code, performing data cleaning, and assisting with model assessments using JupyterLab.

This project presents a machine learning-based tool that predicts drug–drug interactions and possible side effects using Morgan fingerprints generated from SMILES representations.

This study also predicts the interactions between any new molecule and existing drugs.

🧪 Dataset
This project is based on a dataset of 125,249 drug pairs, consisting of:

63,473 positive interactions (interaction = 1)

61,776 negative interactions (interaction = 0)

Each row in the dataset represents a pair of drugs (Drug 1 and Drug 2), including:

Their SMILES strings (X1 and X2), A binary interaction label (0 or 1), The associated side effect name and Fingerprints for each drugs (2048 bit)

To prepare the data:

RDKit was used to convert SMILES strings into Morgan fingerprints

These fingerprints were used as features for a LightGBM classification model

After training, the model can predict whether a new molecule is likely to interact with existing drugs — and what side effects may result.

🧪 Features;

Input: SMILES of two molecules

Output: Binary interaction score + predicted side effect

ML Model: LightGBM

Evaluation: Accuracy = 0.86, AUC = 0.955

Feature extraction: RDKit-based Morgan Fingerprints (4096 bits)

📊 Visualizations
ROC Curve and Prediction Distribution

## 💡 Authors
🔬 Harun Un, PhD – Clinical Biochemist & Data Scientist

🔬 Hacer Ince, BSc – Pharmacist

🔬 Ayse Meliha Varol, BSc – Pharmacist
