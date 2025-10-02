🧩 Customer Segmentation with KMeans and PCA
📌 Deskripsi

Proyek ini bertujuan untuk melakukan clustering (segmentasi) pada dataset menggunakan algoritma KMeans.
Proses melibatkan data cleaning, preprocessing, reduksi dimensi dengan PCA, serta evaluasi hasil clustering.
Dataset diambil dari Google Drive dan diproses menggunakan Google Colab.

⚙️ Tahapan Proses

Import Library & Load Dataset

Import library utama (pandas, numpy, matplotlib, seaborn, sklearn, joblib).

Load dataset dari Google Drive.

Eksplorasi Data

Menampilkan informasi dasar dataset.

Visualisasi data (histogram, distribusi, heatmap korelasi, dll).

Visualisasi tambahan yang lebih informatif (pairplot, countplot, dsb).

Data Preprocessing

Menangani missing value (dropna / fillna).

Menghapus duplikat (drop_duplicates).

Handling outlier data.

Melakukan binning pada fitur numerik dan encoding hasil binning.

Encoding variabel kategorikal (LabelEncoder).

Scaling fitur numerik (StandardScaler / MinMaxScaler).

Clustering dengan KMeans

Menentukan jumlah cluster optimal (Elbow Method & Silhouette Score).

Membuat model KMeans.

Visualisasi hasil clustering.

PCA (Principal Component Analysis)

Reduksi dimensi data menjadi 2–3 komponen.

Visualisasi data setelah PCA.

Membuat model KMeans baru dengan data hasil PCA.

Menyimpan model PCA dengan joblib.dump().

Inverse Transform & Penyimpanan Data

Mengembalikan data numerik hasil scaling ke rentang normal.

Mengembalikan data kategorikal hasil encoding ke kategori asli.

Mengintegrasikan kembali data hasil inverse dengan cluster.

Menyimpan dataset hasil cluster (data_clustering.csv) dan hasil inverse + cluster (data_clustering_inverse.csv).

Analisis Deskriptif

Analisis statistik (mean, min, max) untuk numerik.

Mode untuk fitur kategorikal.

Agregasi dan groupby berdasarkan cluster.

📊 Output yang Dihasilkan

Dataset hasil cluster: data_clustering.csv

Dataset hasil inverse + cluster: data_clustering_inverse.csv

Model PCA: PCA_model_clustering.h5

Visualisasi clustering dan PCA

📦 Dependensi

Pastikan environment sudah terpasang library berikut:

pip install pandas numpy matplotlib seaborn scikit-learn joblib

🚀 Cara Menjalankan

Clone repository ini:

git clone https://github.com/username/repo-name.git


Masuk ke folder project:

cd repo-name


Buka notebook di Google Colab atau Jupyter Notebook.

Jalankan cell sesuai urutan dari preprocessing → clustering → PCA → inverse → simpan data.

📑 Catatan

Dataset diambil dari Google Drive: Dataset Link

Seluruh eksperimen dilakukan di Google Colab.
