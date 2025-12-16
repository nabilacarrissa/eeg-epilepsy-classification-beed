🧠 EEG Epilepsy Detection using Machine Learning & Deep Learning

(Bangalore EEG Epilepsy Dataset – BEED)

👤 Informasi
Nama: Nabila Carrissa Dewi
Repo: 
Video: 

1. 🎯 Ringkasan Proyek

Proyek ini bertujuan untuk mendeteksi dan mengklasifikasikan kejang epilepsi (epileptic seizure) menggunakan sinyal EEG (Electroencephalography) dengan pendekatan   Machine Learning dan Deep Learning. Dataset yang digunakan adalah Bangalore EEG Epilepsy Dataset (BEED) yang berisi data sinyal EEG yang telah diproses dalam bentuk tabular.
Proyek ini dikembangkan sebagai tugas UAS mata kuliah Data Science / Machine Learning dan disusun mengikuti standar laporan proyek machine learning akademik.

Tahapan yang dilakukan dalam proyek ini meliputi:
  a. Melakukan data preparation pada dataset EEG
  b. Membangun tiga model:
    1. Model Baseline
    2. Model Advanced Machine Learning
    3. Model Deep Learning
  c. Melakukan evaluasi performa model
  d. Menentukan model terbaik berdasarkan metrik evaluasi yang relevan

2. 📄 Problem & Goals
Problem Statements :
Data sinyal EEG memiliki pola yang kompleks dan sulit dianalisis secara manual.

Diperlukan model yang mampu membedakan sinyal epileptic seizure dan non-epileptic seizure secara akurat.

Perlu dilakukan perbandingan antara pendekatan machine learning tradisional dan deep learning.

Goals

Membangun model klasifikasi epilepsi berbasis data EEG.

Membandingkan performa baseline, advanced ML, dan deep learning model.

Menentukan model terbaik berdasarkan metrik evaluasi.

📁 Struktur Folder
project/
│
├── data/                   # Dataset (tidak di-commit, download manual)
│
├── notebooks/              # Jupyter notebooks
│   └── ML_Project.ipynb
│
├── src/                    # Source code (opsional)
│
├── models/                 # Saved models
│   ├── model_baseline.pkl
│   ├── model_rf.pkl
│   └── model_dl.h5
│
├── images/                 # Visualizations
│   └── results/
│
├── requirements.txt        # Dependencies
├── .gitignore
└── README.md

3. 📊 Dataset

Sumber: Bangalore EEG Epilepsy Dataset (BEED)

Jumlah Data: [8000] sampel.

Tipe Data: Tabular (representasi sinyal EEG)

Task: Classification

Fitur Utama
| Fitur                | Deskripsi                              |
| -------------------- | -------------------------------------- |
| EEG_Channel          | Nilai sinyal EEG dari channel tertentu |
| Statistical_Features | Mean, std, variance, dll               |
| Label                | Kelas epileptic / non-epileptic        |

4. 🔧 Data Preparation

Tahapan data preparation yang dilakukan meliputi:

Cleaning:
Menangani missing values, data duplikat, dan outliers.

Transformasi:
Normalisasi dan scaling fitur EEG.

Splitting:
Pembagian data menjadi training dan testing set dengan stratified split.

5. 🤖 Modeling

Model yang digunakan dalam proyek ini adalah:

Model 1 – Baseline:
Logistic Regression / K-Nearest Neighbors (KNN)

Model 2 – Advanced ML:
Random Forest / Support Vector Machine (SVM)

Model 3 – Deep Learning:
Multilayer Perceptron (MLP) dengan minimal 2 hidden layer

6. 🧪 Evaluation
Metrik Evaluasi

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

Metrik yang digunakan: Accuracy
| Model         | Score (Accuracy) | Catatan                 |
| ------------- | ---------------- | ----------------------- |
| Baseline      | 0.4731 (47.31%)  | Performa dasar          |
| Advanced ML   | 0.8371 (83.71%)  | Lebih stabil dan akurat |
| Deep Learning | 0.9637 (96.37%)  | Performa terbaik        |

🔎 Versi Alternatif (jika dosen minta F1-Score)
| Model         | Score (F1-Score) | Catatan                 |
| ------------- | ---------------- | ----------------------- |
| Baseline      | 0.4762 (47.62%)  | Performa dasar          |
| Advanced ML   | 0.8340 (83.40%)  | Lebih stabil dan akurat |
| Deep Learning | 0.9637 (96.37%)  | Performa terbaik        |

“Berdasarkan hasil evaluasi, model Deep Learning (Neural Network) menunjukkan performa terbaik dengan accuracy sebesar 96.37%, jauh melampaui model baseline dan advanced machine learning. Hal ini menunjukkan bahwa neural network mampu menangkap pola kompleks pada sinyal EEG secara lebih efektif.”

7. 🏁 Kesimpulan

Model Terbaik: Deep Learning (MLP)

Alasan:
Mampu menangkap pola kompleks pada sinyal EEG dengan performa evaluasi tertinggi.

Insight Penting:
Deep learning memberikan peningkatan signifikan dibandingkan metode ML konvensional dalam klasifikasi EEG.

8. 🔮 Future Work

Menambahkan jumlah data EEG

Melakukan hyperparameter tuning lebih lanjut

Mencoba arsitektur deep learning lain (CNN / LSTM)

Deployment ke aplikasi web atau sistem real-time

9. 🔁 Reproducibility

Proyek ini dapat direproduksi dengan:

Menggunakan Python 3.9+

Menginstall dependency dari requirements.txt

Menjalankan notebook ML_Project.ipynb secara berurutan
