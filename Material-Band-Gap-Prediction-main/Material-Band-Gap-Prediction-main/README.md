# Band Gap Prediction for Compounds using Machine Learning Models

## Overview:
This project focuses on predicting the band gap of various compounds. The band gap refers to the energy difference between the top of the valence band and the bottom of the conduction band, which is a crucial property in materials science. The objective is to employ different machine learning models to make these predictions and subsequently compare their performances.

## Background:
The band gap is inversely proportional to the square root of the dielectric constant. This dielectric constant is influenced by several factors:
- Polarizability of atoms
- Atomic structure
- Density of atoms

**Typical band gap ranges for materials are:**
- Conductors: 0-2 eV
- Semiconductors: 2-3 eV
- Insulators: 3-4 eV


## Data:
The dataset, sourced from **Matminer** (an open-source Python library for material science datasets), comprises approximately 1100 different compounds. Data preprocessing steps involved the removal of certain features, encoding specific columns, and restructuring the dataset for optimal compatibility with ML models.

## Machine Learning Models and Results:
The project utilized multiple machine learning models:
- SVM
- Decision Tree
- K Nearest Neighbors (KNN)
- Random Forest
- Gradient Boosting

Among these, Gradient Boosting and Random Forest consistently outperformed others. Notably, SVM and KNN's performances were significantly influenced by the scaling of input features. After hyperparameter tuning, the Gradient Boosting model achieved the best R2 score of 0.8142, showcasing its potential in the prediction of material properties.

## Evaluation Metrics:
Two primary metrics were employed to assess model performance:
- **Mean Absolute Error (MAE)**
- **R2 Score**

## Future Directions:
Further optimizations and the inclusion of more diverse datasets can potentially enhance the accuracy of predictions. Special attention can be given to models like SVM and KNN, especially concerning the scaling of input features.

## References:
- [Band Gap Theory](https://en.wikipedia.org/wiki/Band_gap)
- [Matminer Dataset](https://hackingmaterials.lbl.gov/matminer/dataset_summary.html)
- [SciKit Learn](https://scikit-learn.org/)
- Other tools utilized: Pandas, Numpy, Matplotlib.
