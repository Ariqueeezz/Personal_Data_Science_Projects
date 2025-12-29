# 🏥 Peningkatan performa model Algoritma Klasifikasi dengan Penerapan Hybrid Resampling SMOTE-ENN menggunakan dataset diabetes (brfss 2015)

[![Python](https://img.shields.io/badge/Python-3.10.12-blue.svg)](https://www.python.org/downloads/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0.3-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.2.2-orange.svg)](https://scikit-learn.org/)
[![imbalanced-learn](https://img.shields.io/badge/imbalanced--learn-0.10.1-ff6347?logo=python&logoColor=white)](https://imbalanced-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-2.0.3-337ab7?logo=xgboost&logoColor=white)](https://xgboost.readthedocs.io/)

**Proyek penelitian ini mengembangkan model machine learning untuk deteksi dini diabetes menggunakan pendekatan hybrid resampling SMOTE-ENN (Synthetic Minority Over-sampling Technique - Edited Nearest Neighbors) untuk mengatasi ketidakseimbangan kelas pada dataset indikator kesehatan.**

## 📌 Highlight Proyek Awal

- **Algoritma**: KNN, Naive Bayes, Decision Tree (C.45)
- **Dataset**: BRFSS 2015 Diabetes Health Indicators (253.680 record, 21 fitur)
- **Evaluasi Model**: dengan Akurasi, Precision, Recall, F1-Score, ROC dan AUC
> Ket:
> - Dataset harus 100rb baris/instances dan sudah pernah dipakai pada artikel orang lain
> - Akurasi > 0.95

## 📌 Highlight Penelitian/Proyek Besar

- **Dataset**: BRFSS 2015 Diabetes Health Indicators (253.680 record, 21 fitur)
- **Distribusi Kelas**: Highly imbalanced (218.334 negatif : 35.346 positif)
- **Model Terbaik**: Random Forest + SMOTE-ENN
- **Peningkatan Recall**: Dari 17.34% → 96.83% (5.6× improvement)
- **ROC-AUC Score**: 0.9931

</div>

---

## 👥 Tim Pengembang

**Kelompok 1 - Kelas F5A1**

| Nama | NPM |
|------|-----|
| Raihan Ariq Muzakki | 202310715297 |
| Bayu Aji Pradana | 202310715302 |
| Fazri Abdurahman | 202310715082 |
| Syahril Achmad Fahrezi | 202310715211 |
| Awang Andriansyah Hermawan | 202310715155 |
| Advan Zharif Naja | 202310715290 |
| Dimas Hendri Pamungkas | 202310715274 |

**Dosen Pengampu:** Wowon Priatna, ST., M.Ti  
**Mata Kuliah:** Machine Learning  
**Institusi:** Universitas Bhayangkara Jakarta Raya

---

## 📌 Informasi Proyek

### Proyek Awal
- **Nama Proyek:** Deteksi Dini Penyakit Diabetes Menggunakan Algoritma Decision Tree, Naive Bayes, KNN dengan penerapan SMOTE-ENN
- **Notebook:** [Proyek 1](https://colab.research.google.com/github/Ariqueeezz/MachineLearningProject/blob/main/Experiment_DiabetesPrediction.ipynb)
- **Platform:** Google Colab
- **Bahasa:** Python 100%

### Proyek Besar/Penelitian
- **Nama Proyek:** Peningkatan Kinerja Deteksi Dini Diabetes Melalui Komparasi Algoritma Klasifikasi dengan Penerapan Hybrid Resampling SMOTE-ENN
- **Notebook:** [Proyek 2](https://colab.research.google.com/github/Ariqueeezz/MachineLearningProject/blob/main/Experiment2_DiabetesPrediction.ipynb)
- **Platform:** Google Colab
- **Bahasa:** Python 100%

---

## 🎯 Tujuan Penelitian/Proyek Besar

1. Mengkomparasi performa algoritma klasifikasi berbasis pohon (Decision Tree, Random Forest, XGBoost) untuk deteksi dini diabetes
2. Menganalisis dampak hybrid resampling SMOTE-ENN terhadap kemampuan deteksi kelas minoritas
3. Meminimalkan False Negative (kasus diabetes yang terlewat) untuk mendukung intervensi dini  

---

## 📊 Dataset

### Sumber Data
**BRFSS 2015 Diabetes Health Indicators Dataset**
- Total record: 253.680
- Jumlah fitur: 21 variabel prediktor
- Target: `Diabetes_binary` (0 = tidak diabetes, 1 = diabetes/prediabetes)
- Sumber: [Kaggle - Diabetes Health Indicators](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)

### Karakteristik Fitur

| Kategori | Fitur |
|----------|-------|
| **Kondisi Kesehatan** | HighBP, HighChol, CholCheck, BMI, Stroke, HeartDiseaseorAttack |
| **Gaya Hidup** | Smoker, PhysActivity, Fruits, Veggies, HvyAlcoholConsump |
| **Akses Kesehatan** | AnyHealthcare, NoDocbcCost |
| **Status Kesehatan** | GenHlth, MentHlth, PhysHlth, DiffWalk |
| **Demografi** | Sex, Age, Education, Income |

### Distribusi Kelas
```
Data Asli (Imbalanced):
├── Kelas 0 (Non-diabetes): 218.334 (86.1%)
└── Kelas 1 (Diabetes/Prediabetes): 35.346 (13.9%)

Setelah SMOTE-ENN:
├── Kelas 0: 145.088 (43.9%)
└── Kelas 1: 185.263 (56.1%)
```

## 🙏 Acknowledgments

### Special Thanks
- 🎓 **Bapak Wowon Priatna, ST., M.Ti** - Dosen pembimbing dan pengampu mata kuliah
- 🏫 **Universitas Bhayangkara Jakarta Raya** - Dukungan fasilitas dan laboratorium
- 📚 **Rekan Rekan Sekelompok** - Bantuan Pembuatan Proyek

### Tools & Services
- Google Colab - Notebook terbaik untuk Machine Learning Model development
- Github - Version control

<div align="center">

**Made with ❤️ by Kelompok 1**

**Fakultas Ilmu Komputer - Program Studi Informatika**  
**Universitas Bhayangkara Jakarta Raya**

**2025**

</div>
