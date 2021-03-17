# Comparing Standard, Keypoint and Deep Learning Features for Shell Recognition

This project aims to compare the discriminative capabilities of standard features using domain knowledge, keypoint features obtained using traditional computer vision techniques, and feature representations derived from pre-trained deep learning models. We trained support vector machine (SVM), random forest (RF), and feed-forward neural network (FFNN) and evaluate it using nested cross-validation using the aforementioned feature sets for evaluation.

**Note**:
- The shell dataset is provided by [Zhang et al. (2019)](https://www.nature.com/articles/s41597-019-0230-3).
- I gratefully acknowledge Aylini Town for inspiring me to work on shell recognition task; I would also gratefully thank Dr. Chris Town for continuous help and support.


## Requirements:
- Python 3.6+
- numpy
- scipy
- pandas
- matplotlib
- TensorFlow 2.0
- Scikit-learn 0.22
- opencv-python 4.5.1.48

### scripts and notebooks
- jupyter
- tqdm

## Folder Structure:
- *data*: contains the shell dataset
- *notebooks*: contains utilities and experiment codes.
- *results*: contains experiments results (in csv and pickle), including
 the extracted features.

## Setup:
```bash
git clone https://github.com/maleakhiw/shell-feature-extraction.git
cd shell-feature-extraction
pip install -r requirements.txt
pip install .
```

 ## Author:
- Maleakhi Wijaya: maw219@cam.ac.uk