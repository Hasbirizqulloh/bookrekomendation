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

Dengan pendekatan-pendekatan ini, diharapkan sistem rekomendasi yang dibangun akan efektif dalam memberikan saran buku yang relevan, meningkatkan pengalaman pengguna, serta membantu meningkatkan penjualan buku di platform.

## Data Understanding
Paragraf awal bagian ini menjelaskan informasi mengenai jumlah data, kondisi data, dan informasi mengenai data yang digunakan. Sertakan juga sumber atau tautan untuk mengunduh dataset. Contoh: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data).

Selanjutnya, uraikanlah seluruh variabel atau fitur pada data. Sebagai contoh:  

Variabel-variabel pada Restaurant UCI dataset adalah sebagai berikut:
- accepts : merupakan jenis pembayaran yang diterima pada restoran tertentu.
- cuisine : merupakan jenis masakan yang disajikan pada restoran.
- dst

**Rubrik/Kriteria Tambahan (Opsional)**:
- Melakukan beberapa tahapan yang diperlukan untuk memahami data, contohnya teknik visualisasi data beserta insight atau exploratory data analysis.

## Data Preparation
Pada bagian ini Anda menerapkan dan menyebutkan teknik data preparation yang dilakukan. Teknik yang digunakan pada notebook dan laporan harus berurutan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan proses data preparation yang dilakukan
- Menjelaskan alasan mengapa diperlukan tahapan data preparation tersebut.

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
