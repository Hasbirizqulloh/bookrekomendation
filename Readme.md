# Laporan Proyek Machine Learning - Moh Hasbi Rizqulloh

## Project Overview

Sistem rekomendasi adalah teknologi yang saat ini banyak digunakan untuk membantu pengguna dalam memilih produk atau konten berdasarkan preferensi atau perilaku mereka sebelumnya. Dalam dunia digital yang penuh dengan pilihan, sistem rekomendasi memainkan peran penting dalam memberikan pengalaman yang lebih personal dan efisien bagi penggunanya. Rekomendasi yang baik tidak hanya membantu pengguna dalam membuat keputusan lebih cepat, tetapi juga dapat meningkatkan kepuasan mereka dengan menyediakan informasi yang lebih relevan dengan kebutuhan atau minat mereka.

Dalam berbagai aplikasi, mulai dari platform belanja online, media sosial, hingga layanan streaming, sistem rekomendasi telah diterapkan dengan tujuan untuk mempermudah pengguna dalam menemukan produk atau konten yang sesuai dengan keinginan mereka. Sebagai contoh, platform seperti Amazon, Netflix, dan Spotify menggunakan sistem rekomendasi untuk memberikan saran produk, film, atau musik yang relevan. Namun, tantangan utama dalam sistem rekomendasi adalah bagaimana memastikan bahwa rekomendasi yang diberikan benar-benar sesuai dengan preferensi pengguna.

Salah satu metode yang banyak digunakan dalam membangun sistem rekomendasi adalah Collaborative Filtering. Metode ini bekerja dengan menganalisis interaksi pengguna terhadap item (misalnya buku, film, produk) dan mencari hubungan atau kesamaan antara pengguna atau item yang serupa. Dalam konteks proyek ini, sistem rekomendasi akan dibangun untuk buku dengan menggunakan pendekatan Collaborative Filtering, di mana sistem akan memberikan rekomendasi berdasarkan interaksi pengguna dengan buku lainnya. Rekomendasi ini akan didasarkan pada perilaku pengguna yang serupa, sehingga buku yang direkomendasikan adalah buku yang disukai oleh pengguna dengan preferensi serupa.

### Mengapa Proyek Ini Penting?
Dalam dunia digital yang penuh dengan pilihan, pengguna sering merasa kewalahan mencari buku yang sesuai dengan minat mereka. Dengan adanya sistem rekomendasi berbasis Collaborative Filtering, pengguna dapat mendapatkan saran buku berdasarkan apa yang telah disukai atau dibaca oleh pengguna lain dengan preferensi serupa. Hal ini tidak hanya menghemat waktu pengguna dalam mencari buku, tetapi juga meningkatkan pengalaman mereka dengan memberi saran yang lebih relevan. Sistem ini membantu pengguna merasa lebih dihargai, karena rekomendasi yang diberikan lebih bersifat personal.

Selain itu, sistem rekomendasi ini dapat meningkatkan interaksi pengguna dengan platform, mendorong mereka untuk membeli buku yang mungkin sebelumnya tidak mereka pertimbangkan, dan mengenalkan mereka pada buku-buku baru yang relevan. Hal ini berpotensi meningkatkan penjualan buku serta memperluas penggunaan koleksi buku yang ada di platform.

### Solusi yang Akan Dikembangkan
Proyek ini bertujuan untuk membangun sistem rekomendasi buku dengan menggunakan Collaborative Filtering. Sistem ini akan menganalisis data interaksi pengguna terhadap buku, seperti rating atau pembelian buku, untuk mencari pola yang ada di antara pengguna yang memiliki preferensi serupa. Dengan menggunakan pendekatan ini, sistem akan merekomendasikan buku yang sebelumnya disukai oleh pengguna lain yang memiliki kesamaan minat atau preferensi. Oleh karena itu, rekomendasi yang diberikan akan lebih relevan dan personal, meningkatkan pengalaman pengguna dan mendorong peningkatan penjualan serta interaksi yang lebih tinggi dengan platform.
  
### Referensi: 
- [Enhancing Personalized Book Recommender System](https://www.ijana.in/papers/V14I3-11.pdf)
- [Book Recomender System](https://www.irjmets.com/adminroot/uploaddir/research_conference_paper/document/36/36_2023121224120151.pdf)
- [Content-Based Recommender Systems Taxonomy](https://sciendo.com/article/10.2478/fcds-2023-0009)
- [An Aggranized Framewok For Enriching Book Recommendation System](https://ejournal.um.edu.my/index.php/MJCS/article/view/29478)
- [Design and Implementation of Book Recommendation Management System Based on Improved Apriori Algorithm](https://www.scirp.org/journal/paperinformation?paperid=99347)


## Business Understanding

Bagian Business Understanding dalam proyek ini bertujuan untuk mengidentifikasi dan menjelaskan permasalahan yang ada dalam platform penyedia buku, serta menguraikan solusi yang akan dikembangkan melalui penerapan sistem rekomendasi berbasis Collaborative Filtering. Dalam konteks ini, kami akan menganalisis bagaimana sistem rekomendasi dapat membantu pengguna menemukan buku yang lebih relevan dan sesuai dengan minat mereka, sekaligus meningkatkan pengalaman pengguna serta penjualan buku di platform. Proyek ini berfokus pada memberikan solusi untuk masalah-masalah yang ada, termasuk kesulitan pengguna dalam mencari buku yang relevan dan kurangnya rekomendasi yang personal.

### Problem Statements

Pada tahap ini, kita akan memulai dengan menganalisis masalah-masalah utama yang sering dihadapi oleh pengguna platform penyedia buku:
1. Masalah Pilihan Buku yang Berlebihan  
Dengan jumlah buku yang sangat banyak yang tersedia di berbagai platform digital, pengguna sering kali merasa bingung dan kewalahan dalam memilih buku yang sesuai dengan minat mereka. Platform yang menyediakan koleksi buku dalam jumlah besar tanpa adanya sistem rekomendasi yang efektif seringkali membuat pengguna kehilangan arah dalam pencarian mereka. Tanpa adanya pemetaan preferensi yang lebih akurat, pengguna mungkin tidak dapat menemukan buku yang mereka sukai, sehingga kualitas pengalaman mereka berkurang.

2. Kurangnya Rekomendasi yang Relevan  
Banyak platform buku yang tidak mampu memberikan rekomendasi yang sesuai dengan preferensi pengguna. Hal ini menyebabkan pengguna harus menghabiskan waktu yang lebih lama untuk mencari buku yang mereka minati, atau bahkan mereka tidak menemukan buku yang relevan sama sekali. Rekomendasi yang tidak personal atau tidak akurat, seperti yang sering terjadi pada sistem berbasis konten, dapat menurunkan kualitas pengalaman pengguna secara keseluruhan. Dalam konteks Collaborative Filtering, masalah ini timbul karena kurangnya hubungan antar item atau pengguna yang serupa yang bisa digunakan untuk memberikan rekomendasi.

3. Tidak Ada Sistem yang Dapat Meningkatkan Penjualan Buku  
Tanpa adanya sistem rekomendasi yang tepat, pengguna cenderung membeli buku yang sudah mereka kenal, sementara buku-buku baru atau buku lain yang relevan dengan minat mereka mungkin tidak mendapatkan perhatian. Ini mengarah pada penurunan penjualan buku yang dapat dengan mudah ditingkatkan dengan sistem rekomendasi berbasis Collaborative Filtering. Dalam hal ini, pengguna akan lebih mudah menemukan buku baru yang disukai oleh pengguna dengan preferensi serupa, yang akhirnya meningkatkan peluang penjualan buku yang lebih tinggi.

### Goals
Dalam rangka mengatasi permasalahan tersebut, tujuan dari proyek ini adalah:
1. Menyediakan Rekomendasi Buku yang Personalisasi dan Relevan  
Sistem rekomendasi berbasis Collaborative Filtering akan dikembangkan untuk memberikan rekomendasi buku yang relevan berdasarkan interaksi atau preferensi pengguna lainnya. Berbeda dengan Content-Based Filtering yang berfokus pada fitur buku, Collaborative Filtering mengandalkan data pengguna dan hubungan antar pengguna (user-user) atau antar item (item-item) untuk membuat prediksi rekomendasi. Dengan demikian, rekomendasi buku akan lebih personal dan sesuai dengan apa yang mungkin disukai pengguna berdasarkan kesamaan mereka dengan pengguna lain.

2. Meningkatkan Pengalaman Pengguna dengan Rekomendasi yang Akurat  
Salah satu tujuan utama dari proyek ini adalah untuk meningkatkan pengalaman pengguna dengan memberikan rekomendasi yang lebih akurat dan personal. Dengan sistem rekomendasi berbasis Collaborative Filtering, pengguna tidak hanya akan lebih mudah menemukan buku yang mereka suka, tetapi juga merasa lebih dihargai karena platform memahami preferensi mereka berdasarkan interaksi mereka dengan pengguna lain yang serupa.

3. Meningkatkan Penjualan Buku  
Melalui penerapan sistem rekomendasi berbasis Collaborative Filtering, platform penyedia buku diharapkan dapat meningkatkan penjualan buku. Dengan memberikan rekomendasi yang relevan dan menarik bagi pengguna berdasarkan data historis pengguna lainnya, buku yang mungkin sebelumnya tidak dipertimbangkan akan lebih sering dibeli. Hal ini berpotensi meningkatkan pendapatan dan efisiensi dalam penggunaan katalog buku.

### Solution Approach
Untuk mencapai tujuan tersebut, beberapa pendekatan yang akan digunakan dalam mengembangkan sistem rekomendasi berbasis konten antara lain:

1. Collaborative Filtering   
Collaborative Filtering adalah pendekatan yang mengandalkan data interaksi antara pengguna dan item (dalam hal ini buku) untuk membuat prediksi atau rekomendasi. Sistem ini mencari pengguna atau item yang memiliki kesamaan preferensi dengan pengguna tertentu dan memberikan rekomendasi berdasarkan kesamaan tersebut. Ada dua pendekatan utama dalam Collaborative Filtering yang dapat digunakan:

    - User-Based Collaborative Filtering:    
Mencari pengguna yang memiliki preferensi atau pola perilaku yang mirip dengan pengguna target dan memberikan rekomendasi buku yang disukai oleh pengguna-pengguna serupa.

    - Item-Based Collaborative Filtering:   
Mencari item (buku) yang serupa berdasarkan perilaku pengguna lain, dan merekomendasikan item-item serupa kepada pengguna yang belum pernah berinteraksi dengan buku tersebut.

2. Cosine Similarity dan Pearson Correlation  
Cosine Similarity dan Pearson Correlation adalah metode untuk mengukur kemiripan antar item atau antar pengguna. Dengan mengukur kemiripan ini, sistem dapat memberikan rekomendasi buku yang memiliki kesamaan dengan buku yang sudah dibaca atau disukai oleh pengguna, berdasarkan kesamaan perilaku pengguna lainnya.

3. Matrix Factorization   
Matrix Factorization adalah metode yang digunakan untuk menurunkan dimensi matriks pengguna-item, sehingga mengidentifikasi pola tersembunyi antara pengguna dan item yang dapat digunakan untuk prediksi rating atau rekomendasi. Salah satu algoritma yang populer adalah Singular Value Decomposition (SVD). Dengan menggunakan teknik ini, sistem rekomendasi dapat memprediksi rating yang belum diberikan oleh pengguna untuk item tertentu dan memberikan rekomendasi yang lebih akurat.

4. K-Nearest Neighbors (KNN)  
K-Nearest Neighbors (KNN) adalah algoritma yang digunakan untuk mencari tetangga terdekat antara pengguna atau item berdasarkan kemiripan rating atau interaksi. Dalam konteks Collaborative Filtering, KNN akan digunakan untuk mencari pengguna atau buku yang paling mirip dengan pengguna tertentu atau buku yang sudah dibaca oleh pengguna. Sistem akan merekomendasikan buku berdasarkan kesamaan pengguna atau item.


Dengan pendekatan-pendekatan ini, diharapkan sistem rekomendasi yang dibangun akan efektif dalam memberikan saran buku yang relevan, meningkatkan pengalaman pengguna, serta membantu meningkatkan penjualan buku di platform.

## Data Understanding
Proyek ini menggunakan dataset dari platform Book-Crossing Dataset yang tersedia di Kaggle. Dataset ini berisi informasi tentang buku, pengguna, serta penilaian (rating) yang diberikan pengguna terhadap buku tersebut. Dataset ini terdiri dari tiga file utama, yaitu Books.csv, Users.csv, dan Ratings.csv, yang masing-masing memiliki jumlah data sebagai berikut:

- Books.csv: berisi 271.360 entri data mengenai buku, termasuk ISBN, judul, pengarang, tahun terbit, penerbit, serta link gambar sampul dalam berbagai ukuran.

- Users.csv: berisi 278.858 data pengguna yang mencakup ID pengguna, lokasi, dan usia (jika tersedia).

- Ratings.csv: berisi 1.149.780 data rating yang diberikan oleh pengguna terhadap buku tertentu, yang direpresentasikan dalam skala integer dari 0 hingga 10.

### Informasi Dataset
Berikut ini adalah penjabaran variabel dari masing-masing file dalam dataset:

1. Books.csv

      - ISBN: Nomor identifikasi unik untuk setiap buku.

      - Book-Title: Judul buku.

      - Book-Author: Nama pengarang buku.

      - Year-Of-Publication: Tahun buku tersebut diterbitkan.

      - Publisher: Nama penerbit buku.
        
      - Image-URL-S: URL gambar sampul buku dalam ukuran kecil.

      - Image-URL-M: URL gambar sampul buku dalam ukuran sedang.

      - Image-URL-L: URL gambar sampul buku dalam ukuran besar.

2. Users.csv
   
      - User-ID: ID unik dari setiap pengguna.

      - Location: Lokasi pengguna yang umumnya terdiri dari kota, negara bagian, dan negara.

      - Age: Umur pengguna. Nilai ini bersifat opsional dan terdapat banyak nilai yang hilang.
  
3.  Ratings.csv
      - User-ID: ID pengguna yang memberikan rating.

      - ISBN: ID buku yang dinilai.

      - Book-Rating: Nilai rating yang diberikan, berkisar dari 0 (tidak memberikan penilaian) hingga 10 (penilaian tertinggi).

### Visualisasi dan Insight Awal
Sebagai bagian dari exploratory data analysis (EDA), dilakukan analisis univariat terhadap sejumlah fitur utama dalam dataset. Analisis ini bertujuan untuk memahami karakteristik data sebelum masuk ke tahap modeling. Berikut beberapa insight penting:

1. Distribusi Tahun Terbit Buku
Sebagian besar buku dalam dataset diterbitkan antara tahun 1980 hingga 2005, dengan puncaknya terjadi sekitar tahun 2000. Ini mengindikasikan bahwa dataset lebih merepresentasikan buku-buku modern yang kemungkinan besar masih relevan dengan selera pembaca masa kini. Buku-buku yang diterbitkan sebelum tahun 1960 jumlahnya sangat sedikit dan dapat dianggap sebagai data historis.

      ![Deskripsi Gambar](https://drive.google.com/uc?export=view&id=1ceqmWdwoFTOiIL7XUI3GMgFOqzcBq5qy)

2. Top 10 Penerbit Buku
Penerbit Harlequin muncul sebagai penerbit paling dominan dengan lebih dari 7.000 judul buku, diikuti oleh Silhouette dan Pocket. Ketiga penerbit ini dikenal luas sebagai penerbit buku fiksi ringan, khususnya genre roman dan sastra populer. Ini memberi gambaran bahwa koleksi buku dalam dataset memiliki kecenderungan kuat terhadap genre-genre tersebut.

3. Distribusi Rating Buku
Rating dengan nilai 0 mendominasi data, yang kemungkinan besar menunjukkan tidak adanya penilaian yang diberikan (implisit), bukan rating rendah. Sementara itu, rating eksplisit (1–10) cenderung berkonsentrasi di kisaran 8 hingga 10, mengindikasikan bahwa pengguna lebih terdorong memberikan ulasan terhadap buku-buku yang mereka sukai.

      ![Deskripsi Gambar](https://drive.google.com/uc?export=view&id=1mC0bLSaRn7WaKIpuYwPuoYHVxaEdbHMS)

4. Distribusi Umur Pengguna
Rentang usia pengguna menunjukkan puncak pada sekitar usia 30 tahun, yang mencerminkan mayoritas pembaca berada pada tahap dewasa muda. Terdapat nilai-nilai ekstrem, seperti umur 0 hingga 244, yang jelas merupakan outlier dan perlu ditangani sebelum masuk ke proses modeling, terutama jika kolom umur akan digunakan sebagai salah satu fitur.

      ![Deskripsi Gambar](https://drive.google.com/uc?export=view&id=1y4fAiOFIOLBy3iDCEpRkqEi0qIiO4Ihx)

5. Penulis Paling Produktif
Agatha Christie tercatat sebagai penulis paling produktif dalam dataset dengan lebih dari 600 judul buku, diikuti oleh William Shakespeare dan Stephen King. Ini menunjukkan representasi kuat dari penulis klasik dan penulis genre misteri/thriller dalam koleksi buku, yang penting dalam konteks content-based filtering yang mengandalkan metadata buku.

6. Lokasi Pengguna Teratas
Lokasi pengguna paling banyak berasal dari negara-negara berbahasa Inggris, seperti United Kingdom, Canada, Australia, dan USA. Kota dengan jumlah pengguna terbanyak adalah London, UK (2.506 pengguna), disusul oleh Toronto, Canada (2.250 pengguna). Hal ini menunjukkan bias geografis pada data pengguna, yang dapat memengaruhi hasil interpretasi preferensi genre dan rekomendasi buku.

### Kesimpulan
1. Ratings.csv menunjukkan dominasi rating bernilai 0 (lebih dari 50%), yang mengindikasikan adanya banyak data yang tidak valid atau berupa implicit feedback. Meskipun begitu, data ini tetap akan digunakan setelah dilakukan seleksi data dan pembersihan untuk menjaga kualitas input sistem rekomendasi. Hanya data dengan rating eksplisit (1–10) yang akan dipertimbangkan untuk digunakan dalam model rekomendasi, sementara data dengan rating 0 akan dihapus atau diperlakukan sebagai data yang tidak relevan. Rating eksplisit yang valid akan menjadi basis utama untuk membangun hubungan antar pengguna dan item dalam model Collaborative Filtering.

2. Users.csv mengandung lebih dari 39% data usia yang hilang dan juga banyak nilai outlier ekstrem. Untuk itu, data pengguna akan dibersihkan terlebih dahulu, dan nilai usia yang hilang akan ditangani menggunakan teknik imputasi atau dengan menghapus entri yang tidak lengkap. Selain itu, informasi lokasi yang tersedia dalam dataset juga akan dipertimbangkan untuk mengidentifikasi pola preferensi berdasarkan wilayah, meskipun fokus utama tetap pada data rating dan interaksi pengguna.
  
3. Books.csv berisi metadata penting seperti judul, penulis, penerbit, dan tahun terbit buku. Namun, karena pendekatan yang digunakan dalam sistem rekomendasi ini lebih berfokus pada interaksi pengguna dan bukan pada fitur konten buku, sebagian besar metadata dalam dataset ini tidak akan digunakan secara langsung. Namun, informasi ini tetap akan berguna dalam tahap evaluasi untuk memahami karakteristik buku yang direkomendasikan.

4. Mengingat keterbatasan memori, hanya sekitar 10.000 entri dari masing-masing dataset (Books.csv, Ratings.csv, Users.csv) yang akan dipertimbangkan untuk meminimalkan penggunaan sumber daya dan memastikan bahwa proses modeling tetap efisien. Gabungan antara data dari ketiga file ini akan dilakukan dengan mencocokkan User-ID dari Ratings.csv dengan User-ID di Users.csv, serta mencocokkan ISBN dari Ratings.csv dengan ISBN di Books.csv.

Berdasarkan evaluasi tersebut, sistem rekomendasi akan dibangun dengan menggabungkan informasi dari Ratings.csv dan Users.csv, menggunakan pendekatan Collaborative Filtering. Fokus utama akan diberikan pada analisis interaksi pengguna dengan buku, untuk menentukan pola preferensi antar pengguna yang dapat digunakan untuk memberikan rekomendasi buku yang relevan berdasarkan perilaku pengguna serupa.

## Data Preparation
Pada tahap ini, dilakukan serangkaian proses untuk mempersiapkan data agar siap digunakan dalam proses pemodelan sistem rekomendasi berbasis Collaborative Filtering. 


### 1. Pembersihan Data Rating
**Langkah yang Dilakukan:** 

Dihapus semua entri pada Ratings.csv yang memiliki nilai rating 0, karena dianggap sebagai umpan balik implisit atau tidak valid.

**Pertimbangan:**   
Langkah ini dilakukan untuk menjaga kualitas data input serta mengurangi beban memori komputasi.

### 2. Seleksi Data Buku Berdasarkan Data Rating
**Langkah yang Dilakukan:**
- Dari seluruh data rating, diambil seluruh ISBN unik yang muncul.
- Dataset Books.csv kemudian disaring untuk hanya menyertakan buku-buku yang memiliki ISBN yang sesuai dengan data rating tersebut.

**Pertimbangan:**   
Menjamin bahwa semua entri pada data rating memiliki referensi metadata buku yang lengkap pada Books.csv.

### 3. Penggabungan Data Pengguna dengan Rating

**Langkah yang Dilakukan:**  
- Dataset Users.csv digunakan untuk menambahkan informasi terkait pengguna ke dalam data rating yang telah dipilih.
- Data pada Ratings.csv yang memiliki User-ID akan digabungkan dengan data pada Users.csv berdasarkan kolom User-ID untuk memperoleh informasi pengguna seperti lokasi dan usia (meskipun ada data usia yang hilang dan outlier, informasi ini tetap akan ditambahkan).
- Penggabungan ini bertujuan untuk memastikan bahwa rekomendasi yang dihasilkan juga mempertimbangkan faktor demografis pengguna (misalnya, lokasi atau usia pengguna, jika tersedia).

**Pertimbangan:**    
Penggabungan data ini memungkinkan analisis yang lebih mendalam terhadap preferensi pengguna berdasarkan karakteristik demografis mereka.

### 4. Pembersihan Data yang Sudah Digabungkan

**Langkah yang Dilakukan:**
- Outlier pada kolom usia yang ekstrem (misalnya, usia 0 atau 244) akan dihapus atau diganti dengan nilai yang wajar melalui teknik imputasi.
- Data yang hilang pada kolom Age akan ditangani dengan teknik imputasi yang sesuai (misalnya, menggunakan nilai rata-rata atau median).
- Data Location yang kosong atau tidak relevan juga akan dipertimbangkan untuk dibersihkan atau diisi dengan nilai default (misalnya, "Unknown").

**Pertimbangan:**  
Pembersihan ini dilakukan untuk memastikan bahwa data pengguna yang digunakan dalam model bersih, konsisten, dan tidak mengandung nilai ekstrem yang dapat mengganggu hasil rekomendasi.


### 5. Seleksi dan Reduksi Fitur
**Langkah yang Dilakukan:**  

Kolom yang tidak memberikan kontribusi terhadap representasi konten buku seperti `Image-URL-S`, `Image-URL-M`, `Year-Of-Publication`, dan `Image-URL-L` dihapus dari dataset.  

Hanya atribut utama yang dipertahankan, yaitu:  
- `Book-Title`  
- `Book-Author`  
- `Publisher`  


**Pertimbangan:**  
Fitur-fitur tersebut memiliki nilai deskriptif terhadap konten buku dan akan digunakan sebagai dasar dalam proses ekstraksi fitur berbasis teks.

### 6. Penggabungan Ketiga Dataset untuk Persiapan Final

Langkah yang Dilakukan:
- Setelah semua data dibersihkan, dataset Ratings.csv, Books.csv, dan Users.csv akan digabungkan. Data akan digabungkan berdasarkan kolom User-ID (untuk menggabungkan data pengguna dengan rating yang diberikan) dan ISBN (untuk menggabungkan data rating dengan metadata buku).
- Gabungan ini akan menghasilkan sebuah dataset yang komprehensif, yang mencakup informasi pengguna, rating buku, serta metadata buku yang relevan.

**Pertimbangan:**  
Penggabungan ketiga dataset ini memungkinkan untuk membangun sistem rekomendasi yang lebih kaya dan lebih akurat dengan informasi lengkap tentang buku, pengguna, dan preferensi rating.

### 7. Sampling dan Pembagian Data untuk Pelatihan dan Pengujian

**Langkah yang Dilakukan:**
- Setelah data final disiapkan, dilakukan sampling untuk memilih subset data yang lebih kecil untuk pelatihan model. Karena keterbatasan memori, sekitar 10.000 entri akan dipilih dari gabungan ketiga dataset tersebut.
- Pembagian data untuk pelatihan dan pengujian dilakukan menggunakan teknik train-test split, dengan sebagian data digunakan untuk melatih model dan sebagian lainnya digunakan untuk menguji akurasi rekomendasi yang dihasilkan.

**Pertimbangan:**  
Sampling data dan pembagian antara data pelatihan dan pengujian memastikan bahwa model dapat diuji secara objektif sebelum digunakan untuk menghasilkan rekomendasi yang lebih luas.

## Modeling
Tahapan ini membahas mengenai model sistem rekomendasi yang dibangun untuk menyelesaikan permasalahan dalam membantu pengguna menemukan buku yang sesuai dengan minat mereka. Sistem rekomendasi ini menggunakan pendekatan Collaborative Filtering dengan dua algoritma yang berbeda, yaitu User-Based Collaborative Filtering dan Item-Based Collaborative Filtering. Output dari model adalah Top-N Recommendation, yaitu daftar rekomendasi buku terbaik yang dipersonalisasi untuk setiap pengguna.

### 1. User-Based Collaborative Filtering
User-Based Collaborative Filtering mencari kemiripan antar pengguna berdasarkan pola rating yang diberikan terhadap buku. Sistem kemudian merekomendasikan buku-buku yang disukai oleh pengguna lain yang memiliki preferensi serupa.
Algoritma yang Digunakan:  
- K-Nearest Neighbors (KNN) untuk mencari tetangga terdekat antar pengguna.
- Similarity Metric: Cosine Similarity.  

Kelebihan:
- Mudah dipahami dan diimplementasikan.
- Dapat memberikan rekomendasi yang bersifat eksploratif berdasarkan minat komunitas pengguna serupa.   

Kekurangan:
- Sulit bekerja dengan baik jika jumlah pengguna sangat besar (scalability problem).
- Butuh data rating yang cukup banyak (dense data) agar bisa menemukan kesamaan antar pengguna.  
- Mengalami masalah cold-start untuk pengguna baru yang belum pernah memberikan rating.

### 2. Item-Based Collaborative Filtering
Item-Based Collaborative Filtering berfokus pada mencari item (dalam hal ini buku) yang mirip berdasarkan pola rating dari seluruh pengguna. Buku yang mirip dengan buku yang telah disukai pengguna akan direkomendasikan.
Algoritma yang digunakan:  
- K-Nearest Neighbors (KNN)  
- Cosine Similarity antar item.  

Kelebihan:
- Lebih stabil dan akurat dalam banyak kasus karena perilaku terhadap item cenderung konsisten.
- Lebih efisien untuk skala besar, karena jumlah item biasanya lebih sedikit dibanding pengguna.
- Cocok untuk platform dengan banyak pengguna aktif.  

Kekurangan:
- Masih mengalami cold-start jika ada item baru yang belum pernah dirating.
- Rekomendasi cenderung terlalu serupa dengan item sebelumnya (kurang eksploratif).

## Evaluation
Pada bagian ini Anda perlu menyebutkan metrik evaluasi yang digunakan. Kemudian, jelaskan hasil proyek berdasarkan metrik evaluasi tersebut.

Ingatlah, metrik evaluasi yang digunakan harus sesuai dengan konteks data, problem statement, dan solusi yang diinginkan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan formula metrik dan bagaimana metrik tersebut bekerja.

**---Ini adalah bagian akhir laporan---**

_Catatan:_
- _Anda dapat menambahkan gambar, kode, atau tabel ke dalam laporan jika diperlukan. Temukan caranya pada contoh dokumen markdown di situs editor [Dillinger](https://dillinger.io/), [Github Guides: Mastering markdown](https://guides.github.com/features/mastering-markdown/), atau sumber lain di internet. Semangat!_
- Jika terdapat penjelasan yang harus menyertakan code snippet, tuliskan dengan sewajarnya. Tidak perlu menuliskan keseluruhan kode project, cukup bagian yang ingin dijelaskan saja.
