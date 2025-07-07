# Analisis Jejaring Sosial: Opini Publik Terkait "Prabowo" di Twitter (X)

## 📌 Deskripsi Singkat
Proyek ini bertujuan untuk menganalisis pola keterhubungan dan peran pengguna dalam penyebaran opini mengenai tokoh politik *Prabowo Subianto* di platform Twitter (X). Melalui pendekatan **Social Network Analysis (SNA)** dan algoritma seperti **Betweenness Centrality** serta **Community Detection**, proyek ini mengidentifikasi aktor kunci yang memiliki pengaruh besar dalam jaringan penyebaran opini publik.

## 🎯 Fitur dan Tujuan
- Mengumpulkan data opini publik di Twitter dengan kata kunci “Prabowo”.
- Menganalisis struktur jaringan dan aktor-aktor penting melalui berbagai metrik centrality.
- Melakukan visualisasi hubungan antar pengguna dalam jaringan sosial.
- Menerapkan metode *Community Detection* (Girvan-Newman & Spectral Clustering).
- Menyimulasikan penyebaran opini dengan *Independent Cascade Model (ICM)*.

## 📊 Dataset yang Digunakan
Dataset diperoleh melalui proses *web crawling* dengan menggunakan library `Tweet-Harvest` dan mencakup:
- Total 9.056 data tweet terkait “Prabowo” dari Januari–April 2025.
- Fitur utama: `username`, `full_text`, `retweet_count`, `reply_count`, `favorite_count`, `created_at`, `location`, dll.
- Dataset memuat berbagai jenis interaksi sosial seperti reply, mention, retweet, dan quote tweet.

## 🛠️ Teknologi / Library
- Python
- NetworkX
- Matplotlib / Seaborn
- Pandas & Numpy
- Scikit-learn (untuk spectral clustering)
- Tweet-Harvest (untuk crawling data Twitter)

## 📈 Hasil dan Visualisasi
- Akun `@BANGSAygSUJUD` ditemukan sebagai aktor paling sentral berdasarkan berbagai metrik centrality.
- Visualisasi dilakukan untuk menunjukkan 10 besar pengguna dalam Betweenness, Degree, Closeness, dan Eigenvector Centrality.
- Simulasi *Contagion* menunjukkan pola penyebaran opini berdasarkan *Independent Cascade Model*.
- Community Detection:
  - Girvan-Newman: Menghasilkan 207 komunitas dengan nilai modularity 0.3005.
  - Spectral Clustering: Menghasilkan 5 komunitas besar dengan nilai modularity -0.0983.
- Perbandingan menunjukkan Girvan-Newman lebih efektif dalam mendeteksi komunitas berdasarkan konteks topik dan waktu.

---

