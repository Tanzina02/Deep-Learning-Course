# Deep Learning Course & Practical Experiments 🚀

Welcome to my **Deep Learning Course** repository! This repository contains my step-by-step practice code, datasets, and a complete **Artificial Neural Network (ANN) built completely from scratch using NumPy** for binary classification.

---

## 📂 What's Inside This Repository? (File Breakdown)

Here is a simple overview of all the files and folders in this project:

### 1. `ANN_Architecture (1).ipynb` (Main Deep Learning Project)
* **What it is:** A complete multi-layer neural network built from scratch using pure `NumPy` (without using TensorFlow or Keras for the core math).
* **What I did here:**
  * **Data Preparation:** Loaded the `online_shopping.csv` dataset, cleaned it, and did manual One-Hot Encoding on text columns (`Month`, `VisitorType`, `Weekend`) while keeping numerical columns as they are.
  * **Model Design:** Built a 3-layer neural network (Input $\rightarrow$ Hidden Layer 1 with 24 neurons $\rightarrow$ Hidden Layer 2 with 12 neurons $\rightarrow$ Output Layer with 1 neuron).
  * **9 Combinations Testing:** Tested the model using **9 different setups** by combining:
    * **Optimizers:** Batch, Mini-Batch ($Batch\_Size = 64$), and Stochastic Gradient Descent (SGD).
    * **Activation Functions:** ReLU, Tanh, and Sigmoid (with safety clipping to prevent math errors like overflow).
  * **Smart Table:** Automatically created a final comparison table and highlighted the best-performing result in bold with a green background.

### 2. `online_shopping.csv` (Dataset)
* **What it is:** A clean dataset with **12,330 rows** of online customer shopping data.
* **Why it's used:** Used to train our custom neural network to predict whether a customer will make a purchase (`Revenue = True/False`).

### 3. `NumPy.ipynb` (NumPy Practice)
* **What it is:** Practice exercises for NumPy arrays, slicing, and matrix multiplication.
* **Why it's used:** This is the foundation for building the custom neural network.

### 4. `Pandas.ipynb` (Data Analysis)
* **What it is:** Practice on loading CSV files, handling missing data, and cleaning data using Pandas.

### 5. `Sci_kit_Learn.ipynb` (Machine Learning Tools)
* **What it is:** Basic machine learning code using Scikit-Learn for preprocessing and data splitting.

### 6. `tensorflow.ipynb` (Introduction to Deep Learning Frameworks)
* **What it is:** Basic introductory experiments using TensorFlow and Keras.

---

## 🧠 Key Highlights

* **Built from Scratch:** Wrote all math formulas (Forward Propagation, Loss calculation, Backpropagation, and Weight updates) manually using linear algebra (`np.dot`).
* **Error Prevention:** Added safety clipping (`np.clip`) to prevent overflow errors in activation functions.
* **Comparison:** Compared how different optimizers (Batch, Mini-Batch, SGD) affect training cost and test accuracy.

---

## 🛠️ Tech Stack

* **Language:** Python 3
* **Libraries:** NumPy, Pandas, Scikit-Learn, TensorFlow, Matplotlib
* **Environment:** Google Colab / Jupyter Notebook

---

## 👨‍💻 Author

**Mst. Tanzina Islam**  
