# Klasifikasi Kualitas Kopi Menggunakan Machine Learning: Perbandingan K-Nearest Neighbors (KNN) dan Support Vector Machines (SVM)
## 1. Judul / Topik Project dan Identitas Lengkap
### Judul: Klasifikasi Kualitas Kopi Menggunakan Machine Learning: Perbandingan K-Nearest Neighbors (KNN) dan Support Vector Machines (SVM)
### Identitas:
Nama: Fajar Adji Wicaksana

NIM: A11.2022.14147
## 2. Ringkasan dan Permasalahan Project + Tujuan yang Akan Dicapai + Model / Alur Penyelesaian
### Ringkasan
Proyek ini bertujuan untuk mengklasifikasikan kualitas kopi berdasarkan berbagai fitur menggunakan algoritma KNN dan SVM. Dataset yang digunakan berisi informasi mengenai karakteristik fisik dan kimia dari biji kopi yang diuji.

## Permasalahan
Permasalahan yang dihadapi adalah bagaimana mengklasifikasikan kualitas kopi dengan akurasi tinggi menggunakan teknik machine learning. Kualitas kopi dapat dipengaruhi oleh banyak faktor, sehingga memilih fitur yang tepat dan model yang efisien sangat penting.

## Tujuan
1. Mengidentifikasi fitur-fitur yang mempengaruhi kualitas kopi.
2. Membangun model KNN dan SVM untuk klasifikasi kualitas kopi.
3. Membandingkan performa kedua model dan menentukan model yang paling akurat.
   
## Model / Alur Penyelesaian
Berikut adalah bagan alur penyelesaian proyek ini:

! [import matplotlib.pyplot as plt
import matplotlib.patches as mpatches
from matplotlib.offsetbox import AnnotationBbox, TextArea


fig, ax = plt.subplots(figsize=(14, 16))
ax.set_xlim(0, 12)
ax.set_ylim(-12, 18)
ax.axis('off')


boxes = {
    "start": (5, 15, "Start"),
    "load_data": (5, 13, "Load Dataset"),
    "data_preprocessing": (5, 11, "Exploratory Data Analysis (EDA)"),
    "feature_selection": (5, 9, "Preprocessing Data"),
    "data_splitting": (5, 7, "Split Data untuk Training dan Testing"),
    "model_selection": (5, 5, "Training Model KNN"),
    "model_training": (5, 3, "Training Model SVM"),
    "grid_search": (5, 1, "Evaluasi Model KNN"),
    "final_evaluation": (5, -1, "Evaluasi Model SVM"),
    "perbandingan_hasil": (5, -3, "Perbandingan Hasil"),
    "kesimpulan" : (5, -6, "Kesimpulan"),
    "end": (5, -9, "End")
}

for key, (x, y, text) in boxes.items():
    ax.add_patch(mpatches.FancyBboxPatch((x-1, y-0.5), 2, 1, boxstyle="round,pad=0.3", edgecolor="black", facecolor="lightgrey"))
    ab = AnnotationBbox(TextArea(text, textprops=dict(ha='center', va='center', fontsize=12)), (x, y), frameon=False)
    ax.add_artist(ab)


arrows = [
    ("start", "load_data"),
    ("load_data", "data_preprocessing"),
    ("data_preprocessing", "feature_selection"),
    ("feature_selection", "data_splitting"),
    ("data_splitting", "model_selection"),
    ("model_selection", "model_training"),
    ("model_training", "grid_search"),
    ("grid_search", "final_evaluation"),
    ("final_evaluation", "perbandingan_hasil"),
    ("perbandingan_hasil", "kesimpulan"),
    ("kesimpulan", "end")
]

for (start, end) in arrows:
    x1, y1 = boxes[start][:2]
    x2, y2 = boxes[end][:2]
    ax.annotate("", xy=(x2, y2+0.5), xytext=(x1, y1-0.5), arrowprops=dict(arrowstyle="->"))

plt.show()]

## 3. Penjelasan Dataset, EDA dan Proses Features Dataset
### Dataset
Dataset yang digunakan berasal dari Kaagle. Dataset ini mencakup berbagai atribut yang mencerminkan kualitas kopi seperti aroma, rasa, dan kandungan kimia.

### Exploratory Data Analysis (EDA)
Lakukan analisis eksplorasi data untuk memahami distribusi data, korelasi antar fitur, dan identifikasi outlier.

### Proses Features Dataset
Langkah-langkah preprocessing data seperti penanganan missing values, normalisasi, dan encoding fitur kategorikal.

## 4. Proses Learning / Modeling
### Model KNN
* Penjelasan konsep KNN
* Implementasi model KNN
* Parameter tuning
* Model SVM
* 
### Penjelasan konsep SVM
* Implementasi model SVM
* Parameter tuning
  
## 5. Performa Model
### Evaluasi Model
* Menggunakan metrik akurasi, precision, recall, dan F1-score untuk mengevaluasi performa model.
* Menampilkan confusion matrix.
* Perbandingan Model
* Membandingkan performa antara model KNN dan SVM.
  
## 6. Diskusi Hasil dan Kesimpulan
### Diskusi Hasil
* Analisis hasil evaluasi model.
* Faktor-faktor yang mempengaruhi performa model.
  
### Kesimpulan
* Model mana yang memiliki performa terbaik.
* Potensi pengembangan lebih lanjut.
