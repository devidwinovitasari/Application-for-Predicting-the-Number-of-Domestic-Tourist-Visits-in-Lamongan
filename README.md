🌊 Dashboard Prediksi Jumlah Kunjungan Wisatawan Kabupaten Lamongan

📌 Deskripsi Aplikasi
Aplikasi ini merupakan dashboard interaktif berbasis Streamlit yang digunakan untuk melakukan prediksi jumlah kunjungan wisatawan nusantara di Kabupaten Lamongan menggunakan metode hybrid:
CEEMDAN–ELM yang dioptimasi dengan PSO
Metode ini menggabungkan:
🔹 CEEMDAN (Complete Ensemble Empirical Mode Decomposition with Adaptive Noise)
🔹 ELM (Extreme Learning Machine)
🔹 PSO (Particle Swarm Optimization)

Aplikasi ini dirancang sebagai implementasi penelitian forecasting time series untuk meningkatkan akurasi prediksi data kunjungan wisatawan bulanan.
🎯 Tujuan Aplikasi
1. Melakukan dekomposisi data time series menggunakan CEEMDAN
2. Melatih model ELM pada setiap komponen IMF
3. Mengoptimasi parameter ELM menggunakan PSO
4. Menggabungkan kembali hasil prediksi seluruh komponen
5. Menghasilkan prediksi 12 bulan ke depan
6. Menyediakan visualisasi interaktif untuk analisis hasil

🧠 Metodologi yang Digunakan
1️⃣ Preprocessing
1. Membersihkan dan mempersiapkan data
2. Menangani nilai 0/pecilan
3. Normalisasi data menggunakan MinMaxScaler
2️⃣ Dekomposisi Menggunakan CEEMDAN
Data time series dipecah menjadi:
1. Beberapa komponen IMF (Intrinsic Mode Functions)
2. Residual/trend
Tujuannya untuk:
1. Mengurangi non-linearitas
2. Mengatasi non-stasioneritas
3. Mempermudah proses pembelajaran model
Library yang digunakan:
PyEMD/EMD-Signal
3️⃣ Modelling dengan ELM
Setiap komponen IMF dilatih menggunakan:
1. Single hidden layer
2. Aktivasi sigmoid
3. Ridge Regression untuk output weight
Kelebihan ELM:
1. Training sangat cepat
2. Cocok untuk time series non-linear
4️⃣ Optimasi dengan PSO
1. Parameter model dioptimasi menggunakan:
2. Particle Swarm Optimization
Library: pyswarms
Tujuannya untuk:
1. Meningkatkan akurasi model
2. Meminimalkan error (MAPE)
5️⃣ Evaluasi Model
Model dievaluasi menggunakan:
1. MAPE (Mean Absolute Percentage Error)

📊 Fitur Utama Dashboard
Aplikasi terdiri dari beberapa tahapan interaktif:
🏠 Home
📂 Upload Data
🧹 Preprocessing
📉 Dekomposisi CEEMDAN
⚙️ Normalisasi
✂️ Split Data
🤖 Modelling
📈 Prediksi

🌐 Live Demo
Aplikasi dapat diakses melalui:
https://aplikasi-prediksi-kabupaten-lamongan.streamlit.app/

👩‍💻 Author
Devi Dwi Novitasari
Data Science & Forecasting Enthusiast
Fokus pada Time Series Analysis dan Hybrid Machine Learning Model
