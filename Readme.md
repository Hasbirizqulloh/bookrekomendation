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

### Goals
Dalam rangka mengatasi permasalahan tersebut, tujuan dari proyek ini adalah:
1. Menyediakan Rekomendasi Buku yang Personalisasi dan Relevan  
Sistem rekomendasi berbasis Collaborative Filtering akan dikembangkan untuk memberikan rekomendasi buku yang relevan berdasarkan interaksi atau preferensi pengguna lainnya. Berbeda dengan Content-Based Filtering yang berfokus pada fitur buku, Collaborative Filtering mengandalkan data pengguna dan hubungan antar pengguna (user-user) atau antar item (item-item) untuk membuat prediksi rekomendasi. Dengan demikian, rekomendasi buku akan lebih personal dan sesuai dengan apa yang mungkin disukai pengguna berdasarkan kesamaan mereka dengan pengguna lain.

2. Meningkatkan Pengalaman Pengguna dengan Rekomendasi yang Akurat  
Salah satu tujuan utama dari proyek ini adalah untuk meningkatkan pengalaman pengguna dengan memberikan rekomendasi yang lebih akurat dan personal. Dengan sistem rekomendasi berbasis Collaborative Filtering, pengguna tidak hanya akan lebih mudah menemukan buku yang mereka suka, tetapi juga merasa lebih dihargai karena platform memahami preferensi mereka berdasarkan interaksi mereka dengan pengguna lain yang serupa.


### Solution Approach

Untuk mencapai tujuan sistem rekomendasi buku yang relevan dan personal, akan digunakan dua pendekatan utama:

1. Content-Based Filtering  
Content-Based Filtering merekomendasikan buku berdasarkan kesamaan konten dengan buku yang pernah disukai pengguna. Sistem menganalisis atribut buku seperti judul, penulis, dan kata kunci yang diturunkan dari metadata buku.
Teknik yang digunakan:  
    - TF-IDF (Term Frequency-Inverse Document Frequency)    
Untuk mengekstraksi fitur dari deskripsi buku dan menghitung bobot pentingnya kata-kata kunci.
    - Cosine Similarity  
Untuk mengukur tingkat kemiripan antar buku berdasarkan fitur-fitur yang telah diekstraksi, sehingga sistem dapat merekomendasikan buku yang mirip dengan buku yang pernah disukai pengguna.
Pendekatan ini efektif untuk menangkap kemiripan tematik, terutama untuk seri buku atau penulis dengan gaya khas.

2. Neural Collaborative Filtering (NCF)  
Neural Collaborative Filtering adalah pendekatan deep learning yang memodelkan interaksi non-linear antara pengguna dan item. NCF tidak memerlukan informasi konten, melainkan belajar dari pola interaksi historis pengguna.    
Langkah-langkah utama:

- Penggunaan embedding layers untuk merepresentasikan User dan Item (ISBN) dalam bentuk vektor.
- Pemrosesan vektor melalui jaringan neural yang mempelajari hubungan kompleks antara pengguna dan buku.
- Model dilatih untuk meminimalkan error prediksi rating terhadap data yang tersedia.
- Evaluasi dilakukan menggunakan Root Mean Squared Error (RMSE) untuk mengukur akurasi prediksi rating, serta visualisasi training loss untuk memantau proses pelatihan.

Dengan kombinasi CBF dan NCF, sistem rekomendasi ini mampu memberikan rekomendasi berbasis kesamaan konten buku (CBF) dan rekomendasi berbasis pola perilaku pengguna (NCF). Pendekatan ini diharapkan memberikan saran buku yang lebih personal dan relevan, sekaligus mengatasi keterbatasan masing-masing metode jika digunakan secara terpisah.

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
- Cek kembali missing values pada data yang digabungkan karena diduga akan terjadi missing values dari metadata buku yang baru digabungkan. Hapus missing values pada Book-Title, Book-Author, dan Publisher karena terdeteksi 49829 missing valuesnya langsung drop saja karena tidak akan mengurangi informasi dari data mengingat datanya sangat banyak 433671 baris data.
- Gabungan ini akan menghasilkan sebuah dataset yang komprehensif, yang mencakup informasi pengguna, rating buku, serta metadata buku yang relevan.

**Pertimbangan:**  
Penggabungan ketiga dataset ini memungkinkan untuk membangun sistem rekomendasi yang lebih kaya dan lebih akurat dengan informasi lengkap tentang buku, pengguna, dan preferensi rating.

### 5. Sampling Data, Encode, dan Splitting Data

**Langkah yang Dilakukan:**

- Setelah data final disiapkan, dilakukan sampling untuk memilih subset data yang lebih kecil untuk pelatihan model. Karena keterbatasan memori, sekitar 10.000 entri akan dipilih dari gabungan ketiga dataset tersebut.

- Selanjutnya, dilakukan proses **encoding** terhadap kolom `User-ID` dan `ISBN`. Karena kedua kolom ini bersifat kategorikal (berisi string atau kode unik), perlu diubah menjadi nilai numerik menggunakan `LabelEncoder`. Hal ini penting karena sebagian besar algoritma machine learning hanya dapat memproses data numerik. (Khusus untuk Colaborative Filtering)

- Setelah data dalam bentuk numerik siap, dataset dibagi menjadi dua bagian menggunakan metode **train-test split**: 80% data untuk pelatihan dan 20% data untuk pengujian. Ini bertujuan agar performa model dapat dievaluasi pada data yang belum pernah dilihat sebelumnya. (Khusus untuk Colaborative Filtering)

**Pertimbangan:**  
- Sampling data bertujuan untuk mengurangi beban komputasi saat pelatihan model, tanpa harus mengolah seluruh data asli yang jauh lebih besar.  
- Encoding memungkinkan sistem memahami data kategorikal dalam bentuk angka yang dapat dimanfaatkan model.  
- Train-test split penting untuk mengevaluasi kemampuan generalisasi model dan mencegah overfitting terhadap data pelatihan.


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

Kelebihan:
- Rekomendasi berdasarkan preferensi individu pengguna.
- Tidak memerlukan data dari pengguna lain untuk merekomendasikan buku.
- Buku baru bisa direkomendasikan jika memiliki fitur yang jelas.

Kekurangan:
- Kurang Diversitas membuat rekomendasi cenderung terbatas pada buku dengan fitur yang mirip.
- Sulit Menangkap Nuansa sehingga tidak dapat menangkap preferensi yang lebih kompleks di luar fitur eksplisit.
- Bergantung pada Kualitas Fitur dan keberhasilan sistem sangat tergantung pada kelengkapan dan akurasi fitur yang ada.

  
Top-N Recommendation Output:  
Sebagai contoh, untuk seorang pengguna yang menyukai buku dalam seri tertentu, sistem merekomendasikan 10 buku lain yang memiliki penulis serupa dan tingkat kemiripan tinggi. Contoh, untuk pengguna yang menyukai buku "**The Dragon Reborn (The Wheel of Time, Book 3)**", sistem merekomendasikan:                                                                                                                                           
| Rank | Judul Buku | Penulis | Penerbit | Predicted Rating |
|------|------------|---------|----------|------------------|
| 1 | *The Eye of the World (The Wheel of Time, Book 1)* | Robert Jordan | Tor Fantasy | 7.0 |
| 2 | *The World of Robert Jordan's The Wheel of Time* | Robert Jordan | Tor Books | 6.8 |
| 3 | *Lord of Chaos (The Wheel of Time, Book 6)* | Robert Jordan | Tor Fantasy | 6.7 |
| 4 | *A Crown of Swords (The Wheel of Time, Book 7)* | Robert Jordan | Tor Fantasy | 6.6 |
| 5 | *The Great Hunt : Book Two of 'The Wheel of Time'* | Robert Jordan | Tor Books | 6.3 |
| 6 | *The Shadow Rising : Book Four of 'The Wheel of Time'* | Robert Jordan | Tor Books | 6.3 |
| 7 | *Winter's Heart (The Wheel of Time, Book 9)* | Robert Jordan | Tor Books | 6.1 |
| 8 | *Earthquake Weather (Tor Fantasy)* | Tim Powers | Tor Books | 2.6 |
| 9 | *Into the Darkness (World at War, Book 1)* | Harry Turtledove | Tor Fantasy | 2.5 |
|10 | *Mount Dragon: A Novel* | Douglas Preston | Tor Books | 2.4 |

---

#### 📊 Insight dari Rekomendasi Content-Based untuk 'The Dragon Reborn (The Wheel of Time, Book 3)'
- Buku-buku yang direkomendasikan **mayoritas berasal dari seri yang sama** (*The Wheel of Time*), menunjukkan bahwa pendekatan content-based sangat efektif dalam mengenali keterkaitan konten berdasarkan judul, penulis, dan penerbit.
- **Robert Jordan** mendominasi hasil rekomendasi, menunjukkan bahwa fitur penulis berpengaruh kuat terhadap kemiripan.
- Buku dari penerbit **Tor Books** dan **Tor Fantasy** juga sering muncul, mengindikasikan bahwa penerbitan juga menjadi sinyal penting dalam penilaian kemiripan.
- Tiga rekomendasi terbawah memiliki prediksi rating yang lebih rendah (sekitar 2.4–2.6), mungkin karena hanya berbagi kesamaan dari penerbit atau genre luas, bukan seri atau penulis.

----

### 2. Neural Collaborative Filtering (NCF)

Pada pendekatan **Neural Collaborative Filtering (NCF)**, sistem menggunakan pola interaksi pengguna dan item (seperti buku) untuk memprediksi rating atau preferensi yang belum diberikan oleh pengguna. NCF menggunakan model berbasis **neural network** yang lebih fleksibel dan dapat menangkap hubungan non-linear antara pengguna dan item. 

Langkah-langkah:
- **Membuat Matriks Interaksi Pengguna-Item** dengan menggunakan **User-ID**, **Item-ID** (misalnya ISBN), dan **Rating** untuk membangun matriks interaksi. Matriks ini berisi data rating yang diberikan pengguna terhadap item (buku).
- Membangun **Model NCF** dengan menggunakan jaringan saraf, **embedding layer** digunakan untuk merepresentasikan pengguna dan item dalam bentuk vektor laten. Vektor-vektor ini kemudian digabungkan melalui lapisan **MLP (Multilayer Perceptron)** untuk memprediksi rating.
- Model dilatih untuk meminimalkan **loss function** yaitu, **MSE Loss**, dengan memperkirakan rating yang belum pernah diberikan oleh pengguna.
- Setelah model terlatih, prediksi rating dilakukan untuk item-item yang belum dinilai oleh pengguna, dan kemudian diberikan **top-10 rekomendasi buku** berdasarkan rating tertinggi.

Kelebihan:
- Dengan menggunakan **neural network**, NCF dapat menangkap hubungan non-linear dan interaksi kompleks antara pengguna dan item yang lebih sulit dipecahkan oleh model tradisional seperti SVD.
- Dengan **embedding layer** dan **MLP**, NCF dapat menangani masalah sparsity dalam data rating dengan baik. Embedding memungkinkan model untuk belajar representasi laten yang efektif meskipun data interaksi pengguna dan item tidak lengkap.
- Dapat memberikan rekomendasi yang lebih relevan dengan memprediksi rating pada item yang belum pernah dinilai, bahkan untuk item baru (cold start problem).

Kekurangan:
- NCF membutuhkan jumlah data yang besar untuk dapat melatih model yang efektif. Semakin banyak data interaksi pengguna-item, semakin baik model dalam memberikan rekomendasi.
- Sama seperti model berbasis collaborative filtering lainnya, NCF mengalami kesulitan dalam merekomendasikan item baru atau pengguna baru yang tidak memiliki cukup data interaksi.
- Proses pelatihan model NCF, terutama untuk dataset yang besar, membutuhkan waktu dan sumber daya komputasi yang lebih banyak dibandingkan dengan teknik tradisional seperti SVD.


Top-10 Recommendation Output:  
Berikut adalah daftar **top-10 rekomendasi buku** untuk pengguna yang dihasilkan oleh model **Neural Collaborative Filtering (NCF)**.

| No | Book Title | Author | Publisher | ISBN |
|----|------------|--------|-----------|------|
| 1  | Holes (Newbery Medal Book) | Louis Sachar | Farrar, Straus and Giroux (BYR) | 0374332657 |
| 2  | Cryptonomicon | Neal Stephenson | Avon | 0380973464 |
| 3  | The Blue Viking | Sandra Hill | Leisure Books | 0843948272 |
| 4  | Acts of the Apostles | John F. X. Sundman | Rosalita Associates | 192975213X |
| 5  | El fantasma de Canterville/El retrato de Dorian Gray/De profundis/La importancia de llamarse Ernesto/El abanico de Lady Windermere | Oscar Wilde | Edimat Libros | 8484036383 |
| 6  | Before Night Falls | Reinaldo Arenas | Penguin Books | 0140157654 |
| 7  | From the Mixed Up Files of Mrs Basil E. Frankweiler | E. L. Konigsburg | Random House Childrens Pub (Mm) | 044022733X |
| 8  | Harry Bear's Railway Adventure | C.J. Whiting | Minerva Press | 186106800X |
| 9  | To Marry an Irish Rogue (Irish Eyes Romance Series, 2) | Lisa Hendrix | Jove Books | 0515127868 |
| 10 | Six Hours One Friday : Anchoring to the Power of the Cross | Max Lucado | Multnomah | 1576736016 |


#### 📊 Insight dari Rekomendasi **Neural Collaborative Filtering** 
- Rekomendasi mencakup berbagai genre seperti petualangan, sejarah, sastra klasik, dan spiritualitas. Model collaborative filtering memberikan rekomendasi yang beragam, menunjukkan kecenderungan pengguna terhadap berbagai topik dan gaya bacaan.
- Buku yang direkomendasikan berasal dari penulis dan penerbit yang berbeda, mulai dari penulis terkenal seperti Oscar Wilde hingga penulis yang kurang dikenal. Ini menunjukkan kemampuan model dalam mengenali beragam penulis dan memperkenalkan buku dari penulis yang lebih niche.
- Collaborative filtering mencocokkan pola perilaku pembaca lain yang serupa dengan User 20. Buku-buku dalam daftar ini kemungkinan besar dipilih berdasarkan kesamaan preferensi dengan pengguna lain, menciptakan rekomendasi yang relevan dan menarik.

---

## Evaluation
Dalam proyek ini menggunakan beberapa metrik evaluasi yang disesuaikan dengan pendekatan sistem rekomendasi yang diterapkan, yaitu Content-Based Filtering dan Collaborative Filtering.

### 1. Content-Based Filtering 
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

### Analisis Evaluasi

- Precision: 0.10    
**Precision** mengukur sejauh mana rekomendasi yang diberikan oleh model benar-benar relevan. Dalam hal ini, model menghasilkan rekomendasi buku yang relevan dengan **10% akurasi**. Artinya, hanya sekitar 10% dari total rekomendasi yang diberikan oleh model yang benar-benar sesuai dengan preferensi atau kebutuhan pengguna. Nilai precision yang rendah ini menunjukkan bahwa sebagian besar rekomendasi yang diberikan model tidak relevan atau tidak sesuai dengan harapan pengguna, sehingga model memerlukan peningkatan untuk memberikan rekomendasi yang lebih akurat.

- Recall: 0.50    
**Recall** mengukur sejauh mana model dapat menemukan seluruh item relevan yang tersedia di dalam dataset. Dengan nilai **50%**, model berhasil menemukan setengah dari item yang relevan yang bisa direkomendasikan kepada pengguna. Meskipun recall berada pada tingkat yang lebih tinggi dibandingkan precision, ini menunjukkan bahwa model mampu menangkap sebagian besar item yang relevan, tetapi masih banyak item relevan lainnya yang terlewatkan dalam rekomendasi.

-  Cosine Similarity Heatmap
![download](https://github.com/user-attachments/assets/274e6750-7492-447e-a879-329f56b9d33f)

      Berdasarkan Cosine Similarity Heatmap sebagian besar buku dari seri The Wheel of Time menunjukkan skor cosine similarity yang tinggi (sekitar 0.6–0.8). Hal ini menunjukkan bahwa sistem rekomendasi mampu mengenali keterkaitan konten, gaya, dan tema dalam seri yang sama. Ini membuktikan efektivitas pendekatan content-based filtering dalam menangkap struktur tematik dari karya yang saling berhubungan.


### Kesimpulan    
- Meskipun precision yang rendah menunjukkan adanya banyak rekomendasi yang tidak relevan, **recall yang lebih tinggi** menunjukkan bahwa model mampu menangkap sebagian besar item relevan. Oleh karena itu, model ini memiliki potensi untuk memberikan rekomendasi yang lebih baik dengan penyesuaian lebih lanjut.
- **Cosine similarity** yang tinggi di dalam seri **The Wheel of Time** membuktikan bahwa **content-based filtering** efektif dalam mengenali keterkaitan tematik dan gaya antar buku dalam satu seri. Ini menunjukkan bahwa pendekatan content-based filtering dapat sangat efektif untuk merekomendasikan buku dengan tema atau genre yang serupa.
- Peningkatan **precision** dan **recall**, serta penyesuaian lebih lanjut pada representasi konten buku, akan lebih meningkatkan kinerja sistem dalam memberikan rekomendasi yang lebih akurat dan relevan.


---

## 2. Neural Collaborative Filtering 

Untuk pendekatan **Neural Collaborative Filtering (NCF)**, model berfokus untuk memprediksi rating yang akan diberikan pengguna pada item tertentu. Oleh karena itu, evaluasi dilakukan menggunakan **RMSE** (Root Mean Squared Error) dan **MSE** (Mean Squared Error).

#### Rumus RMSE (Root Mean Squared Error)
$$
\text{RMSE} = \sqrt{\frac{1}{N} \sum_{i=1}^{N} (y_i - \hat{y}_i)^2}
$$

**Penjelasan**:  
RMSE mengukur seberapa besar rata-rata kesalahan kuadrat antara nilai aktual dan nilai prediksi. RMSE memberikan penalti lebih besar terhadap kesalahan prediksi yang besar (outlier), sehingga sangat sensitif terhadap prediksi yang jauh meleset.

---

#### Rumus MSE (Mean Squared Error)
$$
\text{MSE} = \frac{1}{N} \sum_{i=1}^{N} (y_i - \hat{y}_i)^2
$$

**Penjelasan**:  
MSE menghitung rata-rata dari kuadrat selisih antara nilai aktual dan nilai prediksi. MSE memberikan penalti yang lebih besar terhadap kesalahan yang lebih besar, dan lebih sensitif terhadap outlier dibandingkan dengan MAE. Dalam konteks **NCF**, MSE sering digunakan untuk mengukur seberapa baik model memprediksi rating pengguna.

---

#### Keterangan
- yᵢ = rating aktual ke-i
- ŷᵢ = rating prediksi ke-i
- N = jumlah observasi (jumlah pasangan data aktual dan prediksi)

### Analisis Evaluasi 

- Grafik Loss Curve yang dihasilkan selama pelatihan menunjukkan penurunan yang signifikan pada nilai loss dari epoch pertama hingga epoch ke-20. Di awal pelatihan, nilai loss cukup tinggi (sekitar 16.03), namun dengan bertambahnya epoch, loss menurun secara konsisten, mencapai nilai terendah pada epoch terakhir (sekitar 0.04).
![download (1)](https://github.com/user-attachments/assets/dda7777f-756e-4e12-9c43-d24bb750c9b7)    

  Penurunan loss yang stabil ini menunjukkan bahwa model berhasil belajar dan melakukan optimasi terhadap parameter yang ada selama proses pelatihan. Hal ini mengindikasikan bahwa model menyesuaikan bobotnya dengan baik untuk meminimalkan kesalahan prediksi pada data pelatihan. Tantangan berikutnya adalah memastikan bahwa model tidak hanya bekerja baik pada data pelatihan tetapi juga mampu melakukan generalisasi dengan baik pada data uji.

- Hasil Test RMSE yang diperoleh adalah 2.2320, yang mengukur perbedaan rata-rata antara rating yang diprediksi oleh model dan rating aktual yang diberikan oleh pengguna pada data uji. RMSE yang lebih rendah menunjukkan kinerja model yang baik dalam memprediksi rating dengan akurat. Sebagai acuan, semakin rendah nilai RMSE, semakin dekat prediksi model dengan nilai aktual, yang berarti model lebih akurat dalam memberikan prediksi rating. Dengan nilai RMSE sebesar 2.2320, model menunjukkan performa yang cukup baik, namun masih ada ruang untuk perbaikan lebih lanjut. Nilai RMSE ini menunjukkan bahwa model bisa lebih baik dalam menangkap variasi rating pengguna pada data yang lebih luas atau variatif.

### Kesimpulan 
- Model Neural Collaborative Filtering (NCF) menunjukkan kinerja yang solid dengan penurunan loss yang stabil selama pelatihan dan hasil RMSE yang terbilang baik (2.2320). Namun, masih ada ruang untuk peningkatan, terutama terkait dengan akurasi prediksi rating pada data uji.
- Dengan beberapa perbaikan, seperti penyempurnaan hyperparameter tuning, penambahan fitur, dan penerapan teknik regularisasi, model ini berpotensi memberikan rekomendasi yang lebih akurat bagi pengguna di masa mendatang.

--- 

### Hasil Akhir
Hasil evaluasi sistem rekomendasi menunjukkan bahwa pendekatan Content-Based Filtering (CBF) dan Neural Collaborative Filtering (NCF) telah berkontribusi dalam menjawab sebagian permasalahan yang dirumuskan pada tahap Business Understanding. Namun, masih terdapat ruang yang signifikan untuk perbaikan.

1. Problem Statement 1 – Masalah Pilihan Buku yang Berlebihan:    
Pendekatan Neural Collaborative Filtering (NCF) digunakan untuk memberikan rekomendasi yang dipersonalisasi berdasarkan pola interaksi pengguna.
Model berhasil menunjukkan penurunan loss yang stabil selama pelatihan dan menghasilkan RMSE = 2.2320 pada data uji, menandakan bahwa sistem sudah mampu mempelajari preferensi pengguna.
Namun, nilai RMSE tersebut masih mengindikasikan prediksi rating belum terlalu akurat, sehingga belum sepenuhnya mengurangi kebingungan pengguna dalam memilih buku secara optimal.


2. Problem Statement 2 – Kurangnya Rekomendasi yang Relevan:    
Pendekatan Content-Based Filtering (CBF) diterapkan dengan menggunakan Cosine Similarity antar konten buku.
Hasil evaluasi menunjukkan nilai:

- Precision@10 = 0.10
- Recall@10 = 0.50

Ini menandakan bahwa sistem berhasil menangkap separuh dari buku yang relevan, namun hanya 10% dari rekomendasi yang diberikan benar-benar sesuai dengan preferensi pengguna.
Meskipun demikian, heatmap cosine similarity memperlihatkan kemampuan sistem dalam mengenali keterkaitan tematik antar buku, terutama dalam seri seperti The Wheel of Time, yang menunjukkan skor similarity tinggi (0.6–0.8).

#### Pencapaian Goals Proyek
Beberapa tujuan proyek yang berhasil dicapai seperti penerapan dan integrasi dua pendekatan rekomendasi:

- Content-Based Filtering (CBF) menggunakan cosine similarity antar fitur buku
- Neural Collaborative Filtering (NCF) dengan optimisasi parameter model dan evaluasi berbasis RMSE

Evaluasi model dilakukan menggunakan metrik:
- Precision@K dan Recall@K (CBF)
- RMSE (NCF)
- Visualisasi tambahan seperti training loss curve dan cosine similarity heatmap mendukung interpretasi hasil dan pemahaman performa model.

#### Saran Pengembangan 
Secara umum, sistem rekomendasi yang dibangun sudah menjawab sebagian permasalahan utama dengan menggunakan pendekatan CBF dan NCF.
Namun, relevansi rekomendasi dan akurasi prediksi masih belum cukup kuat untuk memberikan dampak bisnis yang signifikan.
Rekomendasi Pengembangan Selanjutnya:
- Menambahkan metadata buku seperti genre, tahun terbit, sinopsis
- Menggabungkan pendekatan CBF dan NCF ke dalam sistem hybrid
- Melakukan tuning parameter lebih lanjut pada arsitektur model NCF
- Meningkatkan representasi fitur konten pada CBF agar lebih informatif

Dengan pengembangan ini, sistem diharapkan mampu memberikan rekomendasi yang lebih relevan, personal, dan berdampak terhadap pengalaman pengguna serta peningkatan penjualan.






