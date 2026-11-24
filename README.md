# 🚀 Deep Learning Course & Practical Experiments

Welcome to my **Deep Learning Course** repository! This repository documents my step-by-step learning journey—ranging from foundational data processing and custom neural network math from scratch to an advanced Explainable AI (XAI) capstone project.

---

## 📂 What's Inside This Repository?

Here is a structured overview of all the files and projects included in this repository:

---

### 1. 🧠 `ANN_Architecture (1).ipynb` (Neural Network Built from Scratch)

> 🎯 **Goal:** Build a complete multi-layer neural network using **only pure NumPy**—without using TensorFlow, Keras, or PyTorch for any core mathematical operations!

* **Data Preprocessing:** Loaded and cleaned `online_shopping.csv`, manually converting categorical variables (`Month`, `VisitorType`, `Weekend`) via One-Hot Encoding for model compatibility.
* **Network Architecture:** Constructed a 3-layer feedforward network:
  $$\text{Input Layer} \longrightarrow \text{Hidden Layer 1 (24 neurons)} \longrightarrow \text{Hidden Layer 2 (12 neurons)} \longrightarrow \text{Output Layer (1 neuron)}$$
* **9 Experimental Setups:** Evaluated performance by systematically testing combinations of:
  * **Optimizers:** Batch Gradient Descent, Mini-Batch ($Batch\_Size = 64$), and Stochastic Gradient Descent (SGD).
  * **Activation Functions:** ReLU, Tanh, and Sigmoid (with `np.clip` bounds for numerical stability against overflow).
* **Automated Summary:** Automatically formats evaluation metrics into a summary table that bolds and highlights the top-performing setup with a green background.

---

### 2. 📊 `online_shopping.csv` (Dataset)
* **Description:** A clean dataset containing **12,330 rows** of online customer session activities.
* **Usage:** Serves as the benchmark dataset for training the custom ANN model to predict binary purchasing intent (`Revenue = True/False`).

---

### 3. 🔢 `NumPy.ipynb` (Mathematical Foundations)
* **Description:** Exercises covering N-dimensional array manipulations, matrix operations, slicing, and vectorization.
* **Usage:** Forms the mathematical baseline required for writing custom forward/backward propagation algorithms.

---

### 4. 🐼 `Pandas.ipynb` (Data Wrangling)
* **Description:** Practice code for reading datasets, performing exploratory data analysis (EDA), cleaning data, and handling missing values.

---

### 5. 🤖 `Sci_kit_Learn.ipynb` (Machine Learning Tools)
* **Description:** ML utility scripts focusing on standard feature scaling, label encoding, and dataset train-test splitting.

---

### 6. ⚡ `tensorflow.ipynb` (Framework Introduction)
* **Description:** Introductory experiments building standard deep neural network layers using High-Level APIs (TensorFlow & Keras).

---

### 7. 🧩 Capstone Project: Explainable AI-Driven Facial ASD Detection

Located in the [`/Project`](./Project) directory, this capstone study introduces an Explainable AI (XAI) clinical decision support framework to screen Autism Spectrum Disorder (ASD) in children using facial images.

* **Unified Benchmark:** Evaluated 6 deep learning architectures (4 CNNs & 2 Vision Transformers) under a standardized experimental protocol.
* **Dual-XAI Integration:** Applied **Grad-CAM** (focal class-dependent visual features) and **Eigen-CAM** (broad class-independent activation structures) to interpret predictions and address the deep network "black-box" challenge.
* **Top Performance:** **EfficientNet-B0** and **DenseNet121** tied for the highest test accuracy (**96.61%**) and F1-Score (**96.60%**). **ResNet50** achieved the highest recall at **97.17%**.

#### 📊 Dataset Reference
* **Dataset:** Autism Facial Image Dataset
* **Dataset Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/ronakp004/autism-spectrum-detection-from-kaggle-zenodo?select=ASD+Facial+Image+Dataset+Combined)

#### 📁 Main Project Artifacts (`/Project`)
* [`Deep_Learning_ModelTraining.ipynb`](./Project/Deep_Learning_ModelTraining.ipynb) — Model training, testing, and XAI heatmap visualizer pipeline.
* [`DL_proposal.pdf`](./Project/DL_proposal.pdf) — Formal project proposal.
* [`DL_report.pdf`](./Project/DL_report.pdf) — Full academic research report.
* [`DL_ASD_slide.pptx`](./Project/DL_ASD_slide.pptx) — Presentation slides.
* [`DL_project_latex.zip`](./Project/DL_project_latex.zip) — LaTeX source code for report and documentation.

---

## 🧠 Key Highlights of Fundamental Experiments

* **Built from Scratch:** Formulated all linear algebra computations—Forward Propagation, Loss Calculation, Backpropagation (Chain Rule), and Weight Updates—manually via `np.dot`.
* **Numerical Safety:** Integrated safety bounds (`np.clip`) to eliminate numerical errors (e.g., overflow/underflow in exponential functions).
* **Comparative Insights:** Benchmarked convergence dynamics and cost reduction rates across Batch, Mini-Batch, and SGD optimizers.

---

## 🛠️ Tech Stack & Ecosystem

| Domain | Technologies Used |
| :--- | :--- |
| **Languages** | Python 3 |
| **Deep Learning Frameworks** | PyTorch, TensorFlow, Keras |
| **Computer Vision & XAI** | OpenCV, MTCNN, Grad-CAM, Eigen-CAM |
| **Data Science & ML** | NumPy, Pandas, Scikit-Learn, Matplotlib, Seaborn |
| **Environments** | Google Colab, Jupyter Notebook |

---

## 👤 Author (Fundamental Experiments)

- **Mst. Tanzina Islam**

---

## 👥 Capstone Project Authors & Supervision

- **Mst. Tanzina Islam** 
- **Afifa Islam Chy Sabiha** 
- **Department:** Department of Computer Science & Engineering, North East University Bangladesh (NEUB)
- **Supervised By:** Mr. Razorshi Prozzwal Talukder, Lecturer, Department of CSE, NEUB
