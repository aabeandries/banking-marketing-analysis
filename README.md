
# 📊 Bank Marketing Analytics

Proyek ini bertujuan untuk menganalisis data kampanye pemasaran telepon oleh sebuah institusi perbankan, dengan tujuan memprediksi apakah nasabah akan berlangganan produk deposito berjangka (*term deposit*).

---

## 🧾 Business Overview

Sebuah bank melakukan kampanye pemasaran melalui panggilan telepon kepada nasabah. Tujuannya adalah menawarkan produk deposito berjangka. Data yang dianalisis mencakup karakteristik nasabah, riwayat interaksi sebelumnya, dan hasil dari kampanye pemasaran sebelumnya.

---

## 🎯 Tujuan Analisis

1. Membangun model prediktif untuk mengklasifikasikan apakah nasabah akan berlangganan produk.
2. Mengoptimalkan strategi kampanye untuk meningkatkan efektivitas dan efisiensi.
3. Menggunakan interpretasi model (SHAP) untuk memahami pengaruh tiap fitur.
4. Mengukur potensi kerugian finansial dari keputusan prediksi yang salah.

---

## 🧾 Deskripsi Kolom

Berikut adalah penjelasan masing-masing kolom dalam dataset:

| Kolom                   | Deskripsi                                                                 |
|------------------------|---------------------------------------------------------------------------|
| `age`                  | Umur nasabah                                                              |
| `job`                  | Jenis pekerjaan nasabah                                                   |
| `marital`              | Status pernikahan nasabah                                                 |
| `education`            | Tingkat pendidikan nasabah                                                |
| `default`              | Apakah nasabah memiliki kredit macet sebelumnya                           |
| `balance`              | Saldo rata-rata tahunan dalam akun bank                                   |
| `housing`              | Apakah nasabah memiliki pinjaman rumah                                    |
| `loan`                 | Apakah nasabah memiliki pinjaman pribadi                                  |
| `contact`              | Jenis kontak komunikasi terakhir (cellular, telephone, unknown)           |
| `day`                  | Hari dalam bulan saat kontak terakhir                                     |
| `month`                | Bulan saat kontak terakhir dilakukan                                      |
| `duration`             | Durasi panggilan terakhir (dalam detik)                                   |
| `campaign`             | Jumlah kontak selama kampanye ini                                         |
| `pdays`                | Jumlah hari sejak nasabah terakhir dikontak dari kampanye sebelumnya      |
| `previous`             | Jumlah kontak yang dilakukan sebelum kampanye ini                         |
| `poutcome`             | Hasil dari kampanye pemasaran sebelumnya (success, failure, unknown)      |
| `deposit`              | Target variabel: apakah nasabah berlangganan deposito berjangka (yes/no)  |

---

## ⚙️ Metodologi

- **Pra-pemrosesan**: Encoding, scaling, handling missing values.
- **Resampling**: Menggunakan RandomOverSampling untuk mengatasi ketidakseimbangan kelas.
- **Modeling**: Algoritma seperti Logistic Regression,KNN, Decision Tree, Random Forest, XGBoost.
- **Tuning**: Hyperparameter tuning untuk meningkatkan performa model.
- **Evaluasi**: Confusion matrix, precision, recall, F1-score, ROC-AUC.
- **Interpretasi**: SHAP values digunakan untuk menginterpretasikan model.
- **Analisis Finansial**: Estimasi biaya salah prediksi untuk keputusan bisnis.

---

## 📌 Hasil Utama

- Fitur `duration` (durasi kontak), `poutcome_success`, dan `balance` adalah yang paling berpengaruh terhadap keberhasilan kampanye.
- Model dapat membantu menyaring nasabah yang berpotensi tinggi untuk dikontak terlebih dahulu.
- Pendekatan berbasis data dapat menghemat biaya kampanye sebesar **39.9%**.

---

## 💡 Rekomendasi Bisnis

- Fokus pada nasabah yang memiliki durasi kontak panjang dan riwayat positif kampanye sebelumnya.
- Hindari kontak berulang kali tanpa hasil yang positif.
- Perbaiki kualitas data kontak nasabah.
- Gunakan model prediksi sebagai filter utama sebelum memulai kampanye.

---

## 📁 Struktur File

- `Bank_Marketing_Analytics_Final.ipynb`: Notebook utama analisis dan modeling.

---

## 🛠 Tools & Teknologi

- Python, Pandas, Scikit-Learn, XGBoost, SHAP, Matplotlib, Seaborn

---
