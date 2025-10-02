🧩 Customer Segmentation with KMeans and PCA
📌 Deskripsi

Proyek ini bertujuan untuk melakukan clustering (segmentasi) pada dataset menggunakan algoritma KMeans.
Proses melibatkan data cleaning, preprocessing, reduksi dimensi dengan PCA, serta evaluasi hasil clustering.
Dataset diambil dari Google Drive dan diproses menggunakan Google Colab.

📂 Informasi Dataset

Dataset ini menyajikan gambaran mendalam mengenai perilaku transaksi dan pola aktivitas keuangan, sehingga sangat ideal untuk eksplorasi deteksi penipuan (fraud detection) dan identifikasi anomali.

Jumlah sampel: 2.512 transaksi

Isi dataset: atribut transaksi, demografi nasabah, dan pola penggunaan

Fitur Utama:

TransactionID → Pengidentifikasi unik alfanumerik untuk setiap transaksi.

AccountID → ID unik untuk setiap akun, dapat memiliki banyak transaksi.

TransactionAmount → Nilai transaksi (dalam mata uang).

TransactionDate → Tanggal dan waktu transaksi terjadi.

TransactionType → Jenis transaksi: Credit atau Debit.

Location → Lokasi geografis transaksi (nama kota di Amerika Serikat).

DeviceID → ID perangkat yang digunakan dalam transaksi.

IP Address → Alamat IPv4 saat transaksi, dapat berubah.

MerchantID → ID unik merchant.

AccountBalance → Saldo akun setelah transaksi berlangsung.

PreviousTransactionDate → Tanggal transaksi terakhir pada akun.

Channel → Kanal transaksi (Online, ATM, Branch).

CustomerAge → Usia pemilik akun.

CustomerOccupation → Profesi pengguna (Dokter, Insinyur, Mahasiswa, Pensiunan).

TransactionDuration → Lama waktu transaksi (detik).

LoginAttempts → Jumlah upaya login sebelum transaksi.

Setiap entri memberikan wawasan komprehensif terhadap perilaku transaksi, memungkinkan analisis untuk keamanan finansial dan pengembangan model prediktif.

⚙️ Tahapan Proses

Import Library & Load Dataset

Eksplorasi Data & Visualisasi Informasi

Data Preprocessing (handling missing value, duplikat, outlier, encoding, scaling, binning)

Clustering dengan KMeans

PCA (Principal Component Analysis)

Inverse Transform & Integrasi Hasil Cluster

Analisis Deskriptif

📊 Output yang Dihasilkan

Dataset hasil cluster: data_clustering.csv

Dataset hasil inverse + cluster: data_clustering_inverse.csv

Model PCA: PCA_model_clustering.h5

Visualisasi clustering dan PCA

📦 Dependensi
pip install pandas numpy matplotlib seaborn scikit-learn joblib

🚀 Cara Menjalankan

Clone repository:

git clone https://github.com/username/repo-name.git
cd repo-name


Buka notebook di Google Colab atau Jupyter Notebook.

Jalankan cell sesuai urutan preprocessing → clustering → PCA → inverse → simpan data.

📑 Catatan

Dataset diambil dari Google Drive: Dataset Link

Seluruh eksperimen dilakukan di Google Colab.
