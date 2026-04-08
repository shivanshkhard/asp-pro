# 🚗 Driver Stress & Fatigue Detection Using Speech

An intelligent **Audio Signal Processing + Machine Learning system** that detects a driver’s emotional state (Normal, Stress, Fatigue) using speech signals.
The system supports **real-time microphone input** and **audio file upload**, along with advanced visualization and data analysis.

---

## 📌 Overview

Driver fatigue and stress are major contributors to road accidents. This project leverages **speech signal processing** and **machine learning** to classify driver states and provide alerts for safer driving.

---

## 🎯 Features

* 🎤 **Real-time voice detection** using microphone
* 📁 **Upload audio file for prediction**
* 🤖 **ML-based classification (Random Forest / SVM)**
* 📊 **Advanced visualizations**:

  * Confusion Matrix
  * PCA plot
  * Feature correlation heatmap
  * Class distribution
* 📉 **MFCC & Spectrogram visualization**
* 💾 **Model saving & fast loading (joblib)**
* 📜 **Prediction logging (history.csv)**
* 📁 **Auto-saving recordings & graphs**

---

## 🧠 Model Details

* **Feature Extraction:**

  * MFCC (Mel Frequency Cepstral Coefficients)
  * Delta MFCC
  * Zero Crossing Rate (ZCR)
  * RMS Energy
  * Pitch & Pitch Variability
  * Energy Variance
  * Spectral Features

* **Models Used:**

  * Random Forest Classifier 🌲
  * Support Vector Machine (SVM) ⚡

* **Evaluation Metrics:**

  * Accuracy
  * Precision, Recall, F1-score
  * Confusion Matrix

---

## 📂 Project Structure

```
asp-driver-stress-detection/
│
├── src/
│   ├── data_loader.py
│   ├── feature_extractor.py
│   ├── model.py
│   ├── predict.py
│   ├── visualization.py
│
├── recordings/        # Saved live audio
├── graphs/            # Saved MFCC graphs
├── history.csv        # Prediction logs
│
├── main.py            # Full pipeline
├── quick_predict.py   # Fast inference (no training)
├── config.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

pip install -r requirements.txt
```

---

## ▶️ Usage

### 🔹 1. Train + Run Full System

```bash
python main.py
```

---

### 🔹 2. Fast Prediction (No Training)

```bash
python quick_predict.py
```

---

### 🔹 3. Input Modes

* **Option 1:** Upload `.wav` file
* **Option 2:** Live microphone recording 🎤

---

## 📊 Sample Output

* Prediction: `stress / fatigue / normal`
* Driver alert message
* Confusion matrix
* MFCC graph
* PCA visualization

---

## 📈 Results

* Achieved ~75–85% accuracy
* Improved fatigue detection using:

  * Class balancing
  * Pitch-based features
  * Energy-based features

---

## 🧠 Key Insights

* Fatigue detection depends on **low energy + low variation + flat tone**
* Speech-based emotion detection has **class overlap challenges**
* Feature engineering significantly improves performance

---

## 🚀 Future Enhancements

* Deep Learning (CNN / LSTM)
* Real-time continuous monitoring
* Web app deployment (Streamlit)
* Integration with driver monitoring systems

---

## 👨‍💻 Author

**Shivansh Gupta**
B.Tech AI & Data Science
Gati Shakti Vishwavidyalaya

---

## 📜 License

This project is for educational and research purposes.

---

## ⭐ Acknowledgements

* Librosa (Audio Processing)
* Scikit-learn (ML models)
* RAVDESS Dataset

---

> “Turning voice into insights for safer driving.” 🚀
