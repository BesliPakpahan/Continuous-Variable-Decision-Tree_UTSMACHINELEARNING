# UTS - Prediksi Gaji Karyawan (Mirna)

Repository ini berisi deliverable UTS: notebook dan data untuk tugas prediksi gaji karyawan.

Isi repository:
- `UTS/UTS/utsmachinelearning.ipynb` — Notebook utama (preprocessing, training, evaluasi, prediksi).
- `UTS/UTS/data_karyawan.csv` — Dataset historis karyawan yang digunakan.
- `UTS/UTS/studi kasus 3.txt` — Deskripsi studi kasus.

Metode singkat:
- Model: DecisionTreeRegressor (Regression Tree) dari scikit-learn.
- Preprocessing: imputasi median untuk `pengalaman_kerja`, label encoding untuk kategori.
- Evaluasi: RMSE, MAE, dan R²; dibandingkan dua konfigurasi pohon (max_depth=10 & max_depth=15).

Cara menjalankan:
1. Buka `UTS/UTS/utsmachinelearning.ipynb` di Jupyter Notebook / JupyterLab.
2. Jalankan semua cell (kernel Python 3.10+ disarankan).
3. Gunakan fungsi `predict_gaji_karyawan_baru(...)` di dalam notebook untuk memprediksi gaji calon karyawan.

Catatan:
- Repositori ini telah dibersihkan sehingga hanya berisi konten UTS dan README.
- Jika Anda ingin README dipindah ke dalam folder `UTS/` atau menambahkan nilai metrik yang tercetak di notebook, beritahu saya.
# 📚 Machine Learning — Semester 6

Repositori ini berisi kumpulan tugas mata kuliah **Machine Learning** selama **Semester 6**.

---

## 👤 Identitas Mahasiswa

| Keterangan | Detail |
|---|---|
| **Nama** | Besli Saut Marito Pakpahan |
| **NIM** | 4222301027 |
| **Kelas** | Pagi A |
| **Mata Kuliah** | Machine Learning |
| **Semester** | 6 |

---

## 📁 Struktur Repositori

```
Machine-Learning-SEMS6/
├── week 1/
│   ├── Hands_On_Function_in_Python.ipynb
│   ├── Hands_On_Main_Principles_of_OOP.ipynb
│   ├── Hands_On_OOP_Paradigm_Concepts.ipynb
│   └── Week2_Tipe_Data.ipynb
│
├── week 2/
│   ├── Assignment_Week 3.ipynb
│   ├── california_dataset.csv
│   ├── company.csv
│   └── TelcoCustomerChurn.csv
│
├── week 3/
│   ├── Supervised_Learning_Hands_On_Regresi.ipynb
│   └── USA_Housing.csv
│
└── week 5/
    ├── Supervised_Learning_Hands_On_Classification.ipynb
    ├── titanic.csv
    ├── Week 5 - Cara Kerja KNN.xlsx
    ├── Week 5 - Introduction to classification - KNN.pptx
    └── execution.log
```

---

## 📝 Daftar Tugas

### Week 1
| File | Topik |
|---|---|
| `Hands_On_Function_in_Python.ipynb` | Hands-on fungsi dan tipe data di Python |
| `Hands_On_Main_Principles_of_OOP.ipynb` | Prinsip utama OOP beserta implementasi sistem library |
| `Hands_On_OOP_Paradigm_Concepts.ipynb` | Konsep paradigma OOP |
| `Week2_Tipe_Data.ipynb` | Tipe data di Python |

### Week 2
| File | Topik |
|---|---|
| `Assignment_Week 3.ipynb` | Feature Engineering: Outlier Handling (IQR), Missing Value Handling, dan Encoding |

### Week 3
| File | Topik |
|---|---|
| `Supervised_Learning_Hands_On_Regresi.ipynb` | Supervised Learning untuk regresi menggunakan dataset perumahan |

### Week 5
| File | Topik |
|---|---|
| `Supervised_Learning_Hands_On_Classification.ipynb` | Supervised Learning untuk klasifikasi (Titanic), EDA, preprocessing, training, dan evaluasi model |
| `Week 5 - Cara Kerja KNN.xlsx` | Materi pendukung konsep kerja algoritma KNN |
| `Week 5 - Introduction to classification - KNN.pptx` | Materi presentasi pengantar klasifikasi dan KNN |

### Catatan
- Week 4 di-skip sesuai alur perkuliahan.

---

## 🛠️ Teknologi yang Digunakan

- Python 3
- Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- SciPy

---

> Politeknik Negeri Batam — Jurusan Teknik Elektro — Prodi Teknik Robotika
