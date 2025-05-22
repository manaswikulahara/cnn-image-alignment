# 🧠 CNN-Based Image Alignment

This repository contains the code and dataset used for deep learning-based **image alignment** using Convolutional Neural Networks (CNNs). The project replaces traditional SIFT-RANSAC pipelines with a neural network approach, enabling robust image registration for aerial and remote sensing imagery.

---

## 📌 Project Highlights

- 🔁 Geometric transformation learning using CNNs
- 📸 Dataset support with Yong et al.'s image pairs
- ⚙️ End-to-end training and testing pipeline
- 🧪 Jupyter notebooks for data preparation, training, and evaluation
- 📈 CSV outputs to track experiments

---

## 🗂️ Directory Structure

```
cnn-image-alignment/
├── classes/                    # Python helper classes
├── DataSet_Yong.ipynb         # Dataset preparation
├── cnn_geometric.ipynb        # Model architecture and training
├── data_Construct.ipynb       # Data transformation and loading
├── test_train_split.ipynb     # Train-test split creation
├── *.csv                      # Training/testing data splits
├── *.py                       # Supporting Python modules
└── README.md                  # This file
```

---

## 📊 Sample Use Cases

- Aligning satellite or drone images
- Remote sensing change detection preprocessing
- Medical or historical image stitching

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/manaswikulahara/cnn-image-alignment.git
cd cnn-image-alignment
```

### 2. Install required dependencies
```bash
pip install -r requirements.txt
```

### 3. Train the model
```bash
python train.py
```

Or use the Jupyter Notebooks (`*.ipynb`) for interactive execution.

---

## 📁 Datasets

This implementation uses the **Yong et al.** dataset.

Custom CSVs are used for loading paired images:
- `train_yong.csv`
- `test_yong.csv`

Each CSV contains paths to paired input images for alignment tasks.

---

## 🧠 Model Details

The CNN model learns to estimate transformation parameters such as affine or thin plate spline (TPS) directly from input image pairs.

### 🔧 Core Modules:
- `point_tnf.py` – Thin Plate Spline transformer
- `loss.py` – Alignment loss functions
- `cnn_geometric_model_yong.py` – Model backbone

---

## ✍️ Author

**Manaswi Kulahara**  
*M.Sc. Geoinformatics*  
🔗 [GitHub Profile](https://github.com/manaswikulahara)

---

## 📄 License

This project is intended for educational and research purposes.  
Please add a LICENSE file to define official usage rights.

---

## 📚 Reference

Yong et al.,  
*"Learning Feature Transformations with CNNs for Image Alignment"*  

---
