![Shell image](data/shell.png)
# Deep Learning vs Keypoint: Which Feature Set Is Better for Shell Recognition?

Shells are ubiquitous objects that are both useful to humans and essential for preserving the marine ecosystem. With tens of thousands of species, shells are not easy to identify manually, necessitating automated approaches. Machine learning (ML) and computer vision are two technologies that can be employed to solve the issue. Unfortunately, very few studies have proposed the recognition of shells using these technologies. This paper presents an end-to-end shell species detection pipeline comprising feature extraction and recognition components. We exhaustively investigate various feature extraction methods, including those that use domain knowledge, keypoints, and pretrained deep neural networks. Three classifiers are used to validate the discriminative capabilities of all generated features: support vector machine (SVM), random forest (RF), and feed-forward neural network (FFNN). Using the recently proposed shell dataset, we show that our best model -- SVM trained on pretrained VGG16 features achieved 96% accuracy and macro-average F1, outperforming state-of-the-art models by more than 13% in both metrics.

## Requirements:
- Python 3.6+
- numpy
- scipy
- pandas
- matplotlib
- seaborn
- TensorFlow 2.0
- Scikit-learn 0.22
- opencv-python 

### scripts and notebooks
- jupyter
- tqdm

## Folder Structure:
- *data*: contains the shell dataset
- *notebooks*: contains utilities and experimentation codes.
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

## Acknowledgements:
- The shell dataset is provided by [Zhang et al. (2019)](https://www.nature.com/articles/s41597-019-0230-3).
- I gratefully acknowledge Aylini Town for inspiring me to work on shell recognition task; I would also gratefully thank Dr. Chris Town for continuous help and support.