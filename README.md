# Prediksi Permintaan Sewa Sepeda Per Jam (Bike Sharing Demand Prediction)

## 🎯 Tujuan Proyek
Proyek ini bertujuan untuk membangun model **Machine Learning Regresi** yang dapat memprediksi secara akurat **jumlah total peminjaman sepeda per jam**.

Prediksi yang akurat sangat krusial untuk **perencanaan operasional** operator *bike sharing*, sehingga mereka dapat mengoptimalkan distribusi armada untuk:
1.  Mencegah kekurangan pasokan sepeda di jam sibuk.
2.  Menghindari pemborosan unit di jam sepi.

## 🚲 Konteks dan Permasalahan Bisnis

Sistem *bike sharing* menghasilkan data yang sangat kaya (waktu, cuaca, durasi) yang merekam pola mobilitas masyarakat perkotaan.

**Permasalahan (Problem Statement):**
Permintaan sewa sepeda sangat **fluktuatif** tergantung musim, cuaca, dan waktu. Tanpa pemahaman mendalam mengenai faktor-faktor ini, perusahaan sulit mengatur ketersediaan unit. Oleh karena itu, model prediksi diperlukan sebagai dasar untuk **optimasi armada** dan **peningkatan kualitas layanan**.

## ⚙️ Pendekatan Analitik

1.  **Variabel Prediktor:** Digunakan faktor waktu (jam, musim, hari libur) dan kondisi cuaca (suhu, kelembapan, dll.).
2.  **Model:** Membangun model regresi (termasuk model kompleks seperti XGBoost) untuk memprediksi target utama: `cnt` (jumlah total peminjaman).
3.  **Metrik Evaluasi:** Kinerja model dinilai menggunakan metrik kesalahan (semakin rendah, semakin baik), yaitu:
    * **RMSE** (Root Mean Squared Error)
    * **MAE** (Mean Absolute Error)
    * **MAPE** (Mean Absolute Percentage Error)
