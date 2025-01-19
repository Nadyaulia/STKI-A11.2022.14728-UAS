1. Judul / Topik Project dan Identitas Lengkap

Judul: Deteksi Spam dalam Dokumen Email Menggunakan Teknik Pemrosesan Teks
Identitas:

Nama: Nadya Aulia Almas

NIM: A11.2022.14728

Kelas: A11.4701

2. Ringkasan dan Permasalahan Project

-** Ringkasan:**
Proyek ini bertujuan untuk mendeteksi email spam menggunakan teknik pemrosesan teks dan machine learning. Dataset yang digunakan terdiri dari pesan email yang diberi label sebagai "ham" (bukan spam) atau "spam". Teknik seperti eksplorasi data, ekstraksi fitur, dan pembelajaran mesin digunakan untuk membangun model deteksi yang akurat.

-** Permasalahan:**

Bagaimana cara memproses data teks untuk menghasilkan fitur yang relevan?

Model pembelajaran mesin apa yang dapat memberikan akurasi terbaik?

-** Tujuan:**

Mengidentifikasi email spam dengan akurasi tinggi.

Mengoptimalkan proses ekstraksi fitur menggunakan metode TF-IDF.

Mengukur performa model menggunakan metrik evaluasi seperti akurasi dan confusion matrix.

- **Alur Penyelesaian (Bagan):**

Memuat Dataset

Eksplorasi Data (EDA)

Preprocessing dan Ekstraksi Fitur

Pemodelan (Logistic Regression)

Evaluasi dan Interpretasi Hasil

3. Penjelasan Dataset, EDA, dan Proses Features Dataset

- **Dataset:**

Sumber data: Sumber Kaagle File CSV bernama datasetemail.csv.

Kolom penting:

v1: Label (ham/spam).

v2: Teks email.

- **EDA (Exploratory Data Analysis):**

Dataset memiliki dua kategori: ham dan spam.

Analisis distribusi data menunjukkan bahwa kategori "ham" lebih dominan.

-** Proses Features Dataset:**

Membersihkan data:

Menghapus kolom yang tidak relevan (Unnamed: 2, Unnamed: 3, Unnamed: 4).

Memastikan tidak ada data kosong.

Ekstraksi Fitur:

Menggunakan teknik TF-IDF untuk mengonversi teks menjadi vektor numerik.

4. Proses Learning / Modeling

Model: Logistic Regression digunakan sebagai algoritma klasifikasi karena kesederhanaan dan efektivitasnya untuk teks pendek.

Split Data:

Dataset dibagi menjadi data latih (80%) dan data uji (20%).

Langkah Pemodelan:

Ekstraksi fitur dengan TF-IDF.

Melatih model Logistic Regression pada data latih.

Menguji model pada data uji.

5. Performa Model

Confusion Matrix:

True Positive: [1, 1]

True Negative: [0, 0]

False Positive: [0, 1]

False Negative: [1, 0]

Laporan Klasifikasi:

Accuracy :  0.9613152804642167
Precision :  0.9592274678111588
Recall :  0.9977678571428571
Specificity :  0.7246376811594203

6. Diskusi Hasil dan Kesimpulan

Diskusi:

Model Logistic Regression memberikan performa yang memuaskan dengan akurasi lebih dari 90%.

Teknik TF-IDF efektif dalam mengekstraksi fitur relevan dari teks email.

Kategori spam cenderung lebih sulit diklasifikasikan dibandingkan ham.

Kesimpulan:

Proyek ini menunjukkan bahwa Logistic Regression dan TF-IDF dapat digunakan untuk mendeteksi email spam secara efektif.

Dengan optimasi lebih lanjut (misalnya, tuning hyperparameter), performa model dapat ditingkatkan lebih jauh.
