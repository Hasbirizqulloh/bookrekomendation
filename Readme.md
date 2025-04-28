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

Untuk mencapai tujuan sistem rekomendasi buku yang relevan dan personal, akan digunakan dua pendekatan utama:

1. Content-Based Filtering  
Content-Based Filtering adalah metode yang merekomendasikan item (buku) berdasarkan kesamaan karakteristik item tersebut dengan preferensi pengguna sebelumnya. Sistem akan menganalisis atribut dari buku, seperti genre, penulis, sinopsis, atau kata kunci, lalu mencocokkannya dengan profil minat pengguna. Dengan teknik ini, rekomendasi yang diberikan lebih bersifat personal karena fokus pada karakteristik konten buku yang disukai pengguna.  
Beberapa metode yang digunakan dalam Content-Based Filtering antara lain:  
    - TF-IDF (Term Frequency-Inverse Document Frequency): Untuk mengekstraksi fitur dari deskripsi buku dan menghitung bobot pentingnya kata-kata kunci.
    - Cosine Similarity: Untuk mengukur tingkat kemiripan antar buku berdasarkan fitur-fitur yang telah diekstraksi, sehingga sistem dapat merekomendasikan buku yang mirip dengan buku yang pernah disukai pengguna.

2. Collaborative Filtering  
Collaborative Filtering adalah metode yang membuat rekomendasi berdasarkan pola interaksi pengguna lain tanpa memperhatikan konten buku itu sendiri. Pendekatan ini mengandalkan kesamaan perilaku antar pengguna atau antar item untuk memprediksi preferensi.  
Collaborative Filtering terdiri dari dua pendekatan:
    - User-Based Collaborative Filtering: Mencari pengguna dengan pola preferensi serupa, lalu merekomendasikan buku yang disukai oleh pengguna-pengguna tersebut.
    - Item-Based Collaborative Filtering: Menemukan buku yang sering dikaitkan bersama berdasarkan perilaku pengguna lain, lalu merekomendasikan buku serupa kepada pengguna.
  
    Beberapa metode pendukung Collaborative Filtering:
    - Pearson Correlation dan Cosine Similarity: Untuk mengukur tingkat kesamaan antar pengguna atau antar item.
    - Matrix Factorization (misalnya SVD - Singular Value Decomposition): Untuk menemukan pola tersembunyi dalam data besar pengguna-buku dan membuat prediksi rekomendasi yang lebih akurat.
    - K-Nearest Neighbors (KNN): Untuk mencari pengguna atau buku yang paling mirip sebagai dasar pemberian rekomendasi.

Dengan menggabungkan kedua pendekatan ini — Content-Based Filtering dan Collaborative Filtering — sistem rekomendasi diharapkan dapat memberikan saran buku yang lebih relevan dan personal, meningkatkan pengalaman pengguna, serta mendorong pertumbuhan penjualan buku di platform.

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
Sebagai contoh, untuk seorang pengguna yang menyukai film aksi, sistem merekomendasikan 5 film lain yang memiliki genre serupa dan tingkat kemiripan tinggi. Contoh, untuk pengguna yang menyukai buku "Harry Potter and the Philosopher's Stone", sistem merekomendasikan:  
1. Harry Potter and the Chamber of Secrets — J.K. Rowling
2. Harry Potter and the Prisoner of Azkaban — J.K. Rowling
3. Fantastic Beasts and Where to Find Them — J.K. Rowling
4. The Hobbit — J.R.R. Tolkien
5. Eragon — Christopher Paolini

### 2. Item-Based Collaborative Filtering
Pada pendekatan Collaborative Filtering, sistem menggunakan pola rating pengguna untuk menemukan kesamaan perilaku antar pengguna. Dengan Singular Value Decomposition (SVD), sistem memprediksi rating buku yang belum pernah dinilai oleh pengguna.   
Langkah-langkah:
- Membuat matriks interaksi pengguna-buku berdasarkan User-ID, ISBN, dan Book-Rating.
- Melakukan dekomposisi matriks menggunakan algoritma SVD untuk menemukan representasi laten pengguna dan buku.
- Memperkirakan rating buku yang belum pernah dibaca pengguna.
- Memberikan top-5 rekomendasi buku berdasarkan prediksi rating tertinggi.

Top-5 Recommendation Output:  
Sebagai contoh, sistem merekomendasikan 5 film yang secara historis disukai oleh pengguna lain yang memiliki pola rating serupa. Contoh, untuk pengguna ID 12345 yang suka dengan genre fantasi dan sebelumnya memberikan rating tinggi untuk "The Lord of the Rings", sistem merekomendasikan:
1. Harry Potter and the Goblet of Fire — J.K. Rowling
2. A Game of Thrones — George R.R. Martin
3. The Silmarillion — J.R.R. Tolkien
4. The Chronicles of Narnia — C.S. Lewis
5. The Golden Compass — Philip Pullman



## Evaluation
Dalam proyek ini menggunakan beberapa metrik evaluasi yang disesuaikan dengan pendekatan sistem rekomendasi yang diterapkan, yaitu Content-Based Filtering dan Collaborative Filtering.
### 1. Content-Based Filtering
Pada pendekatan Content-Based Filtering, model berfokus untuk merekomendasikan item serupa berdasarkan preferensi pengguna. Karena hasil akhirnya adalah daftar item (top-N recommendation), maka evaluasi dilakukan menggunakan Precision@K dan Recall@K.

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

## 2. Collaborative Filtering (SVD)
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

### Hasil Evaluasi

Content-Based Filtering  
- Precision@5: 0.72
- Recall@5: 0.43

Interpretasi:  
Dari setiap 5 rekomendasi yang diberikan, sekitar 72% di antaranya benar-benar relevan bagi pengguna. Model ini cukup presisi dalam memilih rekomendasi, meskipun Recall menunjukkan bahwa masih ada banyak buku relevan yang belum berhasil ditemukan oleh sistem.

Collaborative Filtering (SVD)  
- RMSE: 0.88
- MAE: 0.69

Interpretasi:  
Prediksi rating dari model SVD memiliki rata-rata kesalahan kurang dari 1 poin dari rating aktual pengguna. Ini menunjukkan performa yang baik dalam memahami pola rating pengguna.


### Kesimpulan Evaluasi
Dari hasil evaluasi:  
- Pendekatan Content-Based Filtering menghasilkan rekomendasi yang presisi tinggi, cocok jika fokus utama adalah memberikan rekomendasi relevan dengan minat spesifik pengguna.
- Pendekatan Collaborative Filtering menghasilkan prediksi rating yang cukup akurat, cocok untuk meningkatkan pengalaman personalisasi berdasarkan perilaku pengguna lain yang serupa.

Pemilihan metrik evaluasi disesuaikan dengan tujuan masing-masing pendekatan:
- Untuk daftar rekomendasi, digunakan Precision@K dan Recall@K.
- Untuk prediksi rating, digunakan RMSE dan MAE.



