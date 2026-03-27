
# MNIST Digit Classification: From Perceptrons to CNNs

This repository contains a comprehensive end-to-end Deep Learning workflow for handwritten digit recognition using the classic **MNIST dataset**. The project explores the evolution of neural network architectures, comparing the performance of a simple Perceptron, a Multi-Layer Perceptron (ANN), and a Convolutional Neural Network (CNN).

## 🚀 Project Overview

The goal of this project is to demonstrate data preprocessing, model architectural design, and comparative evaluation in a supervised learning environment. 

### Key Features:
* **Data Pipeline:** Full preprocessing workflow including normalization, reshaping, and one-hot encoding.
* **Architectural Comparison:** Implementation of three distinct models to solve the same classification task.
* **Visualization:** Detailed plotting of training history (Loss/Accuracy) and comparative performance metrics.
* **Evaluation:** Analysis via Confusion Matrices and visual prediction checks.

---

## 📊 Dataset Details
The **MNIST** (Modified National Institute of Standards and Technology) dataset consists of 70,000 grayscale images of handwritten digits (0-9).
link of DATASET  - "https://www.kaggle.com/datasets/oddrationale/mnist-in-csv"
* **Training Set:** `mnist_train.csv`
* **Test Set:** `mnist_test.csv`
* **Resolution:** 28x28 pixels
* **Preprocessing:** Pixel values normalized to $[0, 1]$ by dividing by 255.0.

---

## 🧠 Model Architectures

We evaluate three different neural network designs:

| Model | Input Shape | Description |
| :--- | :--- | :--- |
| **Perceptron** | (784,) | A single-layer linear classifier. |
| **ANN** | (28, 28) | A Multi-Layer Perceptron with hidden dense layers and ReLU activation. |
| **CNN** | (28, 28, 1) | A deep network utilizing Convolutional and Pooling layers for spatial feature extraction. |

---

## 📈 Performance & Results

Each model was trained for **5 epochs**. The results highlight the significant advantage of spatial feature extraction in CNNs compared to flattened inputs in traditional ANNs.

### Visualizations Included:
* **Training History:** Epoch-wise Loss and Accuracy curves for each model.
* **Accuracy Comparison:** A final bar chart comparing the test accuracy of all three architectures.
* **Confusion Matrix:** A detailed breakdown of the CNN's classification performance across all 10 digits.
* **Prediction Gallery:** A side-by-side visual comparison of model predictions on sample test images.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** * `TensorFlow/Keras` (Model Building)
    * `Pandas/NumPy` (Data Manipulation)
    * `Matplotlib/Seaborn` (Data Visualization)
    * `Scikit-Learn` (Metrics & Evaluation)

---

## 📂 Project Structure
```text
├── data/               # MNIST CSV files 
├── notebooks/          # Jupyter Notebook with full implementation
├── README.md           # Project documentation
└── requirements.txt    # List of dependencies
```

---

## 🏃 How to Run
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/mnist-digit-classification.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Open the Notebook:**
    Launch `jupyter notebook` and run the cells to see the training process and visualizations.
