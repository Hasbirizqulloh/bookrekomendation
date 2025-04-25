# Laporan Proyek Machine Learning - Moh Hasbi Rizqulloh

## Project Overview

Sistem rekomendasi adalah teknologi yang saat ini banyak digunakan untuk membantu pengguna dalam memilih produk atau konten berdasarkan preferensi atau perilaku mereka sebelumnya. Dalam dunia digital yang penuh dengan pilihan, sistem rekomendasi memainkan peran penting dalam memberikan pengalaman yang lebih personal dan efisien bagi penggunanya. Rekomendasi yang baik tidak hanya membantu pengguna dalam membuat keputusan lebih cepat, tetapi juga dapat meningkatkan kepuasan mereka dengan menyediakan informasi yang lebih relevan dengan kebutuhan atau minat mereka.

Dalam berbagai aplikasi, mulai dari platform belanja online, media sosial, hingga layanan streaming, sistem rekomendasi telah diterapkan dengan tujuan untuk mempermudah pengguna dalam menemukan produk atau konten yang sesuai dengan keinginan mereka. Sebagai contoh, platform seperti Amazon, Netflix, dan Spotify menggunakan sistem rekomendasi untuk memberikan saran produk, film, atau musik yang relevan. Namun, tantangan utama dalam sistem rekomendasi adalah bagaimana memastikan bahwa rekomendasi yang diberikan benar-benar sesuai dengan preferensi pengguna.

Salah satu metode yang banyak digunakan dalam membangun sistem rekomendasi adalah Content-Based Filtering. Metode ini bekerja dengan menganalisis konten atau fitur dari item yang telah berinteraksi dengan pengguna (misalnya buku, film, produk) dan mencocokkannya dengan item lain yang memiliki kesamaan. Dalam konteks proyek ini, sistem rekomendasi akan dibangun untuk buku dengan menggunakan pendekatan Content-Based Filtering, di mana sistem akan merekomendasikan buku yang serupa dengan buku yang telah dibaca oleh pengguna, berdasarkan fitur seperti judul, pengarang, dan penerbit.

### Mengapa Proyek Ini Penting?
Dalam dunia digital yang penuh dengan pilihan, pengguna sering merasa kewalahan mencari buku yang sesuai dengan minat mereka. Sistem rekomendasi berbasis konten membantu menyaring pilihan buku yang relevan, menghemat waktu, dan meningkatkan pengalaman pengguna. Dengan memberikan saran yang lebih personal, pengguna merasa lebih dihargai, yang memperkuat hubungan mereka dengan platform penyedia buku. Selain itu, sistem ini dapat meningkatkan interaksi pengguna dengan platform, serta mendorong mereka untuk membeli buku yang mungkin sebelumnya tidak mereka pertimbangkan, sehingga berpotensi meningkatkan penjualan dan pemanfaatan koleksi buku.

### Solusi yang Akan Dikembangkan
Proyek ini bertujuan untuk membangun sistem rekomendasi buku dengan menggunakan Content-Based Filtering. Sistem ini akan menggunakan data mengenai buku, seperti judul, pengarang, penerbit, dan rating yang diberikan oleh pengguna untuk menghitung kesamaan antar buku. Dengan demikian, pengguna yang sudah membaca buku tertentu dapat menerima rekomendasi buku serupa yang mungkin mereka sukai.
  
### Referensi: 
- [Enhancing Personalized Book Recommender System](https://www.ijana.in/papers/V14I3-11.pdf)
- [Book Recomender System](https://www.irjmets.com/adminroot/uploaddir/research_conference_paper/document/36/36_2023121224120151.pdf)
- [Content-Based Recommender Systems Taxonomy](https://sciendo.com/article/10.2478/fcds-2023-0009)
- [An Aggranized Framewok For Enriching Book Recommendation System](https://ejournal.um.edu.my/index.php/MJCS/article/view/29478)
- [Design and Implementation of Book Recommendation Management System Based on Improved Apriori Algorithm](https://www.scirp.org/journal/paperinformation?paperid=99347)


## Business Understanding

Bagian Business Understanding dalam proyek ini bertujuan untuk mengidentifikasi dan menjelaskan permasalahan yang ada dalam platform penyedia buku, serta menguraikan solusi yang akan dikembangkan melalui penerapan sistem rekomendasi berbasis Content-Based Filtering. Dalam konteks ini, akan menganalisis bagaimana sistem rekomendasi dapat membantu pengguna menemukan buku yang lebih relevan dan sesuai dengan minat mereka, sekaligus meningkatkan pengalaman pengguna serta penjualan buku di platform. Proyek ini berfokus pada memberikan solusi untuk masalah-masalah yang ada, termasuk kesulitan pengguna dalam mencari buku yang relevan dan kurangnya rekomendasi yang personal.

### Problem Statements

Pada tahap ini, kita akan memulai dengan menganalisis masalah-masalah utama yang sering dihadapi oleh pengguna platform penyedia buku:
1. Masalah Pilihan Buku yang Berlebihan  
Dengan jumlah buku yang sangat banyak yang tersedia di berbagai platform digital, pengguna sering kali merasa bingung dan kewalahan dalam memilih buku yang sesuai dengan minat mereka. Platform yang menyediakan koleksi buku dalam jumlah besar tanpa adanya sistem rekomendasi yang efektif seringkali membuat pengguna kehilangan arah dalam pencarian mereka.

2. Kurangnya Rekomendasi yang Relevan  
Banyak platform buku yang tidak mampu memberikan rekomendasi yang sesuai dengan preferensi pengguna. Hal ini menyebabkan pengguna harus menghabiskan waktu yang lebih lama untuk mencari buku yang mereka minati, atau bahkan mereka tidak menemukan buku yang relevan sama sekali. Rekomendasi yang tidak personal atau tidak akurat dapat menurunkan kualitas pengalaman pengguna secara keseluruhan.

3. Tidak Ada Sistem yang Dapat Meningkatkan Penjualan Buku  
Tanpa adanya sistem rekomendasi yang tepat, pengguna cenderung membeli buku yang sudah mereka kenal, sementara buku-buku baru atau buku lain yang relevan dengan minat mereka mungkin tidak mendapatkan perhatian. Ini mengarah pada penurunan penjualan buku yang dapat dengan mudah ditingkatkan dengan sistem rekomendasi berbasis konten.

### Goals
Dalam rangka mengatasi permasalahan tersebut, tujuan dari proyek ini adalah:
1. Menyediakan Rekomendasi Buku yang Personalisasi dan Relevan  
Sistem rekomendasi berbasis Content-Based Filtering yang akan dibangun bertujuan untuk menganalisis fitur-fitur buku seperti judul, pengarang, dan penerbit. Sistem ini akan memberikan rekomendasi buku yang relevan berdasarkan kesamaan fitur dengan buku yang sebelumnya dibaca atau disukai oleh pengguna.

2. Meningkatkan Pengalaman Pengguna dengan Rekomendasi yang Akurat  
Salah satu tujuan utama dari proyek ini adalah untuk meningkatkan pengalaman pengguna dengan memberikan rekomendasi yang lebih akurat dan personal. Dengan sistem rekomendasi yang relevan, pengguna tidak hanya akan lebih mudah menemukan buku yang mereka suka, tetapi juga merasa lebih dihargai karena platform memahami preferensi mereka.

3. Meningkatkan Penjualan Buku  
Melalui penerapan sistem rekomendasi berbasis konten, platform penyedia buku diharapkan dapat meningkatkan penjualan buku. Dengan memberikan rekomendasi yang relevan dan menarik bagi pengguna, buku yang mungkin sebelumnya tidak dipertimbangkan akan lebih sering dibeli. Hal ini berpotensi meningkatkan pendapatan dan efisiensi dalam penggunaan katalog buku.

### Solution Approach
Untuk mencapai tujuan tersebut, beberapa pendekatan yang akan digunakan dalam mengembangkan sistem rekomendasi berbasis konten antara lain:

1. Content-Based Filtering  
Content-Based Filtering adalah pendekatan yang digunakan untuk menganalisis dan membandingkan kesamaan antar buku berdasarkan fitur kontennya. Dalam hal ini, fitur buku seperti judul, pengarang, dan penerbit akan digunakan untuk menghitung tingkat kesamaan antar buku yang sudah dibaca dan buku yang belum dibaca pengguna. Buku yang memiliki kesamaan tinggi dengan buku yang disukai pengguna akan lebih cenderung direkomendasikan.

2. Cosine Similarity  
Salah satu metode yang dapat digunakan untuk mengukur kesamaan antar buku adalah Cosine Similarity. Teknik ini mengukur derajat kesamaan antara dua buku dengan membandingkan vektor fitur mereka. Semakin kecil sudut antara dua vektor, semakin mirip buku tersebut. Metode ini efektif untuk memberikan rekomendasi yang akurat berdasarkan kemiripan fitur buku.

3. TF-IDF (Term Frequency-Inverse Document Frequency)  
TF-IDF adalah teknik yang digunakan untuk menghitung pentingnya kata dalam deskripsi buku, judul, atau kategori. Dengan menggunakan TF-IDF, sistem dapat memberi bobot lebih pada kata-kata yang lebih relevan, sehingga meningkatkan akurasi dalam memberikan rekomendasi buku yang sesuai dengan preferensi pengguna.

4. K-Nearest Neighbors (KNN)  
K-Nearest Neighbors (KNN) adalah algoritma yang digunakan untuk mencari buku-buku yang paling mirip berdasarkan kesamaan fitur mereka. Dengan menggunakan KNN, sistem dapat menghitung jarak antar vektor buku dan mencari N buku terdekat dengan buku yang sudah dibaca atau disukai oleh pengguna. Teknik ini akan memberikan rekomendasi buku dengan memilih buku-buku yang memiliki jarak paling dekat dengan buku yang diinginkan pengguna, berdasarkan fitur teks yang telah dihitung sebelumnya.


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
1. Ratings.csv menunjukkan dominasi rating bernilai 0 (lebih dari 50%), yang mengindikasikan adanya banyak data yang tidak valid atau berupa implicit feedback. Meskipun begitu, data ini tetap akan digunakan setelah dilakukan seleksi data dan pembersihan untuk menjaga kualitas input sistem rekomendasi. Hanya data dengan rating eksplisit (1–10) yang akan dipertimbangkan untuk digunakan dalam model rekomendasi, sementara data dengan rating 0 akan dihapus atau diperlakukan sebagai data yang tidak relevan.

2. Users.csv mengandung lebih dari 39% data usia yang hilang dan juga banyak nilai outlier ekstrem. Untuk itu, data pengguna akan dibersihkan terlebih dahulu, dan nilai usia yang hilang akan ditangani menggunakan teknik imputasi atau dengan menghapus entri yang tidak lengkap. Selain itu, informasi lokasi yang tersedia dalam dataset juga akan dipertimbangkan untuk mengidentifikasi pola preferensi berdasarkan wilayah, meskipun fokus utama tetap pada data rating dan buku.
  
3. Books.csv berisi metadata penting seperti judul, penulis, penerbit, dan tahun terbit buku. Namun, karena volume data yang sangat besar, tidak semua informasi dalam dataset ini akan digunakan. Proses seleksi fitur dan reduksi dimensi akan dilakukan pada tahap Data Preparation untuk memilih informasi yang paling relevan, seperti judul, pengarang, dan penerbit, yang akan digunakan dalam analisis Content-Based Filtering.

4. Mengingat keterbatasan memori, hanya sekitar 20.000 entri dari masing-masing dataset (Books.csv, Ratings.csv, Users.csv) yang akan dipertimbangkan untuk meminimalkan penggunaan sumber daya dan memastikan bahwa proses modeling tetap efisien. Gabungan antara data dari ketiga file ini akan dilakukan dengan mencocokkan User-ID dari Ratings.csv dengan User-ID di Users.csv, serta mencocokkan ISBN dari Ratings.csv dengan ISBN di Books.csv.

Berdasarkan evaluasi tersebut, sistem rekomendasi akan dibangun dengan menggabungkan informasi dari Books.csv, Users.csv, dan Ratings.csv, menggunakan pendekatan Content-Based Filtering. Fokus utama akan diberikan pada pemrosesan dan ekstraksi fitur dari metadata buku untuk menghasilkan rekomendasi yang relevan dan informatif.

## Data Preparation
Pada tahap ini, dilakukan serangkaian proses untuk mempersiapkan data agar siap digunakan dalam proses pemodelan sistem rekomendasi berbasis konten. Fokus utama berada pada data Books.csv, karena telah terbukti lebih bersih dan relevan untuk pendekatan yang digunakan.


### 1. Pembersihan dan Seleksi Data Rating
**Langkah yang Dilakukan:** 
- Dihapus semua entri pada Ratings.csv yang memiliki nilai rating 0, karena dianggap sebagai umpan balik implisit atau tidak valid.
- Setelah pembersihan, dilakukan pengambilan sampel secara acak sebanyak 20.000 entri rating untuk digunakan sebagai data utama.

**Pertimbangan:**   
Langkah ini dilakukan untuk menjaga kualitas data input serta mengurangi beban memori komputasi.

### 2. Seleksi Data Buku Berdasarkan Data Rating
**Langkah yang Dilakukan:**
- Dari 20.000 data rating yang telah dipilih, diambil seluruh ISBN unik yang muncul.
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

### 4. Pembersihan Data Pengguna (Users.csv)

**Langkah yang Dilakukan:**
- Outlier pada kolom usia yang ekstrem (misalnya, usia 0 atau 244) akan dihapus atau diganti dengan nilai yang wajar melalui teknik imputasi.
- Data yang hilang pada kolom Age akan ditangani dengan teknik imputasi yang sesuai (misalnya, menggunakan nilai rata-rata atau median).
- Data Location yang kosong atau tidak relevan juga akan dipertimbangkan untuk dibersihkan atau diisi dengan nilai default (misalnya, "Unknown").

**Pertimbangan:**  
Pembersihan ini dilakukan untuk memastikan bahwa data pengguna yang digunakan dalam model bersih, konsisten, dan tidak mengandung nilai ekstrem yang dapat mengganggu hasil rekomendasi.


### 5. Seleksi dan Reduksi Fitur
**Langkah yang Dilakukan:**  

Kolom yang tidak memberikan kontribusi terhadap representasi konten buku seperti `Image-URL-S`, `Image-URL-M`, dan `Image-URL-L` dihapus dari dataset.  

Hanya atribut utama yang dipertahankan, yaitu:  
- `Book-Title`  
- `Book-Author`  
- `Publisher`  
- `Year-Of-Publication`

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
- Setelah data final disiapkan, dilakukan sampling untuk memilih subset data yang lebih kecil untuk pelatihan model. Karena keterbatasan memori, sekitar 20.000 entri akan dipilih dari gabungan ketiga dataset tersebut.
- Pembagian data untuk pelatihan dan pengujian dilakukan menggunakan teknik train-test split, dengan sebagian data digunakan untuk melatih model dan sebagian lainnya digunakan untuk menguji akurasi rekomendasi yang dihasilkan.

**Pertimbangan:**  
Sampling data dan pembagian antara data pelatihan dan pengujian memastikan bahwa model dapat diuji secara objektif sebelum digunakan untuk menghasilkan rekomendasi yang lebih luas.

## Modeling
Tahapan ini membahas mengenai model sisten rekomendasi yang Anda buat untuk menyelesaikan permasalahan. Sajikan top-N recommendation sebagai output.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menyajikan dua solusi rekomendasi dengan algoritma yang berbeda.
- Menjelaskan kelebihan dan kekurangan dari solusi/pendekatan yang dipilih.

## Evaluation
Pada bagian ini Anda perlu menyebutkan metrik evaluasi yang digunakan. Kemudian, jelaskan hasil proyek berdasarkan metrik evaluasi tersebut.

Ingatlah, metrik evaluasi yang digunakan harus sesuai dengan konteks data, problem statement, dan solusi yang diinginkan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan formula metrik dan bagaimana metrik tersebut bekerja.

**---Ini adalah bagian akhir laporan---**

_Catatan:_
- _Anda dapat menambahkan gambar, kode, atau tabel ke dalam laporan jika diperlukan. Temukan caranya pada contoh dokumen markdown di situs editor [Dillinger](https://dillinger.io/), [Github Guides: Mastering markdown](https://guides.github.com/features/mastering-markdown/), atau sumber lain di internet. Semangat!_
- Jika terdapat penjelasan yang harus menyertakan code snippet, tuliskan dengan sewajarnya. Tidak perlu menuliskan keseluruhan kode project, cukup bagian yang ingin dijelaskan saja.
