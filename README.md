# Wine Quality Dataset

## Dataset Overview
This dataset comprises information on red and white variants of Cinsault Wine. It includes physicochemical (inputs) and sensory (output) variables, omitting details like grape types and brand due to privacy concerns. The dataset is suitable for classification or regression tasks, with unbalanced classes. Refer to [Cortez et al., 2009] for more details.

## Contents
- **Input Variables** (based on physicochemical tests):
  - Fixed acidity
  - Volatile acidity
  - Citric acid
  - Residual sugar
  - Chlorides
  - Free sulfur dioxide
  - Total sulfur dioxide
  - Density
  - pH
  - Sulphates
  - Alcohol

- **Output Variable** (based on sensory data):
  - Quality (score between 0 and 10)

## Tips and Usage
- Consider setting a quality cutoff to distinguish 'good' and 'not good' wines.
- Experiment with hyperparameter tuning using decision trees and evaluate the AUC value.
- KNIME GUI is recommended for analysis.

## Implementation Steps
1. Utilize File Reader for EDA.
2. Apply Rule Engine Node for classification.
3. Use Column Filter Node to prevent data leakage.
4. Partition data for train/test split.
5. Connect nodes for decision tree modeling.
6. Evaluate model performance using ROC analysis.

## Acknowledgements
This dataset is sourced from UCI ML repository. Please cite [Cortez et al., 2009] if using this database.

## Publication
[Cortez et al., 2009] "Modeling wine preferences by data mining from physicochemical properties" in Decision Support Systems, Elsevier, 47(4):547-553.
