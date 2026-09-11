# Analisis Faktor Determinan Terhadap Putusan Hakim pada Tindak Pidana Korupsi di Indonesia

Repository ini berisi kode, dataset, dan hasil eksperimen untuk penelitian skripsi mengenai analisis determinan terhadap putusan hakim pada perkara tindak pidana korupsi di Indonesia menggunakan metode **Random Forest** dan **Explainable AI (SHAP)**.

## Judul Penelitian

**Analisis Faktor Determinan Terhadap Putusan Hakim Pada Tindak Pidana Korupsi di Indonesia menggunakan Metode Random Forest dan Explainable AI (SHAP)**

## Latar Belakang

Putusan hakim pada perkara tindak pidana korupsi dapat dipengaruhi oleh berbagai karakteristik perkara dan faktor yang terdapat dalam suatu kasus. Penelitian ini menggunakan pendekatan Machine Learning untuk menganalisis hubungan antara karakteristik perkara dengan putusan hakim.

Model Random Forest digunakan untuk melakukan pemodelan klasifikasi, sedangkan Explainable AI menggunakan SHAP (*SHapley Additive exPlanations*) digunakan untuk membantu menginterpretasikan kontribusi masing-masing variabel terhadap hasil prediksi model.

## Tujuan Penelitian

Penelitian ini bertujuan untuk:

1. Melakukan preprocessing dan analisis terhadap data putusan perkara tindak pidana korupsi.
2. Membangun model klasifikasi menggunakan Random Forest.
3. Mengevaluasi performa model menggunakan metrik klasifikasi.
4. Mengidentifikasi variabel yang memiliki kontribusi terhadap hasil prediksi model.
5. Menginterpretasikan hasil model menggunakan SHAP.

## Dataset

Dataset penelitian berasal dari data putusan perkara tindak pidana korupsi di Indonesia.

Variabel yang digunakan dalam penelitian mencakup karakteristik perkara, faktor finansial, tuntutan, serta informasi terkait putusan hakim.

Contoh variabel yang digunakan antara lain:

* `uang_pengganti`
* `subsider_penjara`
* `nominal_uang`
* `vonis_bulan`
* `tuntutan_penjara`
* `jenis_dakwaan`
* `jabatan_terdakwa`

Dataset akan melalui tahap pemeriksaan, preprocessing, dan transformasi sebelum digunakan dalam proses pemodelan.

> **Catatan:** Nilai `0` pada dataset diperlakukan sebagai nilai data yang valid dan tidak secara otomatis dianggap sebagai missing value. Missing value hanya mengacu pada data yang benar-benar kosong/tidak memiliki isi.

## Metodologi

Tahapan penelitian secara umum adalah sebagai berikut:

```text
Pengumpulan Data
       ↓
Data Preprocessing
       ↓
Exploratory Data Analysis (EDA)
       ↓
Feature Preparation
       ↓
Train-Test Split
       ↓
Random Forest
       ↓
Evaluasi Model
       ↓
Explainable AI (SHAP)
       ↓
Analisis Determinan
```

### 1. Data Preprocessing

Tahap preprocessing meliputi:

* Pemeriksaan struktur dataset
* Pemeriksaan missing value
* Penanganan data kosong
* Transformasi variabel
* Encoding variabel kategorikal
* Persiapan fitur dan target

### 2. Exploratory Data Analysis

EDA dilakukan untuk memahami karakteristik dataset dan distribusi variabel yang digunakan dalam penelitian.

### 3. Random Forest

Random Forest digunakan sebagai metode utama untuk membangun model klasifikasi berdasarkan fitur-fitur yang tersedia pada dataset.

### 4. Evaluasi Model

Performa model akan dievaluasi menggunakan metrik klasifikasi yang sesuai, seperti:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Kendall's Tau
* Spearman Correlation

### 5. Explainable AI

SHAP digunakan untuk menginterpretasikan model dengan menganalisis kontribusi masing-masing fitur terhadap hasil prediksi.

Analisis SHAP digunakan untuk membantu mengidentifikasi fitur yang paling berpengaruh terhadap keputusan prediksi model.

## Struktur Repository

Struktur repository direncanakan sebagai berikut:

```text
Skripsi-Analisis-Determinan-Kasus-Korupsi/
│
├── README.md
│
├── notebooks/
│   └── Skripsi_Analisis_Determinan_Korupsi.ipynb
│
├── data/
│   ├── ekstraksi_dataset.csv
│
├── results/
    ├── figures/
    └── tables/

```

### `notebooks/`

Berisi notebook Google Colab yang digunakan untuk proses penelitian, mulai dari preprocessing hingga analisis model dan SHAP.

### `data/`

berisi data raw yang sudah diubah menjadi data tabular.

### `results/figures/`

Berisi visualisasi hasil penelitian seperti:

* Distribusi data
* Confusion matrix
* Feature importance
* SHAP summary plot
* SHAP bar plot

### `results/tables/`

Berisi tabel hasil eksperimen dan evaluasi model.

## Teknologi

Penelitian ini menggunakan beberapa teknologi dan library berikut:

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* SHAP

## Sumber Data

Data penelitian berasal dari putusan perkara tindak pidana korupsi di Indonesia yang digunakan sebagai sumber data penelitian.

Pengolahan data dilakukan untuk memperoleh dataset terstruktur yang dapat digunakan dalam proses analisis dan pemodelan Machine Learning.

## Reproducibility

Seluruh tahapan pengolahan data dan pemodelan akan didokumentasikan dalam notebook penelitian sehingga eksperimen dapat dilakukan kembali berdasarkan tahapan yang telah ditentukan.

## Author

**Muhammad Rafi Firnanda**

Mahasiswa Informatika
Data Science
