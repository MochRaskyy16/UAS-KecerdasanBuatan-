# Hasil Analisis Kedua Notebook

## CNN MobileNetV2

- Alur lengkap: data collection, EDA, split, preprocessing, augmentation,
  modeling, evaluation, export, dan inference.
- Menggunakan MobileNetV2 sebagai CNN transfer learning.
- Preprocessing menggunakan `preprocess_input`.
- Callback konsisten berdasarkan `val_loss`.
- Accuracy test 98,85%.
- Tidak terdapat underfitting atau overfitting signifikan.

## Random Forest

- Alur lengkap: data collection, EDA, split, feature engineering, modeling,
  evaluation, export, dan inference.
- Menggunakan 1.994 fitur per gambar.
- Accuracy test 95,59%.
- Training accuracy 100%.
- Validation Macro F1 91,22%.
- Terdapat indikasi overfitting ringan, bukan overfitting berat.
- Kelas Healthy memiliki recall terendah, yaitu 77%.

## Perbandingan

CNN lebih unggul pada accuracy, weighted F1, dan macro F1. Test split kedua
notebook berbeda dua gambar akibat pembulatan. Untuk pembandingan ilmiah yang
benar-benar identik, kedua model perlu memakai daftar file split yang sama.
