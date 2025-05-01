# Laporan Proyek Machine Learning - Moh Hasbi Rizqulloh

## Project Overview

Sistem rekomendasi adalah teknologi yang saat ini banyak digunakan untuk membantu pengguna dalam memilih produk atau konten berdasarkan preferensi atau perilaku mereka sebelumnya. Dalam dunia digital yang penuh dengan pilihan, sistem rekomendasi memainkan peran penting dalam memberikan pengalaman yang lebih personal dan efisien bagi penggunanya. Rekomendasi yang baik tidak hanya membantu pengguna dalam membuat keputusan lebih cepat, tetapi juga dapat meningkatkan kepuasan mereka dengan menyediakan informasi yang lebih relevan dengan kebutuhan atau minat mereka.

Dalam berbagai aplikasi, mulai dari platform belanja online, media sosial, hingga layanan streaming, sistem rekomendasi telah diterapkan dengan tujuan untuk mempermudah pengguna dalam menemukan produk atau konten yang sesuai dengan keinginan mereka. Sebagai contoh, platform seperti Amazon, Netflix, dan Spotify menggunakan sistem rekomendasi untuk memberikan saran produk, film, atau musik yang relevan. Namun, tantangan utama dalam sistem rekomendasi adalah bagaimana memastikan bahwa rekomendasi yang diberikan benar-benar sesuai dengan preferensi pengguna.

Dalam membangun sistem rekomendasi, dua metode yang banyak digunakan adalah Content-Based Filtering dan Collaborative Filtering. Kedua metode ini bekerja dengan menganalisis interaksi pengguna terhadap item, seperti buku, film, atau produk, untuk menemukan pola kesamaan antara pengguna atau item. Pada proyek ini, sistem rekomendasi akan dikembangkan menggunakan pendekatan Collaborative Filtering. Sistem akan memberikan rekomendasi buku berdasarkan perilaku pengguna lain yang memiliki preferensi serupa. Dengan demikian, buku yang direkomendasikan adalah buku yang disukai oleh pengguna lain dengan minat yang mirip.

### Mengapa Proyek Ini Penting?
Dalam dunia digital yang penuh dengan pilihan, pengguna sering merasa kewalahan dalam menemukan buku yang sesuai dengan minat mereka. Untuk mengatasi tantangan ini, sistem rekomendasi dikembangkan dengan memanfaatkan dua pendekatan utama, yaitu Collaborative Filtering dan Content-Based Filtering.

Melalui Collaborative Filtering, pengguna akan mendapatkan rekomendasi buku berdasarkan preferensi pengguna lain yang memiliki pola kesukaan serupa. Pendekatan ini membantu pengguna menemukan buku-buku yang populer di kalangan individu dengan minat yang mirip, sehingga menghemat waktu pencarian dan meningkatkan relevansi rekomendasi.

Sementara itu, Content-Based Filtering menganalisis karakteristik buku, seperti genre, tema, atau penulis, dan mencocokkannya dengan riwayat preferensi pengguna. Dengan demikian, pengguna dapat memperoleh rekomendasi yang lebih personal berdasarkan kesamaan konten dengan buku yang pernah mereka sukai.

Kombinasi kedua pendekatan ini tidak hanya meningkatkan pengalaman pengguna dengan menyediakan saran yang relevan dan personal, tetapi juga mendorong interaksi yang lebih tinggi dengan platform. Pengguna akan lebih mungkin menemukan dan membeli buku-buku baru yang mungkin sebelumnya tidak mereka pertimbangkan, sekaligus memperluas eksplorasi terhadap koleksi buku yang tersedia. Pada akhirnya, hal ini berpotensi meningkatkan kepuasan pengguna dan mendorong pertumbuhan penjualan buku di platform.


### Solusi yang Akan Dikembangkan
Proyek ini bertujuan untuk membangun sistem rekomendasi buku dengan menggabungkan pendekatan Collaborative Filtering dan Content-Based Filtering. Sistem ini akan menganalisis data interaksi pengguna terhadap buku, seperti pemberian rating, ulasan, atau riwayat pembelian, untuk menemukan pola di antara pengguna yang memiliki preferensi serupa (Collaborative Filtering). Selain itu, sistem juga akan memanfaatkan informasi karakteristik buku, seperti genre, penulis, atau sinopsis, untuk memberikan rekomendasi berdasarkan kesamaan konten dengan buku-buku yang pernah disukai oleh pengguna (Content-Based Filtering).

Dengan kombinasi kedua pendekatan ini, sistem rekomendasi akan mampu memberikan saran buku yang lebih relevan, personal, dan beragam. Solusi ini diharapkan dapat meningkatkan pengalaman pengguna, mempercepat proses pencarian buku yang sesuai, serta mendorong peningkatan penjualan dan interaksi yang lebih tinggi dengan platform.
  
### Referensi: 
- [Enhancing Personalized Book Recommender System](https://www.ijana.in/papers/V14I3-11.pdf)
- [Book Recomender System](https://www.irjmets.com/adminroot/uploaddir/research_conference_paper/document/36/36_2023121224120151.pdf)
- [Content-Based Recommender Systems Taxonomy](https://sciendo.com/article/10.2478/fcds-2023-0009)
- [An Aggranized Framewok For Enriching Book Recommendation System](https://ejournal.um.edu.my/index.php/MJCS/article/view/29478)
- [Design and Implementation of Book Recommendation Management System Based on Improved Apriori Algorithm](https://www.scirp.org/journal/paperinformation?paperid=99347)


## Business Understanding

Bagian ini bertujuan untuk mengidentifikasi dan menjelaskan permasalahan yang dihadapi oleh platform penyedia buku, serta menguraikan solusi yang akan dikembangkan melalui penerapan sistem rekomendasi berbasis Collaborative Filtering dan Content-Based Filtering. Saat ini, pengguna sering mengalami kesulitan dalam menemukan buku yang relevan dengan minat mereka karena keterbatasan sistem rekomendasi yang ada. Kurangnya saran yang personal dan relevan dapat berdampak pada rendahnya tingkat kepuasan pengguna dan minimnya interaksi dengan platform.

Melalui penerapan Collaborative Filtering, sistem akan menganalisis pola interaksi pengguna untuk menemukan kesamaan preferensi dengan pengguna lain, sehingga dapat merekomendasikan buku berdasarkan pilihan pengguna dengan minat serupa. Di sisi lain, Content-Based Filtering akan menganalisis karakteristik buku seperti genre, tema, atau penulis, untuk memberikan rekomendasi berdasarkan kesamaan konten dengan buku-buku yang pernah disukai pengguna.

Proyek ini berfokus pada pengembangan solusi yang mampu meningkatkan relevansi rekomendasi buku, memperkaya pengalaman pengguna, mempercepat pencarian buku yang sesuai, serta mendorong peningkatan penjualan dan keterlibatan pengguna di platform.

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

Untuk mencapai tujuan sistem rekomendasi buku yang relevan dan personal, akan digunakan dua pendekatan utama:

1. Content-Based Filtering  
Content-Based Filtering adalah metode yang merekomendasikan item (buku) berdasarkan kesamaan karakteristik item tersebut dengan preferensi pengguna sebelumnya. Sistem akan menganalisis atribut dari buku, seperti genre, penulis, sinopsis, atau kata kunci, lalu mencocokkannya dengan profil minat pengguna. Dengan teknik ini, rekomendasi yang diberikan lebih bersifat personal karena fokus pada karakteristik konten buku yang disukai pengguna.  
Beberapa metode yang digunakan dalam Content-Based Filtering antara lain:  
    - TF-IDF (Term Frequency-Inverse Document Frequency)    
Untuk mengekstraksi fitur dari deskripsi buku dan menghitung bobot pentingnya kata-kata kunci.
    - Cosine Similarity  
Untuk mengukur tingkat kemiripan antar buku berdasarkan fitur-fitur yang telah diekstraksi, sehingga sistem dapat merekomendasikan buku yang mirip dengan buku yang pernah disukai pengguna.

2. Collaborative Filtering  
Collaborative Filtering adalah metode yang membuat rekomendasi berdasarkan pola interaksi pengguna lain tanpa memperhatikan konten buku itu sendiri. Pendekatan ini mengandalkan kesamaan perilaku antar pengguna atau antar item untuk memprediksi preferensi.  
Collaborative Filtering terdiri dari dua pendekatan:
    - User-Based Collaborative Filtering  
Mencari pengguna dengan pola preferensi serupa, lalu merekomendasikan buku yang disukai oleh pengguna-pengguna tersebut.
    - Item-Based Collaborative Filtering  
Menemukan buku yang sering dikaitkan bersama berdasarkan perilaku pengguna lain, lalu merekomendasikan buku serupa kepada pengguna.
  
    Beberapa metode pendukung Collaborative Filtering:
    - Pearson Correlation dan Cosine Similarity    
Untuk mengukur tingkat kesamaan antar pengguna atau antar item.
    - Matrix Factorization Singular Value Decomposition    
Untuk menemukan pola tersembunyi dalam data besar pengguna-buku dan membuat prediksi rekomendasi yang lebih akurat.
    - K-Nearest Neighbors (KNN)    
Untuk mencari pengguna atau buku yang paling mirip sebagai dasar pemberian rekomendasi.

Dengan menggabungkan kedua pendekatan ini Content-Based Filtering dan Collaborative Filtering, sistem rekomendasi diharapkan dapat memberikan saran buku yang lebih relevan dan personal, meningkatkan pengalaman pengguna, serta mendorong pertumbuhan penjualan buku di platform.

## Data Understanding
Proyek ini menggunakan dataset dari platform Book-Crossing Dataset yang tersedia di [Kaggle](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset). Dataset ini berisi informasi tentang buku, pengguna, serta penilaian (rating) yang diberikan pengguna terhadap buku tersebut. Dataset ini terdiri dari tiga file utama, yaitu Books.csv, Users.csv, dan Ratings.csv, yang masing-masing memiliki jumlah data sebagai berikut:

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
Sebagai bagian dari exploratory data analysis (EDA), dilakukan analisis univariate terhadap sejumlah fitur utama dalam dataset. Analisis ini bertujuan untuk memahami karakteristik data sebelum masuk ke tahap modeling. Berikut beberapa insight penting:

1. Distribusi Tahun Terbit Buku
Sebagian besar buku dalam dataset diterbitkan antara tahun 1980 hingga 2005, dengan puncaknya terjadi sekitar tahun 2000. Ini mengindikasikan bahwa dataset lebih merepresentasikan buku-buku modern yang kemungkinan besar masih relevan dengan selera pembaca masa kini. Buku-buku yang diterbitkan sebelum tahun 1960 jumlahnya sangat sedikit dan dapat dianggap sebagai data historis.

      ![Image](https://github.com/user-attachments/assets/ac4c3af0-bb5c-43b9-a59c-272dfd94ba9a)


3. Top 10 Penerbit Buku
Penerbit Harlequin muncul sebagai penerbit paling dominan dengan lebih dari 7.000 judul buku, diikuti oleh Silhouette dan Pocket. Ketiga penerbit ini dikenal luas sebagai penerbit buku fiksi ringan, khususnya genre roman dan sastra populer. Ini memberi gambaran bahwa koleksi buku dalam dataset memiliki kecenderungan kuat terhadap genre-genre tersebut.

4. Distribusi Rating Buku
Rating dengan nilai 0 mendominasi data, yang kemungkinan besar menunjukkan tidak adanya penilaian yang diberikan (implisit), bukan rating rendah. Sementara itu, rating eksplisit (1–10) cenderung berkonsentrasi di kisaran 8 hingga 10, mengindikasikan bahwa pengguna lebih terdorong memberikan ulasan terhadap buku-buku yang mereka sukai.

      ![download (2)](https://github.com/user-attachments/assets/264a1928-e959-49eb-97b5-c7cdf629a173)


6. Distribusi Umur Pengguna
Rentang usia pengguna menunjukkan puncak pada sekitar usia 30 tahun, yang mencerminkan mayoritas pembaca berada pada tahap dewasa muda. Terdapat nilai-nilai ekstrem, seperti umur 0 hingga 244, yang jelas merupakan outlier dan perlu ditangani sebelum masuk ke proses modeling, terutama jika kolom umur akan digunakan sebagai salah satu fitur.

      ![download (3)](https://github.com/user-attachments/assets/20800dc2-6440-40a5-9699-d527188b3eaf)


8. Penulis Paling Produktif
Agatha Christie tercatat sebagai penulis paling produktif dalam dataset dengan lebih dari 600 judul buku, diikuti oleh William Shakespeare dan Stephen King. Ini menunjukkan representasi kuat dari penulis klasik dan penulis genre misteri/thriller dalam koleksi buku, yang penting dalam konteks content-based filtering yang mengandalkan metadata buku.

9. Lokasi Pengguna Teratas
Lokasi pengguna paling banyak berasal dari negara-negara berbahasa Inggris, seperti United Kingdom, Canada, Australia, dan USA. Kota dengan jumlah pengguna terbanyak adalah London, UK (2.506 pengguna), disusul oleh Toronto, Canada (2.250 pengguna). Hal ini menunjukkan bias geografis pada data pengguna, yang dapat memengaruhi hasil interpretasi preferensi genre dan rekomendasi buku.

### Kesimpulan
1. Ratings.csv menunjukkan dominasi rating bernilai 0 (lebih dari 50%), yang mengindikasikan adanya banyak data yang tidak valid atau berupa implicit feedback. Meskipun begitu, data ini tetap akan digunakan setelah dilakukan seleksi data dan pembersihan untuk menjaga kualitas input sistem rekomendasi. Hanya data dengan rating eksplisit (1–10) yang akan dipertimbangkan untuk digunakan dalam model rekomendasi, sementara data dengan rating 0 akan dihapus atau diperlakukan sebagai data yang tidak relevan. Rating eksplisit yang valid akan menjadi basis utama untuk membangun hubungan antar pengguna dalam item untuk model Collaborative Filtering.

2. Users.csv mengandung lebih dari 39% data usia yang hilang dan juga banyak nilai outlier ekstrem. Untuk itu, data pengguna akan dibersihkan terlebih dahulu, dan nilai usia yang hilang akan ditangani menggunakan teknik imputasi atau dengan menghapus entri yang tidak lengkap. Selain itu, informasi lokasi yang tersedia dalam dataset juga akan dipertimbangkan untuk mengidentifikasi pola preferensi berdasarkan wilayah, meskipun fokus utama tetap pada data rating dan interaksi pengguna.
  
3. Books.csv berisi metadata penting seperti judul, penulis, penerbit, dan tahun terbit buku. Namun, karena pendekatan yang digunakan dalam sistem rekomendasi ini lebih berfokus pada interaksi pengguna dan bukan pada fitur konten buku, sebagian besar metadata dalam dataset ini tidak akan digunakan secara langsung. Namun, informasi ini tetap akan berguna dalam tahap evaluasi untuk memahami karakteristik buku yang direkomendasikan.

4. Mengingat keterbatasan memori, hanya sekitar 10.000 entri dari masing-masing dataset (Books.csv, Ratings.csv, Users.csv) yang akan dipertimbangkan untuk meminimalkan penggunaan sumber daya dan memastikan bahwa proses modeling tetap efisien. Gabungan antara data dari ketiga file ini akan dilakukan dengan mencocokkan User-ID dari Ratings.csv dengan User-ID di Users.csv, serta mencocokkan ISBN dari Ratings.csv dengan ISBN di Books.csv.

Berdasarkan evaluasi tersebut, sistem rekomendasi akan dibangun dengan menggabungkan informasi dari Ratings.csv dan Users.csv, menggunakan pendekatan Content-Based Filtering dan Collaborative Filtering. Fokus utama akan diberikan pada analisis interaksi pengguna dengan buku, untuk menentukan pola preferensi antar pengguna yang dapat digunakan untuk memberikan rekomendasi buku yang relevan berdasarkan perilaku pengguna serupa.

## Data Preparation
Pada tahap ini, dilakukan serangkaian proses untuk mempersiapkan data agar siap digunakan dalam proses pemodelan sistem rekomendasi berbasis Collaborative Filtering. 

### 1. Pembersihan Data 
Pembersihan data dilakukan pada tiga dataset utama: Books.csv, Ratings.csv, dan Users.csv, guna meningkatkan kualitas data untuk analisis dan pemodelan sistem rekomendasi. 
#### Books.csv
Langkah yang Dilakukan:
- Mengonversi kolom Year-Of-Publication menjadi tipe data numerik.
- Mengisi missing values dengan 'Unknown' pada kolom Book-Author, Publisher, Year-Of-Publication, Image-URL-L
- Melakukan seleksi fitur dengan hanya mempertahankan kolom ISBN, Book-Title, Book-Author, Publisher

**Pertimbangan:**   
- Konversi tipe data penting agar kolom tahun publikasi dapat digunakan dalam analisis kuantitatif.
- Pengisian nilai kosong dengan 'Unknown' mencegah error saat pemrosesan tanpa menghilangkan data yang masih berguna.
- Seleksi kolom dilakukan untuk mengurangi kompleksitas data dan fokus pada atribut yang relevan untuk analisis dan rekomendasi.

#### Ratings.csv
Langkah yang Dilakukan:  

Menghapus semua entri yang memiliki nilai rating 0.

Pertimbangan:
- Rating 0 dianggap sebagai interaksi pasif atau umpan balik implisit, bukan penilaian sebenarnya.
- Menghapus data ini akan meningkatkan kualitas input untuk algoritma Collaborative Filtering serta mengurangi beban memori saat pemrosesan.

#### Users.csv
Langkah yang Dilakukan:
- Mengisi missing values pada kolom Age dengan nilai median dari kolom tersebut.
- Menyaring data pengguna, hanya mempertahankan usia dalam rentang 10 hingga 99 tahun.
- Mengisi missing values pada kolom Location dengan 'Unknown'.

Pertimbangan:
- Penggunaan median untuk pengisian nilai Age lebih tahan terhadap outlier dibanding rata-rata.
- Rentang usia 10–99 dianggap sebagai rentang yang valid dan realistis untuk pengguna.
- Mengisi lokasi kosong dengan 'Unknown' menjaga konsistensi data tanpa membuang baris.

### 2. Seleksi Data Buku Berdasarkan Data Rating
**Langkah yang Dilakukan:**
- Dari seluruh data rating, diambil seluruh ISBN unik yang muncul.
- Dataset Books.csv kemudian disaring untuk hanya menyertakan buku-buku yang memiliki ISBN yang sesuai dengan data rating tersebut.

**Pertimbangan:**   
Menjamin bahwa semua entri pada data rating memiliki referensi metadata buku yang lengkap pada Books.csv.

### 3. Penggabungan Data Pengguna dengan Rating

**Langkah yang Dilakukan:**  
- Dataset Users.csv digunakan untuk menambahkan informasi terkait pengguna ke dalam data rating yang telah dipilih.
- Data pada Ratings.csv yang memiliki User-ID akan digabungkan dengan data pada Users.csv berdasarkan kolom User-ID untuk memperoleh informasi pengguna seperti lokasi dan usia. Meskipun ada data usia yang hilang dan outlier, informasi ini tetap akan ditambahkan.
- Penggabungan ini bertujuan untuk memastikan bahwa rekomendasi yang dihasilkan juga mempertimbangkan faktor demografis pengguna misalnya, lokasi atau usia pengguna, jika tersedia.

**Pertimbangan:**    
Penggabungan data ini memungkinkan analisis yang lebih mendalam terhadap preferensi pengguna berdasarkan karakteristik demografis mereka.

### 4. Penggabungan Ketiga Dataset untuk Persiapan Final

Langkah yang Dilakukan:
- Setelah semua data dibersihkan, dataset Ratings.csv, Books.csv, dan Users.csv akan digabungkan. Data akan digabungkan berdasarkan kolom User-ID untuk menggabungkan data pengguna dengan rating yang diberikan dan ISBN untuk menggabungkan data rating dengan metadata buku.
- Cek kembali missing values pada data yang digabungkan karena diduga akan terjadi missing values dari metadata buku yang baru digabungkan.
- Gabungan ini akan menghasilkan sebuah dataset yang komprehensif, yang mencakup informasi pengguna, rating buku, serta metadata buku yang relevan.

**Pertimbangan:**  
Penggabungan ketiga dataset ini memungkinkan untuk membangun sistem rekomendasi yang lebih kaya dan lebih akurat dengan informasi lengkap tentang buku, pengguna, dan preferensi rating.

### 5. Sampling Data

**Langkah yang Dilakukan:**
- Setelah data final disiapkan, dilakukan sampling untuk memilih subset data yang lebih kecil untuk pelatihan model. Karena keterbatasan memori, sekitar 10.000 entri akan dipilih dari gabungan ketiga dataset tersebut.

**Pertimbangan:**  
Sampling data bertujuan untuk mengurangi beban komputasi saat nanti data di training.

## Modeling and Result
### Sistem Rekomendasi yang Dibangun
Untuk menyelesaikan permasalahan dalam memberikan rekomendasi yang relevan kepada pengguna, kami mengembangkan dua pendekatan sistem rekomendasi, yaitu Content-Based Filtering dan Collaborative Filtering. Masing-masing pendekatan menggunakan algoritma yang berbeda untuk mengakomodasi karakteristik data dan kebutuhan pengguna.

### 1. Content-Based Filtering
Pada pendekatan Content-Based Filtering, sistem merekomendasikan buku berdasarkan kesamaan fitur antar buku. Fitur yang digunakan meliputi judul buku, penulis, dan penerbit. Buku yang memiliki karakteristik serupa dengan buku yang disukai pengguna akan direkomendasikan.  
Langkah-langkah:
- Menggabungkan fitur teks seperti Book-Title, Book-Author, dan Publisher.
- Melakukan ekstraksi fitur teks menggunakan TF-IDF Vectorizer.  
- Menghitung kemiripan antar buku menggunakan Cosine Similarity.
- Memberikan top-N rekomendasi item yang paling mirip dengan item yang pernah disukai pengguna.
  
Top-N Recommendation Output:  
Sebagai contoh, untuk seorang pengguna yang menyukai film aksi, sistem merekomendasikan 10 film lain yang memiliki genre serupa dan tingkat kemiripan tinggi. Contoh, untuk pengguna yang menyukai buku "**The Dragon Reborn (The Wheel of Time, Book 3)**", sistem merekomendasikan:                                                                                                                                           
| No | Book Title                                                                 | Book Author     | Predicted Rating |
|----|-----------------------------------------------------------------------------|------------------|------------------|
| 1  | The Eye of the World (The Wheel of Time, Book 1)                           | Robert Jordan    | 10.0             |
| 2  | The Eye of the World (The Wheel of Time, Book 1)                           | Robert Jordan    | 7.0              |
| 3  | The World of Robert Jordan's The Wheel of Time...                          | Robert Jordan    | 7.0              |
| 4  | Lord of Chaos (The Wheel of Time, Book 6)                                  | Robert Jordan    | 6.8              |
| 5  | A Crown of Swords (The Wheel of Time, Book 7)                              | Robert Jordan    | 6.7              |
| 6  | A Crown of Swords (The Wheel of Time, Book 7)                              | Robert Jordan    | 6.6              |
| 7  | A Crown of Swords (The Wheel of Time, Book 7)                              | Robert Jordan    | 6.6              |
| 8  | The Great Hunt: Book Two of 'The Wheel of Time'                            | Robert Jordan    | 6.6              |
| 9  | The Shadow Rising: Book Four of 'The Wheel of Time'                        | Robert Jordan    | 6.3              |
| 10 | The Shadow Rising: Book Four of 'The Wheel of Time'                        | *Unknown*        | 6.3              |

#### 📊 Insight dari Rekomendasi Content-Based untuk 'The Dragon Reborn (The Wheel of Time, Book 3)'
Berdasarkan sistem rekomendasi berbasis konten, hasilnya menunjukkan bahwa buku-buku yang sangat mirip dengan "The Dragon Reborn" adalah buku-buku lain dalam seri "The Wheel of Time" karya Robert Jordan. Ini mencakup buku seperti "The Eye of the World" dan "The Lord of Chaos", yang juga merupakan bagian dari seri yang sama. Hal ini mengonfirmasi bahwa sistem dapat mengenali pola konten yang konsisten di antara buku-buku dalam satu seri.

- Buku dengan peringkat tertinggi: "The Eye of the World" muncul beberapa kali di rekomendasi, dengan peringkat yang sangat tinggi (10.0).
- Buku lain dalam seri yang sama: Banyak buku dari seri "The Wheel of Time", seperti "Lord of Chaos" dan "A Crown of Swords", juga mendapatkan peringkat yang cukup baik (di atas 6.0), menunjukkan bahwa kemiripan tematik dan genre sangat mempengaruhi rekomendasi.
- Peringkat Prediksi: Peringkat prediksi untuk buku-buku terkait berkisar antara 6.3 hingga 10.0, memberikan gambaran bahwa pengguna kemungkinan besar akan tertarik pada buku-buku dalam seri yang sama, dengan variasi dalam tingkat kesukaan.  

Dengan rekomendasi ini, sistem berhasil mengidentifikasi dan menyarankan buku-buku yang sangat relevan, meningkatkan pengalaman pengguna dalam menemukan buku-buku lanjutan dalam seri yang mereka sukai.

----

### 2. Item-Based Collaborative Filtering
Pada pendekatan Collaborative Filtering, sistem menggunakan pola rating pengguna untuk menemukan kesamaan perilaku antar pengguna. Dengan Singular Value Decomposition (SVD), sistem memprediksi rating buku yang belum pernah dinilai oleh pengguna.   
Langkah-langkah:
- Membuat matriks interaksi pengguna-buku berdasarkan User-ID, ISBN, dan Book-Rating.
- Melakukan dekomposisi matriks menggunakan algoritma SVD untuk menemukan representasi laten pengguna dan buku.
- Memperkirakan rating buku yang belum pernah dibaca pengguna.
- Memberikan top-10 rekomendasi buku berdasarkan prediksi rating tertinggi.

Top-10 Recommendation Output:  
Sebagai contoh, sistem merekomendasikan 10 buku yang secara historis disukai oleh pengguna lain yang memiliki pola rating serupa. Contoh, untuk pengguna ID 123284 yang suka dengan buku sebelumnya memberikan rating tinggi untuk "Year of Wonders", sistem merekomendasikan:
| Rank | Book Title                                                                     | Book Author         | Predicted Rating     |
|------|----------------------------------------------------------------------------------|----------------------|-----------------------|
| 1    | A Child's Christmas in Wales                                                    | Dylan Thomas         | 6.93×10⁻¹⁷           |
| 2    | Rainbow Tribe: Ordinary People Journeying on the Red Road                      | Ed McGaa             | 6.93×10⁻¹⁷           |
| 3    | The Compact Trail of Tsathoggua (Call of Cthulhu Role Playing Game Supplement) | Keith Herber         | 6.93×10⁻¹⁷           |
| 4    | Standing Stones: Stonehenge, Carnac and the World of Megaliths                 | Jean Pierre Mohen    | 6.93×10⁻¹⁷           |
| 5    | The Doctors Book of Home Remedies  Revised Edition                             | Prevention Magazine  | 6.93×10⁻¹⁷           |
| 6    | A Dictionary of Sussex Folk Medicine                                            | Andrew Allen         | 6.93×10⁻¹⁷           |
| 7    | Terry Pratchett's "Discworld" Quizbook                                          | David Langford       | 6.93×10⁻¹⁷           |
| 8    | Coyote Waits (Joe Leaphorn/Jim Chee Novels)                                     | Tony Hillerman       | 7.54×10⁻¹⁷           |
| 9    | Sacred Space                                                                    | Denise Linn          | 6.93×10⁻¹⁷           |
| 10   | The Well of Loneliness                                                          | Radclyffe Hall       | 6.93×10⁻¹⁷           |

#### 📊 Insight dari Rekomendasi Item-Based Collaborative Filtering untuk User-ID 123284
Berdasarkan Item-Based Collaborative Filtering, sistem merekomendasikan buku-buku yang serupa dengan buku yang telah diberikan rating oleh pengguna. Berikut adalah beberapa insight dari hasil tersebut:

- Rekomendasi Berdasarkan Kemiripan Item: Rekomendasi buku yang diberikan didasarkan pada kemiripan antara buku yang telah dinilai oleh pengguna dengan buku lainnya. Hal ini menunjukkan bahwa sistem mencari buku-buku dengan pola rating yang serupa untuk memberikan rekomendasi.
- Buku yang Berbeda Genre dan Tema: Sebagai contoh, buku seperti "A Child's Christmas in Wales" dan "Rainbow Tribe" disarankan meskipun genre dan temanya bisa sangat berbeda. Ini menunjukkan bahwa sistem melihat kesamaan dalam rating pengguna, meskipun buku tersebut mungkin memiliki topik yang berbeda.
- Prediksi Rating yang Sangat Rendah: Prediksi rating untuk buku-buku ini, yang semuanya berada di angka sekitar 6.93e-17, mengindikasikan bahwa sistem mungkin mengalami masalah dalam memprediksi rating dengan baik, mungkin karena data sparsity atau kesalahan dalam dekomposisi matriks.
- Rekomendasi yang Tidak Spesifik: Meskipun buku yang disarankan sesuai dengan pola rating pengguna lain, prediksi rating yang hampir sama rendahnya untuk semua buku menunjukkan bahwa sistem belum optimal dalam memberikan rekomendasi yang lebih terpersonalisasi. Data yang lebih kaya atau teknik lain seperti Matrix Factorization atau Deep Learning bisa membantu meningkatkan akurasi prediksi.

🔎 Kesimpulan:
Sistem Item-Based Collaborative Filtering berhasil memberikan rekomendasi berdasarkan kesamaan antar buku. Namun, kualitas rekomendasi dan prediksi rating perlu diperbaiki, mengingat prediksi rating yang rendah untuk sebagian besar buku. Untuk meningkatkan kualitas rekomendasi, teknik tambahan seperti Matrix Factorization atau Penurunan Dimensi bisa dicoba, atau memperkaya data dengan informasi lebih lanjut tentang interaksi pengguna.

---
### 3. User-Based Collaborative Filtering
Pada pendekatan User-Based Collaborative Filtering, sistem menggunakan pola rating pengguna untuk menemukan pengguna lain dengan perilaku yang mirip. Kemudian, sistem merekomendasik
Langkah-langkah:
- Membuat matriks interaksi pengguna-buku berdasarkan User-ID, ISBN, dan Book-Rating.
- Menghitung cosine similarity antar pengguna untuk mengukur tingkat kemiripan preferensi.
- Menentukan k tetangga terdekat (k-nearest neighbors) berdasarkan skor kemiripan tertinggi.
- Menghitung weighted average rating buku dari tetangga terdekat.

Top-10 Recommendation Output:    
Sebagai contoh, sistem merekomendasikan 10 buku yang secara historis disukai oleh pengguna lain dengan pola rating serupa. Contohnya, untuk User-ID 106893, sistem merekomendasikan:

| Rank | Book Title                                                                 | Book Author       | Predicted Rating |
|------|-----------------------------------------------------------------------------|-------------------|------------------|
| 1    | Old Devils                                                                  | Kingsley Amis     | 6.70             |
| 2    | The Polish Way: A Thousand-Year History of the Poles and Their Culture     | Adam Zamoyski     | 5.21             |
| 3    | Vamps and Tramps: New Essays                                                | Camille Paglia    | 2.55             |
| 4    | How to Become a Virgin                                                      | Quentin Crisp     | 2.55             |
| 5    | The Hippopotamus                                                            | Stephen Fry       | 2.55             |
| 6    | Skipped Parts                                                               | Tim Sandlin       | 2.30             |
| 7    | Armadillo                                                                   | William Boyd      | 2.30             |
| 8    | Neverwhere: A Novel                                                         | Neil Gaiman       | 2.30             |
| 9    | Whit                                                                         | Iain Banks        | 2.30             |
| 10   | Careless Love: The Unmaking of Elvis Presley                               | Peter Guralnick   | 2.30             |


#### 📊 Insight dari User-Based CF Recommendations untuk User-ID 106893
Sistem User-Based Collaborative Filtering berhasil memberikan rekomendasi buku untuk User-ID 106893 berdasarkan kemiripan preferensi dengan pengguna lainnya. Berikut adalah beberapa temuan dari hasil rekomendasi:

- Buku dengan Peringkat Prediksi Tertinggi: Buku pertama yang direkomendasikan adalah "Old Devils" oleh Kingsley Amis, dengan rating yang diprediksi cukup tinggi (6.7). Ini menunjukkan bahwa buku tersebut memiliki kemiripan dengan preferensi pengguna.

- Buku dengan Prediksi Rating Lebih Rendah: Buku seperti "The Polish Way" dan "Vamps and Tramps" memiliki rating yang lebih rendah (5.2 dan 2.55), namun tetap termasuk dalam rekomendasi, mengindikasikan bahwa mereka memiliki beberapa kesamaan dengan minat pengguna, meskipun tidak sekuat rekomendasi lainnya.

- Buku Populer dan Tidak Familiar: Ada beberapa buku yang direkomendasikan, seperti "The Hippopotamus" dan "Neverwhere", yang beragam dalam genre dan tema. Ini menunjukkan bahwa sistem memberikan berbagai pilihan berdasarkan keberagaman minat pengguna yang serupa.

- Rentang Prediksi Rating: Prediksi rating untuk buku yang direkomendasikan bervariasi antara 6.7 hingga 2.3. Buku-buku dengan rating rendah kemungkinan besar adalah buku yang relevan dalam konteks genre atau tema, tetapi dengan minat yang lebih terbatas dari pengguna serupa.    


Dengan rekomendasi ini, pengguna diberikan berbagai pilihan buku yang relevan berdasarkan kesamaan rating dari pengguna lain yang memiliki preferensi serupa.

---

## Evaluation
Dalam proyek ini menggunakan beberapa metrik evaluasi yang disesuaikan dengan pendekatan sistem rekomendasi yang diterapkan, yaitu Content-Based Filtering dan Collaborative Filtering.
### 1. Content-Based Filtering dan User-Based Collaborative Filtering (UserCF)
Pada pendekatan Content-Based Filtering dan User-Based Collaborative Filtering (UserCF), model berfokus untuk merekomendasikan item serupa berdasarkan preferensi pengguna. Karena hasil akhirnya adalah daftar item (top-N recommendation), maka evaluasi dilakukan menggunakan Precision@K dan Recall@K.

#### Rumus Precision@K
$$
\text{Precision@K} = \frac{\text{Jumlah item relevan yang direkomendasikan pada Top-K}}{K}
$$

**Penjelasan**:  
Precision@K menilai seberapa akurat rekomendasi yang diberikan oleh sistem. Semakin tinggi precision, semakin banyak rekomendasi yang relevan di antara Top-K hasil yang ditampilkan.

---

#### Rumus Recall@K
$$
\text{Recall@K} = \frac{\text{Jumlah item relevan yang direkomendasikan pada Top-K}}{\text{Jumlah total item relevan}}
$$

**Penjelasan**:  
Recall@K menilai seberapa banyak item relevan yang berhasil ditangkap oleh sistem rekomendasi dari keseluruhan item relevan yang tersedia. Semakin tinggi recall, semakin banyak item relevan yang ditemukan oleh sistem.

## 2. Collaborative Filtering (Item-Based Collaborative Filtering (SVD))
Untuk pendekatan Collaborative Filtering, model berfokus untuk memprediksi rating yang akan diberikan pengguna pada item tertentu. Oleh karena itu, evaluasi dilakukan menggunakan RMSE (Root Mean Squared Error) dan MAE (Mean Absolute Error).

#### Rumus RMSE (Root Mean Squared Error)
$$
\text{RMSE} = \sqrt{\frac{1}{N} \sum_{i=1}^{N} (y_i - \hat{y}_i)^2}
$$

**Penjelasan**:  
RMSE mengukur seberapa besar rata-rata kesalahan kuadrat antara nilai aktual dan nilai prediksi. RMSE memberikan penalti lebih besar terhadap kesalahan prediksi yang besar (outlier), sehingga sangat sensitif terhadap prediksi yang jauh meleset.

---

#### Rumus MAE (Mean Absolute Error)
$$
\text{MAE} = \frac{1}{N} \sum_{i=1}^{N} |y_i - \hat{y}_i|
$$

**Penjelasan**:  
MAE menghitung rata-rata dari selisih absolut antara nilai aktual dan nilai prediksi. MAE memberikan ukuran kesalahan yang lebih "stabil" terhadap outlier dibandingkan RMSE.

---

#### Keterangan
- yᵢ = rating aktual ke-i
- ŷᵢ = rating prediksi ke-i
- N = jumlah observasi (jumlah pasangan data aktual dan prediksi)

### Analisis Evaluasi

#### Content-Based Filtering 
Buku yang Disukai oleh User:    
['Fatal Voyage', 'A Prayer for the Dying', 'I Killed June Cleaver: Modern Moms Shatter the Myth of  Perfect Parenting']

Hasil Rekomendasi Model:    
['Deja Dead', 'Death du Jour', 'Bare Bones : A Novel', 'Bare Bones : A Novel', 'Deadly Decisions', 'Death du Jour', 'Death du Jour', 'Lasst Knochen Sprechen', 'Fatal', 'Fatal']

Evaluation Metrics:
- Precision@5: 0.00
- Recall@5: 0.00

Interpretasi:    
Model Content-Based Filtering yang diterapkan pada dataset ini belum berhasil memberikan rekomendasi yang sesuai dengan buku-buku yang disukai oleh pengguna. Dari 10 buku yang direkomendasikan, tidak ada satu pun yang relevan dengan preferensi yang telah ditunjukkan oleh pengguna. Precision@5 dan Recall@5 yang bernilai 0 menunjukkan bahwa model tidak dapat memberikan rekomendasi yang memadai pada level tersebut.

Beberapa faktor yang dapat menyebabkan hasil ini antara lain:
- Kemiripan Fitur yang Terbatas: Model hanya mengandalkan beberapa fitur seperti judul, penulis, dan penerbit, yang mungkin tidak cukup kuat untuk menangkap nuansa preferensi pengguna. Banyaknya kemiripan kata-kata dalam judul (seperti "Fatal" yang muncul di beberapa buku) bisa menyebabkan model kesulitan dalam membedakan antara buku yang relevan dan yang tidak.
- Evaluasi yang Terpisah dari Training Data: Jika evaluasi dilakukan dengan data yang terpisah dari training data, model mungkin kesulitan memberikan rekomendasi yang relevan pada data yang belum pernah dilihat sebelumnya.
- Fitur yang Tidak Memadai: Penggunaan fitur yang terbatas pada judul, penulis, dan penerbit saja mungkin belum cukup untuk menghasilkan rekomendasi yang tepat. Penggunaan fitur tambahan seperti deskripsi buku atau genre dapat meningkatkan akurasi model.    

Secara keseluruhan, hasil evaluasi ini menunjukkan bahwa ada kebutuhan untuk memperbaiki teknik ekstraksi fitur atau metode similarity yang digunakan, serta mengeksplorasi kemungkinan untuk menggabungkan berbagai teknik lain seperti Collaborative Filtering atau menggunakan model berbasis deep learning untuk meningkatkan kualitas rekomendasi yang dihasilkan. Perbandingan antara **hasil training** dan **hasil evaluasi** menunjukkan adanya gap yang signifikan, yang mengindikasikan bahwa sistem perlu dilakukan penyempurnaan terutama pada bagian **penanganan data pengguna** dan **ekstraksi fitur**.

#### **Kesimpulan dan Rekomendasi**
- **Model Content-Based Filtering** dalam bentuk yang saat ini diterapkan belum memberikan rekomendasi yang memadai pada tahap evaluasi. Meskipun pada **training** hasil prediksi tampak baik, model perlu ditingkatkan dengan memperhatikan fitur yang lebih kaya dan teknik similarity yang lebih baik.
- Evaluasi yang lebih beragam dan penggunaan **hybrid approaches** (misalnya menggabungkan model content-based dengan collaborative filtering) bisa menjadi solusi untuk mengatasi masalah ini.
- Penambahan fitur **metadata** seperti **kategori buku**, **deskripsi singkat**, atau bahkan **review pengguna** bisa meningkatkan hasil rekomendasi secara keseluruhan.

---

#### Item-Based Collaborative Filtering (SVD)  
- RMSE: 7.5156
- MAE: 7.0376

Interpretasi:  
Model Item-Based Collaborative Filtering berbasis Singular Value Decomposition (SVD) menunjukkan kinerja yang kurang optimal dengan nilai RMSE dan MAE yang cukup tinggi, masing-masing 7.5156 dan 7.0376. Kedua metrik ini menunjukkan bahwa prediksi rating yang dihasilkan model masih memiliki kesalahan yang cukup besar dari rating yang sebenarnya diberikan oleh pengguna.

Beberapa faktor yang dapat menyebabkan hasil ini antara lain:
- Sparsity Data: Dalam data yang memiliki banyak nilai kosong (rating yang hilang), model akan kesulitan memberikan prediksi yang akurat. Banyaknya data yang tidak diberi rating bisa mempengaruhi performa model secara signifikan.
- Jumlah Latent Factors yang Kurang Optimal: Penggunaan 20 latent factors dalam dekomposisi SVD mungkin belum cukup untuk menangkap kompleksitas hubungan antara pengguna dan buku. Pengoptimalan jumlah latent factors bisa meningkatkan akurasi model.

Kesimpulan:
- RMSE dan MAE yang tinggi mengindikasikan bahwa model Collaborative Filtering berbasis SVD belum dapat memberikan prediksi yang akurat.
- Rekomendasi yang dihasilkan tidak sesuai dengan rating yang seharusnya diberikan, kemungkinan karena data yang sangat jarang (sparse) atau pemilihan jumlah latent factors yang belum cukup baik.
- Perlu ada upaya untuk mengoptimalkan model, seperti menyesuaikan jumlah latent factors atau menerapkan teknik lain untuk menangani sparsity dalam data, guna meningkatkan kualitas prediksi dan rekomendasi.

#### User-Based Collaborative Filtering (UserCF)
Buku yang Disukai oleh User:    
['The Godforsaken']

Hasil Rekomendasi Model:    
['The Best of Rock: The Essential Cd Guide (The Essential CD Guides)', 'The angry tide: A novel of Cornwall, 1798-9', 'Collins guide to dinosaurs', 'The first Eden: The Mediterranean world and man', "Stalin's nose: Across the face of Europe", 'Girlfriend In a Coma', 'Forms of Devotion: Stories and Pictures', "Black as he's painted", "Little Wolf's Book of Badness", 'Agent In Place']

Evaluation Metrics:
- Precision@10: 0.0000
- Recall@10: 0.0000

Interpretasi:    
Model User-Based Collaborative Filtering saat ini belum mampu memberikan rekomendasi buku yang relevan dengan preferensi pengguna. Meskipun model telah menghitung kesamaan antar pengguna, hasil rekomendasi yang dihasilkan tidak relevan dengan buku yang telah disukai oleh pengguna.
Precision@10 dan Recall@10 yang menunjukkan nilai 0.0000 mengindikasikan bahwa tidak ada satu pun rekomendasi yang relevan dengan buku yang disukai oleh pengguna. Dalam hal ini, tidak ada kesamaan antara buku yang disukai pengguna dengan rekomendasi yang diberikan oleh model.

Perbandingan dengan Hasil Training:    
Ketika melakukan training pada model User-Based Collaborative Filtering, hasil prediksi rating untuk buku-buku yang direkomendasikan cukup tinggi, seperti terlihat pada User-Based CF Recommendations untuk User-ID 106893, dengan prediksi rating yang cukup baik untuk buku-buku seperti Old Devils (6.7) dan The Polish Way (5.2).
- Namun, Precision dan Recall yang rendah pada evaluasi menunjukkan ketidaksesuaian antara prediksi rating dan hasil rekomendasi aktual yang relevan untuk pengguna. Hal ini bisa disebabkan oleh beberapa faktor:
- Keterbatasan Data: Jika data rating pengguna terbatas atau tidak representatif terhadap preferensi mereka, model akan kesulitan menghasilkan rekomendasi yang relevan.
- Model Hyperparameter: Parameter yang digunakan dalam model, seperti jumlah tetangga terdekat (k_neighbors) atau cara menghitung kesamaan antar pengguna, mungkin belum optimal.
- Sparsity dalam Data: Kekurangan interaksi (rating) antara pengguna dan buku dapat menyebabkan model kesulitan untuk menemukan kesamaan yang tepat.

Kesimpulan:    
- Meskipun model User-Based Collaborative Filtering menunjukkan prediksi rating yang tinggi pada tahap training, hasil evaluasi menggunakan Precision@10 dan Recall@10 menunjukkan bahwa model ini belum berhasil merekomendasikan buku yang relevan dengan preferensi pengguna.
- Perlu adanya perbaikan dalam data input atau penyesuaian hyperparameter untuk meningkatkan kualitas rekomendasi. Penyempurnaan model, misalnya dengan mengatasi masalah sparsity atau menggunakan algoritma yang lebih robust, bisa meningkatkan relevansi rekomendasi di masa mendatang.

#### Evaluation Results

| Model                          | Precision@10 | Recall@10 | RMSE   | MAE    |
|---------------------------------|--------------|-----------|--------|--------|
| Content-Based Filtering (CBF)   | 0.0000       | 0.0000    | -      | -      |
| Item-Based Collaborative Filtering | -          | -         | 7.5156 | 7.0376 |
| User-Based Collaborative Filtering | 0.0000     | 0.0000    | -      | -      |

Berdasarkan hasil evaluasi terhadap beberapa pendekatan sistem rekomendasi:

- Content-Based Filtering    
Content-Based Filtering menunjukkan hasil yang sangat rendah pada Precision dan Recall. Tidak ada rekomendasi yang relevan dengan preferensi pengguna yang sudah diketahui. Hal ini menunjukkan bahwa model belum efektif dalam merekomendasikan buku berdasarkan kemiripan konten.

Pelatihan:   
Pada data pelatihan, model berhasil menghasilkan rekomendasi yang cukup relevan, namun pada evaluasi, model kesulitan dalam merekomendasikan buku yang sesuai dengan preferensi pengguna. Ini bisa disebabkan oleh faktor ekstraksi fitur yang tidak cukup representatif atau kurangnya perbedaan fitur antar buku.

- Item-Based Collaborative Filtering (menggunakan SVD)    
Model ini menunjukkan kesalahan prediksi yang cukup tinggi dengan RMSE dan MAE di atas 7. Hal ini mengindikasikan bahwa meskipun sistem dapat melakukan prediksi rating, perbedaan antara rating prediksi dan aktual masih cukup besar.

Pelatihan:     
Sistem dapat memberikan prediksi rating yang cukup baik, tetapi ketepatannya belum optimal. Ini bisa disebabkan oleh sparsity data (kurangnya interaksi antara pengguna dan buku), serta jumlah latent factors yang belum optimal.

- User-Based Collaborative Filtering    
Model User-Based Collaborative Filtering juga tidak memberikan hasil yang relevan untuk rekomendasi. Meskipun ada penghitungan kesamaan antar pengguna, hasil rekomendasi yang diberikan tidak sesuai dengan buku yang telah disukai pengguna.

Pelatihan:     
Pada tahap pelatihan, model ini menunjukkan prediksi rating yang cukup baik, namun tidak efektif dalam mengenali pola kesamaan antar pengguna yang dapat mengarah pada rekomendasi yang relevan.

--- 

Kesimpulan dan Rekomendasi Model:
Dari ketiga pendekatan yang dievaluasi, Item-Based Collaborative Filtering (SVD) terlihat sebagai model yang paling layak untuk dipilih dalam tahap awal, meskipun masih menunjukkan kesalahan prediksi yang signifikan. Model ini memiliki kemampuan untuk menghasilkan prediksi rating numerik yang mendekati kenyataan, yang membuatnya lebih dapat diandalkan sebagai dasar pengembangan sistem rekomendasi berbasis perilaku pengguna.

Alasan memilih Item-Based Collaborative Filtering (SVD):
- Model ini merupakan satu-satunya pendekatan yang dapat memberikan prediksi rating numerik yang relevan, meskipun ada kesalahan yang cukup besar.
- Pendekatan ini memiliki potensi untuk ditingkatkan lebih lanjut dengan perbaikan pada data (misalnya, menangani masalah sparsity) atau penambahan informasi pengguna dan buku melalui teknik hybrid.

### Kesimpulan Evaluasi
Hasil evaluasi sistem rekomendasi menunjukkan bahwa pendekatan yang diterapkan sebagian telah membantu menjawab permasalahan yang dirumuskan dalam tahap Business Understanding:

1. Problem Statement 1 – Masalah Pilihan Buku yang Berlebihan:    
Pendekatan Collaborative Filtering (baik user-based maupun item-based/SVD) bertujuan mengurangi kebingungan pengguna dalam memilih buku dengan memberikan rekomendasi yang dipersonalisasi.
Namun, berdasarkan hasil evaluasi, sistem ini belum mampu menghasilkan rekomendasi yang relevan secara konsisten (Precision@10 dan Recall@10 = 0 untuk user-based, dan RMSE/MAE cukup besar untuk item-based). Ini menunjukkan bahwa masalah kebingungan dalam memilih buku belum terselesaikan secara optimal.

2. Problem Statement 2 – Kurangnya Rekomendasi yang Relevan:    
Content-Based Filtering mencoba menawarkan rekomendasi buku yang mirip dengan buku yang disukai pengguna.
Namun, hasil evaluasi menunjukkan Precision@10 dan Recall@10 = 0, yang berarti rekomendasi yang dihasilkan masih belum cukup relevan dengan preferensi pengguna. Dengan demikian, sistem belum berhasil sepenuhnya menjawab kebutuhan pengguna akan rekomendasi yang lebih personal.

3. Problem Statement 3 – Tidak Ada Sistem untuk Meningkatkan Penjualan Buku:    
Karena relevansi rekomendasi masih rendah, potensi untuk meningkatkan penjualan buku melalui penemuan buku baru juga belum maksimal.
Sistem rekomendasi yang relevan diperlukan untuk mendorong penjualan, tetapi saat ini performa model masih perlu ditingkatkan untuk mencapai tujuan ini.

#### Pencapaian Goals Proyek
Meskipun terdapat banyak ruang untuk perbaikan, beberapa goals proyek tetap tercapai:
- Pengembangan sistem rekomendasi berbasis Collaborative Filtering dan Content-Based Filtering telah berhasil dilakukan sesuai rencana solusi.
- Evaluasi model telah dilakukan menggunakan metrik yang sesuai:
      - Precision@K dan Recall@K untuk mengevaluasi relevansi rekomendasi.
      - RMSE dan MAE untuk mengukur akurasi prediksi rating.
- Penerapan teknik Cosine Similarity dan SVD memungkinkan sistem memahami hubungan antar pengguna dan antar item, sesuai dengan pendekatan yang direncanakan.

Namun, dari segi dampak terhadap tujuan bisnis (meningkatkan relevansi rekomendasi, pengalaman pengguna, dan potensi penjualan), hasil saat ini menunjukkan bahwa performa sistem masih perlu diperbaiki untuk memberikan dampak bisnis yang signifikan.

#### Kesimpulan Akhir
Model rekomendasi yang dikembangkan sudah menjawab sebagian aspek solusi dengan membangun Content-Based dan Collaborative Filtering.
Namun, performa aktual model saat ini belum cukup kuat untuk benar-benar mengatasi masalah utama yang telah dirumuskan. Pengembangan lebih lanjut sangat diperlukan, seperti:
- Peningkatan kualitas data,
- Penambahan informasi metadata buku,
- Penerapan hybrid recommendation system,
- Dan tuning lebih lanjut terhadap model Collaborative Filtering.

Dengan peningkatan ini, diharapkan sistem rekomendasi dapat lebih relevan, personal, dan efektif, sehingga benar-benar mendorong pengalaman pengguna dan pertumbuhan penjualan buku di platform.





