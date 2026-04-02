# 🧠 Hybrid Alzheimer’s Disease Progression Forecasting

A hybrid soft computing project that combines **Recurrent Neural Networks (LSTM)** and **Fuzzy Logic** to predict the progression of Alzheimer’s Disease using longitudinal clinical data.

---

## 📌 Overview

Alzheimer’s Disease (AD) is a progressive neurodegenerative disorder. Early prediction of disease progression helps in better treatment planning and clinical decision-making.

This project proposes a **hybrid intelligent system** that:

* Learns **temporal patterns** using LSTM (deep learning)
* Handles **uncertainty** using fuzzy logic
* Produces **interpretable predictions** for disease progression

---

## 🎯 Objectives

* Predict disease stages:

  * **CN (Cognitively Normal)**
  * **MCI (Mild Cognitive Impairment)**
  * **AD (Alzheimer’s Disease)**
* Model **time-dependent progression** using longitudinal data
* Improve interpretability using **fuzzy inference rules**

---

## 🧠 System Architecture

```plaintext
ADNI Dataset (ADNIMERGE.csv)
        ↓
Data Preprocessing
        ↓
Sequence Generation (time-series)
        ↓
LSTM Model (prediction)
        ↓
Fuzzy Logic System (refinement)
        ↓
Final Disease Stage Output
```

---

## 🛠️ Tech Stack

* **Language:** Python
* **Deep Learning:** TensorFlow (Keras)
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Fuzzy Logic:** scikit-fuzzy
* **Visualization:** Matplotlib
* **Environment:** WSL / Linux / VS Code

---

## 📂 Project Structure

```plaintext
adni-project/
│
├── data/                  # Place dataset here (not included in repo)
│   └── ADNIMERGE.csv
│
├── src/
│   ├── preprocess.py      # Data cleaning & preparation
│   ├── sequence.py        # Time-series sequence generation
│   ├── model.py           # LSTM model definition
│   ├── train.py           # Training pipeline
│   ├── fuzzy.py           # Fuzzy logic module
│   └── utils.py
│
├── notebooks/
│   └── exploration.ipynb  # Optional EDA
│
├── outputs/
│   ├── model.h5           # Saved model
│   └── results.txt
│
├── requirements.txt
└── main.py
```

---

## 📥 Dataset Access

This project uses the **ADNI (Alzheimer’s Disease Neuroimaging Initiative)** dataset.

### 🔗 Steps to download:

1. Go to the ADNI data portal
2. Register and request access
3. Download:

   * **ADNIMERGE.csv**

### 📌 Place the file:

```plaintext
/data/ADNIMERGE.csv
```

⚠️ Note: The dataset is not included in this repository due to licensing restrictions.

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/adni-project.git
cd adni-project
```

---

### 2. Create virtual environment

```bash
python3 -m venv venv
source venv/bin/activate
```

---

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

```bash
python main.py
```

---

## 📊 Model Details

* Model Type: LSTM (Recurrent Neural Network)
* Input: Sequential patient data (Age, MMSE, CDRSB)
* Output: Disease stage classification (3 classes)

---

## 🧩 Fuzzy Logic Integration

The fuzzy module enhances interpretability by applying rule-based reasoning:

Example:

* IF MMSE is LOW AND Age is HIGH → High AD Risk
* IF MMSE is MEDIUM → Moderate Risk

---

## 📈 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score

---

## 💡 Key Features

* Hybrid AI system (Learning + Reasoning)
* Time-aware disease prediction
* Modular and extensible architecture
* Designed for research and academic use

---

## ⚠️ Notes

* Ensure dataset is properly placed before running
* ADNI data requires approval before access
* Sequence generation depends on longitudinal data ordering

---

## 🚀 Future Improvements

* Add UI using Streamlit
* Improve fuzzy rule base
* Use Transformer models for sequence learning
* Integrate multimodal data (MRI, PET)

---

## 👨‍💻 Authors

* Pakhi Agrawal
* Kaustubh Kanodia

---

## 📜 License

This project is for academic and research purposes only.
