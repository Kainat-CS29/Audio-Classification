# 🎵 Audio Classification using ANN

## 📌 Project Overview
This project focuses on **classifying environmental sounds** using **Artificial Neural Networks (ANN)**.  
We use the **UrbanSound8K** dataset and apply **feature extraction techniques** like **MFCCs** (Mel-Frequency Cepstral Coefficients) to train a robust model for audio classification.  
The model distinguishes between multiple categories of sounds such as **dog barks, sirens, car horns, and more**.

---

## 📂 Dataset
- **Name:** UrbanSound8K  
- **Download:** [UrbanSound8K Dataset](https://goo.gl/8hY5ER)  
- **Size:** ~5.4 GB  
- **Format:** `.wav` files  
- **Classes:** 10 categories (e.g., Dog Bark, Car Horn, Siren, etc.)  
- **Samples:** 8,732 audio clips with metadata.

---

## 🔍 Exploratory Data Analysis (EDA)
We performed EDA to:
- Inspect dataset structure & metadata.
- Analyze **class distribution** to check for imbalance.
- Visualize **waveforms** and **spectrograms** for different sound types.
- Examine **sample rates**, durations, and amplitude patterns.

---

## ⚙️ Data Preprocessing
- **Resampling**: Standardized sample rate using `resampy`.
- **Feature Extraction**: Used `librosa` to compute **MFCCs**.
- **Normalization**: Scaled features for uniformity.
- **Data Split**: 80% Training, 20% Testing.

---

## 🧠 Model Architecture
We implemented an **Artificial Neural Network (ANN)** with:
- **Input Layer**: MFCC features
- **Hidden Layers**: Dense layers with activation functions (ReLU)
- **Output Layer**: Softmax activation for multi-class classification

---

## 📊 Training & Evaluation
- **Loss Function**: Categorical Cross-Entropy  
- **Optimizer**: Adam  
- **Metrics**: Accuracy, Precision, Recall, F1-score  
- **Evaluation Tools**: Confusion matrix, classification report.

---

## 🚀 Steps to Run

**1. Clone the repository**
```bash
git clone https://github.com/yourusername/audio-classification.git
cd audio-classification

**2. Install dependencies**
pip install -r requirements.txt

**3. Download and extract the dataset into** data/UrbanSound8K/

**4. Run preprocessing and training**
python train.py

**5. Evaluate the model**
python evaluate.py

## 🛠 Technologies Used Python

Librosa – Audio processing

NumPy / Pandas – Data handling

Matplotlib / Seaborn – Visualization

Scikit-learn – Model evaluation

TensorFlow / Keras – Deep learning

## 📌 Applications
Speech recognition

Music genre classification

Environmental sound detection

Industrial anomaly detection


