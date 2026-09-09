# Research AI/ML Projects

A collection of interdisciplinary research projects combining **Bioinformatics, Artificial Intelligence, Machine Learning, Computational Biology, Computational Drug Discovery, and Medical Image Analysis**.

This repository contains three research projects that apply computational and AI/ML approaches to biomedical problems involving **cancer genomics, therapeutic compound discovery, and medical imaging**.

---

## Projects

### 1. T-Cell Functional State Prediction in Chronic Lymphocytic Leukemia Using StarCAT

#### Overview

This project focuses on the computational analysis of **T-cell functional states in Chronic Lymphocytic Leukemia (CLL)** using single-cell RNA sequencing (scRNA-seq) data.

**StarCAT** is used as a computational cell-state annotation tool to characterize T-cell functional programs and investigate differences in cellular states across disease conditions and treatment-related timepoints.

The analysis provides insights into T-cell functional heterogeneity within a hematological malignancy and can support further research in cancer immunology, therapeutic response, and cancer treatment strategies.

#### Objectives

- Identify and characterize T-cell populations in CLL.
- Predict T-cell functional states using StarCAT.
- Characterize functional programs associated with T-cell populations.
- Compare T-cell states between sensitive and resistant conditions.
- Investigate changes between pre-treatment and post-treatment samples.
- Explore T-cell functional heterogeneity in CLL.
- Generate interpretable cell-state profiles for downstream analysis.

#### Dataset

| Feature | Value |
|---|---:|
| Total genes | 19,105 |
| Total cells | 24,790 |
| Patients | 4 |
| T cells identified | 6,588 |
| CD8+ T cells | 5,006 |
| CD4+ T cells | 1,582 |
| Conditions | Sensitive, Resistant |
| Timepoints | Pre-treatment, Post-treatment |

After metadata harmonization and removal of unmatched cells, **6,584 cells** were used for downstream StarCAT analysis.

#### Workflow

```text
CLL scRNA-seq Dataset
        ↓
Preprocessing & Quality Control
        ↓
T-Cell Identification
        ↓
T-Cell Subset Analysis
        ↓
StarCAT Cell-State Annotation
        ↓
Functional Program Analysis
        ↓
Condition & Timepoint Comparison
        ↓
Visualization
        ↓
Biological Interpretation
````

#### Tools & Technologies

* Python
* Google Colab
* Scanpy
* AnnData
* StarCAT
* Single-Cell RNA Sequencing
* Data Visualization
* Computational Immunology

#### Significance

T-cell functional-state analysis can provide insights into **tumor–immune interactions, treatment response, and treatment resistance** in CLL.

This project demonstrates the application of single-cell computational approaches to investigate immune-cell heterogeneity in hematological malignancies and support future research in **cancer immunology and therapeutic development**.

---

## 2. In-Silico Analysis of Phytochemicals Targeting Common Molecular Mechanisms of Type 2 Diabetes and Alzheimer's Disease

### Overview

This project investigates the molecular association between **Type 2 Diabetes Mellitus (T2DM)** and **Alzheimer's Disease (AD)** by exploring shared molecular mechanisms and potential therapeutic targets.

The study focuses on the computational evaluation of **phytochemicals** that may have potential against disease-associated molecular targets.

An integrated computational drug-discovery workflow was developed using **QSAR modeling, molecular descriptors, Morgan fingerprints, machine learning, applicability domain analysis, and molecular docking**.

### Objectives

* Investigate shared molecular mechanisms between T2DM and Alzheimer's disease.
* Identify potential common therapeutic targets.
* Identify and characterize relevant phytochemicals.
* Develop QSAR models for biological activity prediction.
* Apply machine-learning algorithms to molecular data.
* Evaluate model performance.
* Apply applicability domain analysis to assess prediction reliability.
* Prioritize promising phytochemical candidates.
* Perform molecular docking for further computational investigation.

### Computational Workflow

```text
Literature & Target Identification
        ↓
Phytochemical Identification
        ↓
Dataset Collection & Preprocessing
        ↓
Molecular Descriptor Generation
        ↓
Morgan Fingerprint Generation
        ↓
QSAR Model Development
        ↓
Machine Learning
        ↓
Model Evaluation
        ↓
Applicability Domain Analysis
        ↓
Compound Prioritization
        ↓
Molecular Docking
```

### QSAR Dataset

A TNF-associated experimental dataset containing **907 compounds** was used for QSAR model development.

| Parameter                |   Value |
| ------------------------ | ------: |
| Total compounds          |     907 |
| Training compounds       |     725 |
| Test compounds           |     182 |
| Training : Testing Ratio | 80 : 20 |
| Target Variable          |   pIC50 |
| Missing Values           |       0 |
| Duplicate SMILES         |       0 |
| Mean pIC50               |   5.856 |
| Standard Deviation       |   1.109 |
| Minimum pIC50            |   1.686 |
| Maximum pIC50            |   9.523 |

### Molecular Representation

Molecular structures were represented using molecular descriptors and **Morgan fingerprints** generated from SMILES structures.

Morgan fingerprints provide numerical representations of molecular structures that can be used as input features for machine-learning-based QSAR models.

### Machine Learning Models

The following machine-learning algorithms were explored:

* Random Forest
* Support Vector Machine (SVM)
* XGBoost

### Applicability Domain Analysis

Applicability Domain (AD) analysis was incorporated to determine whether predicted compounds fall within the chemical space represented by the training dataset.

This provides an additional assessment of the reliability of model predictions for candidate compounds.

### Molecular Docking

Prioritized phytochemical candidates were further investigated through molecular docking to explore potential interactions with selected molecular targets.

Docking analysis can provide insights into:

* Protein–ligand interactions
* Binding poses
* Hydrogen-bond interactions
* Hydrophobic interactions
* Predicted binding affinity

### Recognition

This research was presented as a **poster at an international conference at Sharda University**, where it secured **1st position among 120+ participants**.

### Tools & Technologies

* Python
* Google Colab
* Machine Learning
* QSAR
* Cheminformatics
* Molecular Descriptors
* Morgan Fingerprints
* Applicability Domain Analysis
* Molecular Docking
* Computational Drug Discovery
* Bioinformatics

### Significance

This project explores a computational strategy for investigating shared biological mechanisms between metabolic and neurodegenerative disease and for prioritizing **plant-derived compounds** for further computational and experimental investigation.

---

## 3. Multi-Class Skin Cancer Classification Using CNN and Transfer Learning

### Overview

This project focuses on the development of a **deep learning-based image classification system** for automated classification of skin cancer.

The system uses **Convolutional Neural Networks (CNNs)** and **Transfer Learning** to classify skin lesion images into **seven different classes of skin cancer**.

The project demonstrates the application of Artificial Intelligence, Deep Learning, Computer Vision, and Medical Image Processing to cancer classification.

### Objectives

* Develop an automated skin lesion image-classification pipeline.
* Classify images into seven different skin cancer classes.
* Apply CNN-based deep-learning techniques.
* Implement transfer learning using pretrained architectures.
* Train and evaluate deep-learning models.
* Analyze model performance using appropriate classification metrics.
* Explore AI-based approaches for computer-aided skin lesion analysis.

### Workflow

```text
Skin Lesion Image Dataset
        ↓
Image Preprocessing
        ↓
Image Resizing
        ↓
Normalization
        ↓
Data Augmentation
        ↓
CNN / Transfer Learning
        ↓
Model Training
        ↓
Validation & Testing
        ↓
Performance Evaluation
        ↓
Seven-Class Classification
```

### Deep Learning Approach

#### Convolutional Neural Networks

CNNs can automatically learn meaningful visual features from medical images.

The network learns hierarchical features such as:

* Edges
* Textures
* Shapes
* Patterns
* Higher-level visual characteristics

#### Transfer Learning

Transfer learning was used to leverage pretrained deep-learning architectures and adapt their learned feature representations to the skin cancer classification task.

### Model Evaluation

The classification models can be evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* Class-wise Performance

### Significance

Automated skin lesion analysis is an important application of Artificial Intelligence in healthcare.

This project demonstrates how **CNNs and transfer learning can be applied to multi-class skin cancer image classification**, providing a foundation for further research in **medical imaging and AI-assisted healthcare**.

> **Disclaimer:** This project is intended for academic and research purposes and should not be considered a standalone clinical diagnostic system.

### Tools & Technologies

* Python
* Google Colab
* TensorFlow
* Keras
* Convolutional Neural Networks
* Transfer Learning
* Deep Learning
* Computer Vision
* Image Processing
* Medical Image Analysis

---

# Technical Skills Demonstrated

### Bioinformatics & Computational Biology

* Single-Cell RNA-seq Analysis
* T-Cell Functional-State Analysis
* Cell-State Annotation
* Cancer Bioinformatics
* Computational Immunology
* Data Analysis
* Data Visualization

### Artificial Intelligence & Machine Learning

* Machine Learning
* Deep Learning
* CNN
* Transfer Learning
* Classification
* Predictive Modeling
* Model Evaluation

### Computational Drug Discovery

* QSAR Modeling
* Molecular Descriptors
* Morgan Fingerprints
* Applicability Domain Analysis
* Molecular Docking
* Cheminformatics
* Phytochemical Analysis

### Medical AI

* Medical Image Processing
* Computer Vision
* Multi-Class Classification
* Skin Cancer Classification
* Deep-Learning-Based Image Analysis

---

# Technologies & Tools

```text
Python
Google Colab
Scanpy
AnnData
StarCAT
Scikit-learn
XGBoost
TensorFlow
Keras
QSAR
Morgan Fingerprints
Molecular Docking
Computer Vision
Deep Learning
Single-Cell RNA-seq
```

---

# Repository Structure

```text
Research-AI-ML-Projects/
│
├── 01_CLL_TCell_State_Analysis/
│   └── CLL_TCell_StarCAT_Analysis.ipynb
│
├── 02_AD_T2DM_Phytochemical_QSAR/
│   └── AD_T2DM_Phytochemical_QSAR.ipynb
│
├── 03_Skin_Cancer_CNN/
│   └── Skin_Cancer_Classification.ipynb
│
└── README.md
```

---

# Project Summary

| Project                            | Domain                       | Data Type      | Main Approach           |
| ---------------------------------- | ---------------------------- | -------------- | ----------------------- |
| T-Cell Functional State Prediction | Cancer Bioinformatics        | scRNA-seq      | StarCAT                 |
| AD–T2DM Phytochemical Analysis     | Computational Drug Discovery | Molecular Data | QSAR + ML + Docking     |
| Skin Cancer Classification         | Medical AI                   | Medical Images | CNN + Transfer Learning |

---

# Research Focus

These projects collectively demonstrate the application of **AI and computational methods across multiple areas of biomedical research**:

```text
Single-Cell Genomics
        ↓
Cancer & Immune-Cell Analysis
        ↓
Computational Drug Discovery
        ↓
Machine Learning & QSAR
        ↓
Medical Image Analysis
        ↓
Deep Learning & AI
```

The overall portfolio integrates:

**Bioinformatics + AI/ML + Computational Biology + Drug Discovery + Medical AI**

---

# Future Directions

Potential future extensions include:

* Advanced single-cell and multi-omics analysis.
* Integration of additional clinical and molecular datasets.
* External validation of QSAR predictions.
* Extended molecular docking and molecular dynamics simulations.
* Experimental validation of prioritized phytochemicals.
* Model explainability and optimization for deep-learning approaches.
* External validation of skin cancer classification models.
* Development of interactive AI-based research applications.
* Integration of multimodal biomedical datasets.

---

# Author

**Khushi Sharma**

B.Tech Bioinformatics
IILM University

---

# Disclaimer

All projects in this repository are developed for **academic, educational, and research purposes**.

Computational predictions, machine-learning outputs, and AI-based classifications require appropriate **experimental, external, or clinical validation** before being considered for real-world therapeutic or diagnostic applications.

```
```
