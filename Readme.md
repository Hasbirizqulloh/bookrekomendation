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

### 1. Pembersihan Data Rating
**Langkah yang Dilakukan:** 

Dihapus semua entri pada Ratings.csv yang memiliki nilai rating 0, karena dianggap sebagai umpan balik implisit atau tidak valid.

**Pertimbangan:**   
Langkah ini dilakukan untuk menjaga kualitas data input untuk Colaborative Filtering serta mengurangi beban memori komputasi.

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
- Setelah semua data dibersihkan, dataset Ratings.csv, Books.csv, dan Users.csv akan digabungkan. Data akan digabungkan berdasarkan kolom User-ID untuk menggabungkan data pengguna dengan rating yang diberikan dan ISBN untuk menggabungkan data rating dengan metadata buku.
- Cek kembali missing values pada data yang digabungkan karena diduga akan terjadi missing values dari metadata buku yang baru digabungkan.
- Gabungan ini akan menghasilkan sebuah dataset yang komprehensif, yang mencakup informasi pengguna, rating buku, serta metadata buku yang relevan.

**Pertimbangan:**  
Penggabungan ketiga dataset ini memungkinkan untuk membangun sistem rekomendasi yang lebih kaya dan lebih akurat dengan informasi lengkap tentang buku, pengguna, dan preferensi rating.

### 7. Sampling Data

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
Sebagai contoh, untuk seorang pengguna yang menyukai film aksi, sistem merekomendasikan 5 film lain yang memiliki genre serupa dan tingkat kemiripan tinggi. Contoh, untuk pengguna yang menyukai buku "**Fire and Hemlock**", sistem merekomendasikan:                                                                                                                                           
| Rank | Book Title             | Book Author         | Predicted Rating |
|:----:|:-----------------------|:--------------------|:----------------:|
| 1    | Power of three          | Diana Wynne Jones    | 5.9              |
| 2    | Dark Lord of Derkholm   | Diana Wynne Jones    | 4.7              |
| 3    | Hemlock Bay             | Catherine Coulter    | 3.1              |
| 4    | No Other Option         | Marcus Wynne         | 2.6              |
| 5    | Stuart Little           | E. B. White          | 2.0              |
| 6    | Stuart Little           | E. B. White          | 2.0              |
| 7    | Voyager                 | DIANA GABALDON       | 1.9              |
| 8    | Outlander               | DIANA GABALDON       | 1.9              |
| 9    | Outlander               | DIANA GABALDON       | 1.9              |
| 10   | Outlander               | DIANA GABALDON       | 1.9              |

### 2. Item-Based Collaborative Filtering
Pada pendekatan Collaborative Filtering, sistem menggunakan pola rating pengguna untuk menemukan kesamaan perilaku antar pengguna. Dengan Singular Value Decomposition (SVD), sistem memprediksi rating buku yang belum pernah dinilai oleh pengguna.   
Langkah-langkah:
- Membuat matriks interaksi pengguna-buku berdasarkan User-ID, ISBN, dan Book-Rating.
- Melakukan dekomposisi matriks menggunakan algoritma SVD untuk menemukan representasi laten pengguna dan buku.
- Memperkirakan rating buku yang belum pernah dibaca pengguna.
- Memberikan top-10 rekomendasi buku berdasarkan prediksi rating tertinggi.

Top-10 Recommendation Output:  
Sebagai contoh, sistem merekomendasikan 10 film yang secara historis disukai oleh pengguna lain yang memiliki pola rating serupa. Contoh, untuk pengguna ID 116320 yang suka dengan genre fantasi dan sebelumnya memberikan rating tinggi untuk "The Lord of the Rings", sistem merekomendasikan:


| Rank | Book Title                                        | Book Author         | Predicted Rating   |
|:----:|:--------------------------------------------------|:--------------------|:------------------:|
| 1    | The Alienist                                       | Caleb Carr           | 3.77e-17           |
| 2    | A College of Magics                                | Caroline Stevermer   | 3.10e-17           |
| 3    | The Lovely Bones: A Novel                          | Alice Sebold         | 1.12e-16           |
| 4    | The Many-Colored Land                              | Julian May           | 3.45e-17           |
| 5    | Stealing Heaven: The Love Story of Heloise and...  | Marion Meade         | 3.10e-17           |
| 6    | Blue Guide: Wales and the Marches                  | Tomeo                | 3.10e-17           |
| 7    | The Inner Sky: How to Make Wiser Choices for a...  | Steven Forrest       | 3.45e-17           |
| 8    | Asteroid Goddesses                                 | Demetra George       | 3.10e-17           |
| 9    | A Dictionary of Heraldry                           | Stephen Friar        | 3.45e-17           |
| 10   | The Npr Guide to Building a Classical Cd Collection| Ted Libbey           | 3.45e-17           |

---
### 3. User-Based Collaborative Filtering
Pada pendekatan User-Based Collaborative Filtering, sistem menggunakan pola rating pengguna untuk menemukan pengguna lain dengan perilaku yang mirip. Kemudian, sistem merekomendasik
Langkah-langkah:
- Membuat matriks interaksi pengguna-buku berdasarkan User-ID, ISBN, dan Book-Rating.
- Menghitung cosine similarity antar pengguna untuk mengukur tingkat kemiripan preferensi.
- Menentukan k tetangga terdekat (k-nearest neighbors) berdasarkan skor kemiripan tertinggi.
- Menghitung weighted average rating buku dari tetangga terdekat.

Top-10 Recommendation Output:    
Sebagai contoh, sistem merekomendasikan 10 buku yang secara historis disukai oleh pengguna lain dengan pola rating serupa. Contohnya, untuk User-ID 232959, sistem merekomendasikan:

| Rank | Book Title                                         | Book Author           | Predicted Rating |
|:----:|:---------------------------------------------------|:----------------------|:----------------:|
| 1    | Fiona Range                                        | Mary McGarry Morris    | 2.64             |
| 2    | The Buddha of Brewer Street                        | Michael Dobbs          | 1.68             |
| 3    | With Thanks and Appreciation: The Sweet Nellie... | Pat Ross               | 1.52             |
| 4    | Talk Before Sleep: A Novel                         | Elizabeth Berg         | 1.52             |
| 5    | Now All We Need Is a Title: Famous Book Titles...  | Andre Bernard          | 1.35             |
| 6    | Liar                                               | Stephen Fry            | 1.35             |
| 7    | Betrayal in Death                                  | Nora Roberts           | 1.35             |
| 8    | Mrs Dalloway                                       | Virginia Woolf         | 1.18             |
| 9    | Timoleon Vieta Come Home: A Sentimental Journey    | Dan Rhodes             | 0.00             |
| 10   | The Master of All Desires                          | Judith Merkle Riley     | 0.00             |


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

### Hasil Evaluasi

#### Content-Based Filtering 
Buku yang Disukai oleh User:
- Monkeys on the Interstate: And Other Tales from America's Favorite Zookeeper
- The Lost Boy: A Foster Child's Search for the Love of a Family
- The Four Agreements: A Practical Guide to Personal Freedom
- Color Purple
- Marilyn Monroe: Photographs 1945-1962 (Schirmer's Visual Library)
- Jurassic Park
- Macroscope
- How Stella Got Her Groove Back
- Letters from the Earth
- My Story

Hasil Rekomendasi Model:
- Power of three
- Dark Lord of Derkholm
- Hemlock Bay
- No Other Option
- Stuart Little
- Stuart Little
- Voyager
- Outlander
- Outlander
- Outlander

Evaluation Metrics:
- Precision@5: 0.00
- Recall@5: 0.00

Interpretasi:    
Model Content-Based Filtering belum berhasil memberikan rekomendasi yang sesuai dengan buku-buku yang disukai pengguna. Tidak ada satu pun rekomendasi yang cocok. Ini menunjukkan perlunya perbaikan pada teknik ekstraksi fitur atau metode similarity.

#### Item-Based Collaborative Filtering (SVD)  
- RMSE: 7.5156
- MAE: 7.0376

Interpretasi:  
Model Item-Based Collaborative Filtering berbasis SVD menunjukkan kesalahan prediksi yang cukup tinggi.
RMSE dan MAE di atas 7 berarti rata-rata prediksi rating berbeda jauh dari rating aktual. Ini bisa disebabkan oleh sparsity data (rating yang sedikit) atau kurang optimalnya jumlah latent factors.

#### User-Based Collaborative Filtering (UserCF)
Buku yang Disukai oleh User:
- Confessions of a Shopaholic

Hasil Rekomendasi Model:
- A Trip to the Light Fantastic: Travels With a Mexican Circus
- House of Cards
- The Buddha of Brewer Street
- Queen of Shaba: The Story of an African Leopard
- Triple Factor
- Liar
- Airport International: Level 4 - Intermediate (Nelson Readers)
- Steel Bonnets: The Story of the Anglo-Scottish Border Reivers
- Girlfriend in a Coma
- Firewing

Evaluation Metrics:
- Precision@10: 0.0000
- Recall@10: 0.0000

Interpretasi:    
Sama seperti Content-Based Filtering, model User-Based Collaborative Filtering saat ini juga belum mampu merekomendasikan buku yang relevan. Meskipun pola kesamaan antar pengguna sudah dihitung, namun belum mampu menangkap preferensi pengguna dengan akurat.

#### Evaluation Results

| Model                          | Precision@10 | Recall@10 | RMSE   | MAE    |
|---------------------------------|--------------|-----------|--------|--------|
| Content-Based Filtering (CBF)   | 0.0000       | 0.0000    | -      | -      |
| Item-Based Collaborative Filtering | -          | -         | 7.5156 | 7.0376 |
| User-Based Collaborative Filtering | 0.0000     | 0.0000    | -      | -      |

Berdasarkan hasil evaluasi terhadap beberapa pendekatan sistem rekomendasi:

- Content-Based Filtering    
Menghasilkan Precision@10 dan Recall@10 sebesar 0.0000. Ini menunjukkan bahwa sistem belum mampu merekomendasikan buku yang benar-benar relevan berdasarkan kemiripan konten buku. Dengan demikian, pendekatan ini belum efektif untuk kebutuhan rekomendasi dalam platform.

- Item-Based Collaborative Filtering (menggunakan SVD)    
Model ini menunjukkan hasil evaluasi RMSE sebesar 7.5156 dan MAE sebesar 7.0376. Meskipun prediksi rating dapat dilakukan, error yang relatif besar ini menunjukkan bahwa model belum cukup akurat dalam memahami preferensi pengguna.

- User-Based Collaborative Filtering    
Pendekatan ini menghasilkan Precision@10 dan Recall@10 sebesar 0.0000, yang menunjukkan bahwa sistem belum berhasil memberikan rekomendasi berbasis pola kesamaan antar pengguna.

Dari ketiga pendekatan yang dievaluasi, Item-Based Collaborative Filtering (SVD) menjadi model yang paling layak untuk dipilih dalam tahap awal, karena:
- Satu-satunya pendekatan yang mampu menghasilkan prediksi rating numerik.
- Meskipun error masih cukup besar, pendekatan ini lebih dekat untuk membangun fondasi sistem rekomendasi berbasis perilaku pengguna.

Dengan perbaikan pada sisi data (seperti filtering data sparse, pengayaan metadata buku, atau hybrid dengan content-based), model ini berpotensi memberikan hasil yang jauh lebih baik.

📌 Model yang Dipilih:  
Item-Based Collaborative Filtering menggunakan SVD dipilih sebagai dasar pengembangan sistem rekomendasi, karena memiliki performa prediksi terbaik dibandingkan pendekatan lain yang diuji.

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





