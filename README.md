
# Number Recognition using Random Forest Classifier

This project demonstrates the process of optical recognition of handwritten digits using the popular Random Forest Classifier from scikit-learn. The dataset used for this project is the **Optical Recognition of Handwritten Digits Dataset** from the UCI Machine Learning Repository.

## Dataset Description

- **Number of Instances:** 1797
- **Number of Attributes:** 64 (8x8 pixel images)
- **Attribute Information:** Each attribute represents an integer pixel value ranging from 0 to 16.
- **Missing Attribute Values:** None
- **Source:** [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/Optical+Recognition+of+Handwritten+Digits)

## Project Overview

The dataset consists of images of handwritten digits (0-9). The goal is to build a machine learning model that can accurately recognize and classify these digits. The workflow includes:

1. **Data Preprocessing:** 
   - Normalizing pixel values.
   - Splitting the data into training and testing sets.
     

2. **Model Training:**
   - Implemented using `RandomForestClassifier` with `max_depth=128` and `n_estimators=256`.

3. **Evaluation Metrics:**
   - Accuracy
   - Precision
   - Recall
   - Confusion Matrix

## Results

- **Training Accuracy:** 1.0
- **Test Accuracy:** 97.22%
- **Precision Score:** 97.31%
- **Recall Score:** 97.22%

### Confusion Matrix:
|   | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
|---|---|---|---|---|---|---|---|---|---|---|
| 0 | 39| 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 28| 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 2 | 1 | 0 | 38| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 3 | 0 | 0 | 0 | 39| 0 | 0 | 0 | 0 | 0 | 0 |
| 4 | 0 | 0 | 0 | 0 | 34| 0 | 0 | 0 | 0 | 1 |
| 5 | 0 | 0 | 0 | 0 | 0 | 37| 1 | 0 | 0 | 0 |
| 6 | 0 | 0 | 0 | 0 | 0 | 0 | 35| 0 | 0 | 0 |
| 7 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 40| 0 | 1 |
| 8 | 0 | 2 | 1 | 0 | 0 | 0 | 0 | 0 | 30| 1 |
| 9 | 0 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 30|

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/number_recognition.git
   cd number_recognition
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook number_recognition.ipynb
   ```

## Dependencies

- Python 3.x
- scikit-learn
- matplotlib
- numpy
- pandas
- jupyter

## License

This project is licensed under the MIT License.

## Acknowledgments

- **UCI Machine Learning Repository** for providing the dataset.
- **scikit-learn** for the machine learning tools used in this project.
