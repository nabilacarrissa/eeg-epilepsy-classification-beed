# 📘 Klasifikasi Epileptic Seizure Menggunakan Sinyal EEG

## Machine Learning & Deep Learning (Bangalore EEG Epilepsy Dataset – BEED)

---

## 👤 Informasi

- **Nama:** Nabila Carrissa Dewi
- **Repository:** https://github.com/nabilacarrissa/eeg-epilepsy-classification-beed
- **Video Presentasi:** https://youtu.be/GGM0MhEDik8

---

## 1. 🎯 Ringkasan Proyek

Proyek ini bertujuan untuk menyelesaikan permasalahan **klasifikasi kejang epilepsi (epileptic seizure)** menggunakan **sinyal EEG (Electroencephalography)** dengan pendekatan **Machine Learning dan Deep Learning**.

Tahapan utama dalam proyek ini meliputi:

- Melakukan **data preparation** pada data EEG
- Membangun **tiga model klasifikasi**, yaitu:
  - Model Baseline
  - Model Advanced Machine Learning
  - Model Deep Learning
- Melakukan **evaluasi performa model**
- Menentukan **model terbaik** berdasarkan metrik evaluasi

---

## 2. 📄 Problem & Goals

### **Problem Statements**

1. Sinyal EEG memiliki pola yang kompleks dan sulit dianalisis secara manual.
2. Dibutuhkan model yang mampu mengklasifikasikan kondisi epileptic dan non-epileptic secara akurat.
3. Perlu dibandingkan performa metode machine learning konvensional dengan deep learning pada data EEG.

### **Goals**

1. Mengembangkan model klasifikasi epilepsi berbasis sinyal EEG.
2. Membandingkan performa baseline, advanced ML, dan deep learning model.
3. Menentukan model terbaik berdasarkan hasil evaluasi.

---

## 📁 Struktur Folder

betulkan tampilan dibawah ini 
EEG-Epilepsy-BEED/
├── data/
│   ├── raw/
│   │   └── BEED_Data.csv          # Dataset asli (tidak di-commit)
│   └── processed/
│       └── beed_clean.csv         # Data setelah preprocessing
├── notebooks/
│   └── EEG_Epilepsy_BEED.ipynb    # Notebook utama (end-to-end)
├── models/
│   ├── baseline_logreg.pkl        # Baseline model
│   ├── random_forest.pkl          # Advanced ML model
│   └── neural_network.h5          # Deep Learning model
├── images/
│   └── evaluation/
│       ├── confusion_matrix.png
│       ├── accuracy_plot.png
│       └── loss_plot.png
├── src/
│   ├── preprocessing.py           # (opsional) fungsi preprocessing
│   ├── training.py                # (opsional) training pipeline
│   └── evaluation.py              # (opsional) evaluasi model
├── requirements.txt               # Dependency
├── .gitignore
└── README.md

---

## 3. 📊 Dataset

- **Nama Dataset:** Bangalore EEG Epilepsy Dataset (BEED)
- **Sumber:** Dataset EEG medis
- **Jumlah Data:** 8000 sampel _(sesuai output `df.shape`)_
- **Tipe Data:** Tabular (representasi sinyal EEG)
- **Task:** Classification (Epileptic vs Non-Epileptic)

### **Fitur Utama**

| Fitur                | Deskripsi                               |
| -------------------- | --------------------------------------- |
| EEG Features         | Nilai sinyal EEG dari berbagai channel  |
| Statistical Features | Mean, standard deviation, variance, dll |
| Label                | Kelas epileptic / non-epileptic         |

---

## 4. 🔧 Data Preparation

Tahapan data preparation yang dilakukan:

- **Cleaning:**  
  Menangani missing values dan memastikan konsistensi data.
- **Transformasi:**  
  Normalisasi dan scaling fitur EEG.
- **Splitting:**  
  Pembagian data menjadi data training dan testing secara stratified.

---

## 5. 🤖 Modeling

Model yang digunakan dalam proyek ini:

- **Model 1 – Baseline:**  
  Logistic Regression

- **Model 2 – Advanced Machine Learning:**  
  Random Forest

- **Model 3 – Deep Learning:**  
  Neural Network (Multilayer Perceptron)

---

## 6. 🧪 Evaluation

### **Metrik Evaluasi**

- Accuracy
- Precision
- Recall
- F1-Score

### **Hasil Evaluasi**

Metrik yang digunakan: Accuracy
| Model | Score (Accuracy) | Catatan |
| ------------- | ---------------- | ----------------------- |
| Baseline | 0.4731 (47.31%) | Performa dasar |
| Advanced ML | 0.8371 (83.71%) | Lebih stabil dan akurat |
| Deep Learning | 0.9637 (96.37%) | Performa terbaik |

---

## 7. 🏁 Kesimpulan

- **Model Terbaik:** Deep Learning (Neural Network)
- **Alasan:**  
  Model deep learning mampu menangkap pola kompleks pada sinyal EEG dengan sangat baik dan menghasilkan accuracy tertinggi.
- **Insight Penting:**  
  Pendekatan deep learning memberikan peningkatan performa yang signifikan dibandingkan metode machine learning konvensional dalam klasifikasi sinyal EEG.

---

## 8. 🔮 Future Work

- Menambahkan jumlah data EEG
- Melakukan hyperparameter tuning
- Mencoba arsitektur deep learning lain seperti CNN atau LSTM
- Deployment ke sistem real-time atau aplikasi web

---

## 9. 🔁 Reproducibility

Untuk mereproduksi proyek ini:

- Gunakan **Python 3.9+**
- Install dependency melalui `requirements.txt`
- Jalankan notebook `ML_Project.ipynb` secara berurutan

---

## 🛠️ Tools & Libraries

- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- TensorFlow / Keras

---

## 👩‍🎓 Author

**Nabila Carrissa Dewi**  
Program Studi: Teknologi Rekayasa Perangkat Lunak
Mata Kuliah: Data Science
