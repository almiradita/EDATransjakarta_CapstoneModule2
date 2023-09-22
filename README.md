# **READ ME**
Halo semuanya! 🎉

Selamat datang di proyek saya! Ini adalah bagian dari perjalanan saya di bootcamp Data Science di Purwadhika. Di sini saya mencoba menerapkan ilmu yang sudah saya pelajari untuk menyelesaikan Capstone Module 2 Project mengenai Exploratory Data Analysis (EDA). Lebih dari itu, proyek ini juga adalah cerminan dari perjalanan saya menjadi seorang Data Scientist yang handal. 🚀

# **Outline**

Project ini terdiri dari:
1. [Jupyter Notebook](https://github.com/almiradita/EDATransjakarta_CapstoneModule2/blob/8e52b8d8329490a3a41bc901d544d12772af10a5/EDATransjakarta_CM2.ipynb) untuk *Exploratory Data Analysis* yang terperinci 
2. [Tableau Story & Dashboard](https://public.tableau.com/views/Transjakarta_CapstoneModule2/HasilAnalisis?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link) untuk visualisasi data

# **Overview**

PT Transportasi Jakarta (TransJakarta) adalah pusat perhatian kita -sebuah perusahaan Badan Usaha Milik Daerah (BUMD) yang bergerak di bidang layanan transportasi umum, khususnya bus 🚌. Ada tiga layanan utama:

#### 3 Layanan TransJakarta
| Jenis Transportasi                 | Deskripsi                                                   | Harga   |
|-----------------------------------|-------------------------------------------------------------|---------|
| 1. Transjakarta                   | Menawarkan perjalanan dalam kota                           | Rp3.500       |
| 2. Royal Trans                    | Menawarkan perjalanan lintas kota                           | Rp20.000   |
| 3. Mikrotrans JakLingko | Menawarkan perjalanan dalam kota dengan kapasitas bangku lebih sedikit dan bisa berhenti dimana saja tanpa harus berhenti di halte pemberhentian | Rp0 |

## **Pernyataan Masalah**
Direktur Pelayanan & Bisnis PT Transportasi Jakarta punya misi! Yaitu untuk **mengevaluasi dan meningkatkan efektivitas operasional serta infrastruktur Transjakarta**. . Oleh karena itu, Direktur merekrut *data analyst* untuk membantu dalam mengoptimalkan perjalanan TransJakarta.

### **Problem**
**Langkah apa yang bisa diambil oleh Direktur Pelayanan & Bisnis PT Transportasi Jakarta untuk mengoptimalkan operasional Transjakarta??**

### **Hasil yang di Harapkan**
Dalam menjawab pertanyaan di atas, kita akan melakukan **Exploratory Data Analysis** (EDA) dan memperoleh informasi seperti berikut:
1. **Analisis Rute Perjalanan** :
    1. Rute/Corridor yang paling sering digunakan
    2. Halte yang paling ramai
2. **Analisis Waktu Perjalanan** :
    1. Peak Hour 
    2. Waktu tap in dan tap out terbanyak
    3. Waktu rute dan halte terpadat terjadi di jam berapa 
    4. Waktu yang dibutuhkan dalam melakukan 1x perjalanan
3. **Analisis Penumpang Transjakarta** 
    1. Distribusi jenis kelamin penumpang
    2. Volume penumpang di setiap halte
    3. Distribusi usia penumpang
      
Dengan informasi ini, Direktur berharap dapat mengoptimalkan operasional dan infrastruktur Transjakarta.

# **Memahami Data 🧐**

Dalam menjawab masalah yang sudah ditentukan di atas, *analyst* menggunakan dataset [Transaksi Transjakarta](https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction) pada bulan April 2023. Dataset ini mencakup detail transaksi, informasi penumpang, dan rute perjalanan.

## **Deskripsi Dataset 📄**

| Column Name       | Description                                                                           |
|-------------------|--------------------------------------------------------------                         |
| transID           | Unique transaction id for every transaction                                           |
| payCardID         | Customers main identifier. The card customers use as a ticket for entrance and exit.  |
| payCardBank       | Customers card bank issuer name                                                       |
| payCardName       | Customers name that is embedded in the card.                                          |
| payCardSex        | Customers sex that is embedded in the card                                            |
| payCardBirthDate  | Customers birth year                                                                  |
| corridorID        | Corridor ID / Route ID as key for route grouping.                                     |
| corridorName      | Corridor Name / Route Name contains Start and Finish for each route.                  |
| direction         | 0 for Go, 1 for Back. Direction of the route.                                         |
| tapInStops        | Tap In (entrance) Stops ID for identifying stops name                                 |
| tapInStopsName    | Tap In (entrance) Stops Name where customers tap in.                                  |
| tapInStopsLat     | Latitude of Tap In Stops                                                              |
| tapInStopsLon     | Longitude of Tap In Stops                                                             |
| stopStartSeq      | Sequence of the stops, 1st stop, 2nd stops etc. Related to direction.                 |
| tapInTime         | Time of tap in. Date and time                                                         |
| tapOutStops       | Tap Out (Exit) Stops ID for identifying stops name                                    |
| tapOutStopsName   | Tap out (exit) Stops Name where customers tap out.                                    |
| tapOutStopsLat    | Latitude of Tap Out Stops                                                             |
| tapOutStopsLon    | Longitude of Tap Out Stops                                                            |
| stopEndSeq        | Sequence of the stops, 1st stop, 2nd stops etc. Related to direction.                 |
| tapOutTime        | Time of tap out. Date and time                                                        |
| payAmount         | The number of what customers pay. Some are free. Some not                             |

# **Perjalanan EDA 🕵️**
Project ini bertujuan untuk mendapatkan informasi berharga mengenai penggunaan Transjakarta agar bisa mengoptimalkan operasional Transjakarta. Analisis akan meliputi:
1. Data Preparation
2. Data Cleaning & Data Wrangling 
3. Data Analysis
4. Kesimpulan & Temuan Utama
5. Rekomendasi

Fokus akan diberikan pada tiga sub-topik yaitu, **Informasi Perjalanan, Informasi Waktu Perjalanan, dan Informasi Penumpang Transjakarta**, dengan tujuan untuk mengevaluasi dan meningkatkan efektivitas operasional serta infrastruktur Transjakarta.

Monggo! Jika ada pertanyaan atau ingin membahas lebih lanjut mengenai project ini, jangan ragu untuk menghubungi saya via [LinkedIn](https://www.linkedin.com/in/almira-d-48107b141/)! 💌
