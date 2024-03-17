# deep-learning-challenge
## Alphabet Soup Charity Deep Learning Model Performance Report
## Overview of the Analysis

The purpose of this analysis is to develop a deep learning model to predict the success of funding applications for Alphabet Soup, a fictional philanthropic organization. The model aims to classify funding applications as either successful or unsuccessful based on various input features.

### Results

### Data Preprocessing

#### Variables Removed
* **First Analysis (Notebook 1)**:
  - The `EIN` and `NAME` columns were removed from the input data as they are identifiers and do not provide meaningful predictive information.

* **Second Analysis (Notebook 2)**:
  - In addition to `EIN` and `NAME`, the `STATUS` column was also removed from the input data as it does not contribute to predicting the success of funding applications.

### Compiling, Training, and Evaluating the Model

#### Model Architecture
* **First Analysis (Notebook 1)**:
  - The model architecture consists of two hidden layers with 128 and 64 neurons, respectively, followed by an output layer with a sigmoid activation function.
  - The model was trained for 100 epochs.

* **Second Analysis (Notebook 2)**:
  - The model architecture comprises three hidden layers with 128, 64, and 32 neurons, respectively, followed by an output layer with a sigmoid activation function.
  - Similar to the first analysis, the model was trained for 100 epochs.

#### Model Performance
* **First Analysis (Notebook 1)**:
  - Despite variations in hyperparameters, the model accuracy remained below the target threshold of 75%.

* **Second Analysis (Notebook 2)**:
  - Despite additional hidden layers and neurons, the model accuracy also fell short of the target performance.

#### Attempts to Improve Model Performance
* Various hyperparameters were adjusted, including the number of neurons, hidden layers, activation functions, and epochs.
* Additionally, different preprocessing techniques were explored, such as binning and feature scaling.

## Summary

In both analyses, the deep learning models failed to achieve the target performance of 75% accuracy. The inability to reach the desired accuracy suggests that the predictive power of the features in the dataset may be limited. 

### Recommendation

Given the complexity of the dataset and the challenges encountered in achieving the target performance with deep learning models, an alternative approach using a different machine learning algorithm could be explored. Ensemble methods like Random Forest or Gradient Boosting may offer better performance for this classification problem. These algorithms are less sensitive to feature scaling and may provide more robust predictions, ultimately improving the success rate of funding application predictions for Alphabet Soup.
