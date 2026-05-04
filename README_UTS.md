# UTS Machine Learning

## Prediksi Gaji Karyawan Menggunakan Regression Tree

Repository ini berisi deliverable UTS untuk studi kasus prediksi gaji karyawan (Mirna) menggunakan pendekatan machine learning berbasis **Continuous Variable Decision Tree**.

## Latar Belakang
Mirna sebagai pemilik startup membutuhkan pendekatan yang konsisten untuk:
1. Menentukan gaji calon karyawan secara adil dan kompetitif.
2. Memahami faktor-faktor yang paling memengaruhi besaran gaji.

Masalah ini dimodelkan sebagai **regresi** karena target yang diprediksi adalah nilai kontinu (`gaji`).

## Dataset
- Sumber data: `data_karyawan.csv`
- Jumlah fitur utama:
	- `usia`
	- `pengalaman_kerja`
	- `jenis_kelamin`
	- `pendidikan`
- Target:
	- `gaji`

## Metodologi
Pipeline yang digunakan pada notebook `utsmachinelearning.ipynb`:

1. Data loading dan eksplorasi awal.
2. Data preprocessing:
	 - Imputasi nilai hilang pada `pengalaman_kerja` dengan median.
	 - Encoding fitur kategorikal (`jenis_kelamin`, `pendidikan`) ke bentuk numerik.
3. Train-test split (80:20).
4. Pelatihan dua model `DecisionTreeRegressor`:
	 - Model A: `max_depth=10`
	 - Model B: `max_depth=15`
5. Evaluasi model menggunakan metrik regresi.
6. Analisis feature importance untuk interpretasi faktor penentu gaji.

## Metrik Evaluasi
Karena studi kasus ini adalah **regresi**, evaluasi menggunakan:
- **MSE** (Mean Squared Error)
- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)
- **R2 Score**

Catatan: **Confusion matrix tidak digunakan** pada studi kasus ini karena confusion matrix adalah metrik untuk klasifikasi.

## Hasil dan Insight Utama
- Model terbaik dipilih berdasarkan performa pada data uji (terutama nilai R2 dan error yang lebih rendah).
- Analisis feature importance menunjukkan faktor yang paling berkontribusi terhadap prediksi gaji.
- Model dapat digunakan sebagai baseline objektif untuk rekomendasi gaji kandidat baru.

## Struktur File
- `utsmachinelearning.ipynb` -> notebook utama (end-to-end workflow)
- `data_karyawan.csv` -> dataset historis karyawan
- `studi kasus 3.txt` -> deskripsi studi kasus UTS
- `README_UTS.md` -> dokumentasi proyek

## Cara Menjalankan
1. Buka `utsmachinelearning.ipynb` di Jupyter Notebook / JupyterLab / VS Code.
2. Pastikan environment Python telah terpasang library: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.
3. Jalankan seluruh cell secara berurutan dari awal hingga akhir.
4. Gunakan fungsi `predict_gaji_karyawan_baru(...)` untuk simulasi prediksi kandidat baru.

## Batasan dan Saran Pengembangan
- Model belum memasukkan faktor eksternal seperti jabatan, performa, dan keahlian khusus.
- Validasi silang (cross-validation) dan hyperparameter tuning lanjutan dapat meningkatkan stabilitas model.
- Prediksi sebaiknya digunakan sebagai **pendukung keputusan**, bukan satu-satunya penentu nilai gaji.

## Penulis
Besli Saut Marito Pakpahan

