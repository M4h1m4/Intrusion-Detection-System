# Intrusion Detection with PSO-Tuned Deep Learning Models

**Authors:** Mahima Chowdary Mannava & Rikhila Reddy Annem  
**Course:** CS258 – Computer Communication Systems  

## Project Overview  
Modern networks face evolving cyberattacks that rule-based IDS miss. This project implements an end-to-end deep learning pipeline on NSL-KDD (125,973 train / 22,544 test samples) to detect five attack categories. We compare a hybrid CNN–LSTM, and two PSO-tuned deep-learning models (1D-CNN, plain LSTM).


## Data Preparation
* Mapping: 39 fine-grained attacks → 5 categories (DoS, Probe, R2L, U2R, Normal)

* Encoding: LabelEncode categorical features; one-hot encode targets

* Balancing: SMOTE to oversample minority classes


The models used for this task are:


* CNN–LSTM Hybrid

* PSO-Optimized 1D-CNN

* PSO-Optimized LSTM

## Key Results

| Model                         | Test Accuracy |
|-------------------------------|--------------:|
| **PSO-Optimized 1D-CNN**      |         0.76  |
| **PSO-Optimized LSTM**        |         0.83  |
| **CNN–LSTM Hybrid**           |         0.83  | |

