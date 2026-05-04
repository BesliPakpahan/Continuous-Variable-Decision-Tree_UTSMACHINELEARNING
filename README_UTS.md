# UTS - Prediksi Gaji Karyawan (Mirna)

Dokumentasi singkat untuk deliverable UTS: model prediksi gaji berbasis Regression Tree.

## Ringkasan
- Tujuan: Membantu Mirna memprediksi gaji calon karyawan berdasarkan data historis.
- Dataset: `UTS/UTS/data_karyawan.csv` (fitur: usia, pengalaman_kerja, jenis_kelamin, pendidikan, gaji).

## Metode
- Model utama: DecisionTreeRegressor (Regression Tree) dari scikit-learn.
- Preprocessing: imputasi nilai hilang pada `pengalaman_kerja` (median); label encoding untuk `jenis_kelamin` dan `pendidikan`.
- Evaluasi: RMSE, MAE, dan R² pada testing set; dibandingkan dua kedalaman pohon (max_depth=10 dan max_depth=15).

## Hasil singkat
- Model terbaik dipilih berdasarkan R² pada testing set (dicetak di notebook).
- Feature importance diekstrak dari model; biasanya usia dan pengalaman kerja muncul sebagai kontributor utama.

## Cara pakai
1. Buka notebook `UTS/UTS/utsmachinelearning.ipynb` dan jalankan semua cell (kernel Python 3.10+).
2. Gunakan fungsi `predict_gaji_karyawan_baru(usia, pengalaman, jenis_kelamin, pendidikan)` di dalam notebook untuk memprediksi gaji baru.

## Catatan
- File yang relevan: `UTS/UTS/utsmachinelearning.ipynb`, `UTS/UTS/data_karyawan.csv`, `UTS/UTS/studi kasus 3.txt`.
- Folder laporan mingguan telah dihapus dari repository agar repositori berfokus pada deliverable UTS.

Jika Anda ingin README ditempatkan di dalam folder `UTS/` atau ingin menambahkan detail hasil (nilai R², RMSE), beri tahu saya dan saya akan perbarui.
