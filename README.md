# Intrusion Detection with PSO-Tuned Deep Learning Models

**Authors:** Mahima Chowdary Mannava & Rikhila Reddy Annem  
**Course:** CS258 – Computer Communication Systems  

## Project Overview  
Modern networks face evolving cyberattacks that rule-based IDS miss. This project implements an end-to-end ML pipeline on NSL-KDD (125,973 train / 22,544 test samples) to detect five attack categories. We compare classical ML, a hybrid CNN–LSTM, and two PSO-tuned deep-learning models (1D-CNN, plain LSTM).

## Installation  
bash
git clone https://github.com/your-username/ps-intrusion-detection.git
cd ps-intrusion-detection
python3 -m venv venv
source venv/bin/activate       # Windows: venv\Scripts\activate
pip install -r requirements.txt

## Data Preparation
* Mapping: 39 fine-grained attacks → 5 categories (DoS, Probe, R2L, U2R, Normal)

* Encoding: LabelEncode categorical features; one-hot encode targets

* Balancing: SMOTE to oversample minority classes


The models used for this task are:

* Random Forest

* HistGradientBoostingClassifier

* Logistic Regression

* 1D Convolutional Neural Network (1D-CNN)

* CNN–LSTM Hybrid

* PSO-Optimized 1D-CNN

* PSO-Optimized LSTM

## Key Results

| Model                         | Test Accuracy |
|-------------------------------|--------------:|
| Random Forest                 |         0.91  |
| HistGradientBoostingClassifier|         0.92  |
| Logistic Regression           |         0.86  |
| **PSO-Optimized 1D-CNN**      |         0.76  |
| **PSO-Optimized LSTM**        |         0.83  |
| **CNN–LSTM Hybrid**           |         0.83  |
| **Best (AE-MLP / Ensemble)**  |        0.88+  |

