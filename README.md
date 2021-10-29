# TELCO COSTUMER CHURN PREDICTION

 Profile : Kresna Dwipayana Sindudharma H | [Email](mailto:kresnadwipsh@gmail.com) | [LinkedIn](https://www.linkedin.com/in/kresnadwipsh)
 
 Dataset : WA_Fn-UseC_-Telco-Customer-Churn.csv
 
 Source :  [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn)
 
 ---
 
 # Background

Dalam bisnis, mendapatkan pelanggan merupakan tujuan utama perusahaan. Namun ada kala pelanggan memilih beralih dengan berbagai alasan, yang nanti akan berdampak pada perusahaan.
 Peralihan itu disebut _Customer Churn_. Sehingga perlu diperhatikan _Churn Rate_ supaya memastikan retensi pelanggan pada suatu perusahaan tetap baik.
 
 Dalam proyek ini, saya memposisikan diri sebagai bagian dari tim Data Scientist pada sebuah perusahaan _Telco_.
 saya ingin meneliti perilaku pelanggan dan memastikan pelanggan mana yang bertahan dan tidak. Saya ingin membantu tim Pemasaran dengan membuat pemetaan pelanggan, supaya tim Pemasaran dapat melakukan kegiatan pemasaran tepat sasaran. 
 
 ---
 
 # I. Problem Statement
 
 ## 1. Problem Definition
 
 Dalam kasus ini, saya menemukan bahwa beberapa pelanggan memilih beralih atau menghentikan interaksi mereka terhadap perusahaan, namun tidak diketahui alasan pelanggan tersebut memilih beralih. Perusahaan tidak mengetahui dampak keuangan dari beralihnya pelanggan.
 
 Selain itu tim marketing kesulitan untuk menentukan pelanggan yang mana diperkirakan akan beralih untuk nanti diberikan sejumlah benefit atau diskon, sehingga menghindari dari pelanggan memilih beralih.
 
 <img src="https://www.jojonomic.com/wp-content/uploads/2020/11/34.-Churn1.jpg" width="500" />
 
 Untuk mengatasi masalah tersebut, perusahaan memerlukan :
 - Pemetaan mengenai produk unggulan dan non-unggulannya untuk kedepannya dapat dioptimalisasikan pelayanannya 
 - Pemetaan pelanggan mana yang di prediksi beralih atau tidak beralih supaya tim marketing dapat menyesuaikan kegiatan pemasarannya dengan karakteristik pelanggan. 
 - Dampak dari _customer churn_ terhadap keuangan perusahaan

Hasil yang diharapkan dari proyek ini adalah dapat menghasilkan sistem yang dapat mengklasifikasikan pelanggan yang berpotensi melakukan _churn_ dan pelanggan yang bertahan secara akurat dengan menggunakan pendekatan Machine Learning, sehingga dapat memberikan informasi pada stakeholder dan dapat dimanfaatkan untuk mencapai tujuan bisnis. 

## 2. Business Objective 

Adapun terdapat beberapa tujuan bisnis yang ingin dicapai melalui proyek ini, yakni sebagai berikut :
- Memaksimalkan keuntungan dengan memastikan pelanggan untuk tidak memutuskan interaksi bisnis atau memilih beralih dari perusahaan
- Memastikan pelanggan yang mendapat sejumlah benefit atau diskon tepat sasaran dan menjadi pelanggan yang loyal atau bertahan
- Meminimalisir kerugian dengan mengoptimalkan layanan unggulan

## 3. Data Requirements
 
Dalam proyek ini, berdasarkan _problem definition_ yang telah didefinisikan , maka dibutuhkan data sebagai fitur meliputi daftar pelanggan, perilaku pelanggan, karakteristik pelanggan,  total tagihan, DLL.
 
## 4. Analytic Approach

### Machine Learning Technique :
Pada proyek ini, karena saya ingin memprediksi pelanggan mana yang akan memilih beralih atau bertahan , dan telah memiliki label yakni _Churn_ dan _Not churn_, sehingga hal ini dapat diatasi dengan metode _supervised learning_ yang fokus pada klasifikasi. Saya akan memberikan data pada model dengan algortima klasifikasi untuk dipelajari atau di _training_, yang hasilnya kami harap dapat membuat prediksi yang baik dan akurat untuk memprediksi pelanggan mana yang akan memilih beralih atau bertahan. 

### Risk :
Terdapat beberapa resiko yang dapat disebabkan kesalahan prediksi dari model, yakni :
- Kesalahan proporsi prediksi pelanggan yang ditandai sebagai _Churn_ lebih besar dari yang ditandai _Not Churn_, sehingga kemungkinan perusahaan dapat berlebihan mengeluarkan anggaran promosi dan merugikan keuangan perusahaan karena memberikan benefit pada pelanggan yang sebenarnya memilih bertahan atau loyal.
- Kebalikan dari poin pertama, Kesalahan proporsi prediksi pelanggan yang ditandai sebagai _Not Churn_ lebih besar dari yang ditandai _Churn_, sehingga perusahaan akan merasa pada posisi aman namun tidak menyadari bahwa pelanggan mulai meninggalkan perusahaan.

### Performance Measure
Metrik yang digunakan untuk mengukur kemampuan model dalam melakukan prediksi, yakni :
- Recall
- Precision
- F1 score

## 5. Action
Para _Stakeholder_ dapat memanfaatkan hasil prediksi untuk menentukan standar pelanggan loyal dan pelanggan tidak loyal.

## 6. Value
Hasil atau nilai tambah yang dapat diciptakan dari proyek ini yakni adanya peningkatan dalam proses penentuan keputusan dalam kegiatan pemasaran, dan acuan dalam standar penetuan pelanggan diklasifikasikan sebagai pelanggan loyal, yang mana pelanggan loyal adalah sumber terbesar keuntungan perusahaan, tidak hanya dampak baik pada keuangan tetapi juga pada citra perusahaan, sehingga perusahaan harus dapat mempertahankan retensi pelanggan dan terus membina hubungan baik dengan pelanggan, yang nanti dapat memaksimalkan keuntungan dan menurunkan kerugian.

---

# II. Data Understanding

### Informasi Fitur :
<br>

Terdapat `7043` data observasi dengan `21` fitur dan `1` label (`Churn`)

|__No.__|__Fitur__|__Deskripsi__|__Tipe Data__|
| - | - | - | - |
|1| **Customer ID** | Menunjukkan nomor ID yang mengidentifikasi setiap pelanggan | Kategorikal, Objek |
|2|	**Gender** | Menunjukkan Jenis kelamin pelanggan (Pria, Wanita) | Kategorikal, Objek |
|3|	**Senior Citizen** | Menunjukkan jika pelanggan berusia 65 tahun atau lebih (Ya = 1, Tidak = 0) | Numerik, Integer |
|4|	**Partner** | Menunjukkan apakah pelanggan memiliki pasangan atau tidak (Ya, Tidak) | Kategorikal, Objek | 
|5|	**Dependents** | Menunjukkan jika pelanggan tinggal dengan tanggungan, bisa tanggungan anak-anak, orang tua, kakek-nenek, dll (Ya, Tidak)| Kategorikal, Objek |
|6|	**Tenure** | Menunjukkan jumlah bulan pelanggan telah tinggal atau berlangganan | Numerik, Integer |
|7|	**Phone Service** | Menunjukkan apakah pelanggan memiliki layanan telepon atau tidak (Ya, Tidak) | Kategorikal, Objek |
|8|	**Multiple Lines** | Menunjukkan jika pelanggan berlangganan beberapa saluran telepon dengan perusahaan (Ya, Tidak) | Kategorikal, Objek |
|9|	**Internet Service** | Menunjukkan jika pelanggan berlangganan layanan Internet dengan perusahaan (Tidak, DSL, Fiber Optic, Kabel) | Kategorikal, Objek |
|10|	**Online Security** | Menunjukkan jika pelanggan berlangganan layanan keamanan online tambahan yang disediakan oleh perusahaan (Ya, Tidak) | Kategorikal, Objek |
|11|	**Online Backup** | Menunjukkan jika pelanggan berlangganan layanan pencadangan online tambahan yang disediakan oleh perusahaan (Ya, Tidak) | Kategorikal, Objek |
|12|	**Device Protection** | Menunjukkan jika pelanggan berlangganan paket perlindungan perangkat tambahan untuk peralatan Internet mereka yang disediakan oleh perusahaan (Ya, Tidak) | Kategorikal, Objek |
|13|	**Tech Support** | Menunjukkan jika pelanggan berlangganan paket dukungan teknis tambahan dari perusahaan dengan waktu tunggu yang lebih singkat (Ya, Tidak) | Kategorikal, Objek |
|14|	**Streaming TV** | Menunjukkan jika pelanggan menggunakan layanan Internet mereka untuk melakukan streaming program televisi dari penyedia pihak ketiga, perusahaan tidak mengenakan biaya tambahan untuk layanan ini (Ya, Tidak) | Kategorikal, Objek |
|15|	**Streaming Movies** | Menunjukkan jika pelanggan menggunakan layanan Internet mereka untuk streaming film dari penyedia pihak ketiga, perusahaan tidak mengenakan biaya tambahan untuk layanan ini (Ya, Tidak) | Kategorikal, Objek |
|16|	**Contract** | Menunjukkan jenis kontrak pelanggan saat ini(Bulan-ke-Bulan, Satu Tahun, Dua Tahun) | Kategorikal, Objek |
|17|	**Paperless Billing** | Menunjukkan jika pelanggan telah memilih penagihan tanpa kertas (Ya, Tidak) | Kategorikal, Objek |
|18|	**Payment Method** | Menunjukkan bagaimana metode pelanggan membayar tagihan mereka (Penarikan Bank, Kartu Kredit, Cek yang Dikirim) | Kategorikal, Objek |
|19|	**Monthly Charges** | Menunjukkan total biaya bulanan pelanggan saat ini untuk semua layanan mereka dari perusahaan | Numerik, Float |
|20|	**Total Charges** | Menunjukkan total biaya pelanggan | Kategorikal, Objek |
|21|	**Churn** | Menunjukkan apakah pelanggan churn atau tidak (Ya atau Tidak) | Kategorikal, Objek |
<br>

Selengkapnya --> [EDA - Data Preparation Notebook](https://github.com/Kresnadwipsh/Telco_Costumer_Churn/blob/main/EDA%20-%20Data%20Preparation.ipynb)

---

# III. Modeling

Selengkapnya --> [Model Notebook](https://github.com/Kresnadwipsh/Telco_Costumer_Churn/blob/main/Model.ipynb)

---

# IV. Conclusion

### Final Conclusion :
- Model klasifikasi yang dipilih adalah _Logistic Regression_, hal ini berdasarkan pertimbangan dari hasil _recall_, kecepatan performa dan kestabilan model _Logistic Regression_ yang lebih baik dari model lainnya , saya menggunakan model _Logistic Regression_ tanpa tuning dikarenakan performa yang lebih baik yakni sebesar 80% dibandingkan setelah tuning yang menurun menjadi 79%

- Berdasarkan korelasi variabel numerik, dapat dilihat fitur _Monthly Charges_ cukup berpengaruh terhadap _Churn_, artinya besaran biaya bulanan pelanggan cukup mempengaruhi pelanggan untuk beralih, sehingga harus diperhatikan besaran biaya dengan kemampuan keuangan setiap pelanggan untuk menghidari pelanggan beralih

- Pada _Confusion Matrix_ , model _Machine Learning_ yang dikembangkan dapat meminimalisir kesalahan prediksi pelanggan _Not Churn_ tetapi sebenarnya _Churn_ (FN) yang hanya sebesar 8,64%, artinya dari 100 pelanggan yang diteliti, hanya ada 9 pelanggan yang salah prediksi atau pelanggan yang beralih dan tidak mendapatkan pelakuan tertentu, hal ini menjadi fokus karena pada penelitian ini saya mengutamakan penurunan _False Negatif Rate_, karena berbahaya jika perusahaan tidak melakukan perlakuan tertentu terhadap pelanggan yang ingin beralih hanya karena salah prediksi 

- Namun disini juga harus diperhatikan bahwa _False Positive Rate_ yang tinggi yakni sebesar 48,97%, artinya dari 100 pelanggan yang diteliti, terdapat 49 pelanggan yang mendapat pelakuan tertentu yang sebenarnya tidak perlu dikarenakan pelanggan tersebut sebenarnya tidak berpotensi untuk beralih, hal ini jika berlanjut dapat menjadi sumber kerugian perusahaan

- Di akhir, saya membuat prediksi pada dataset berdasarkan _test set_ dengan memberikan probabilitas pada setiap kelas, untuk memetakan pelanggan mana saja yang bertahan namun memiliki potensi untuk _Churn_, dengan melihat rata" nilai probabilitas _Non Churn_ yang mana jika pelanggan (_churn_ = 0) dengan nilai probabilitas < 0,4233, artinya memiliki indikasi untuk beralih. Pemetaan ini juga menjadi wujud supaya hasil penelitian ini dapat langsung diaplikasikan pada produk yang membutuhkan dan dapat meningkatkan akurasi prediksi.

### Business Insight :
- **Perusahaan harus memperhatikan :**
     - Senior Citizen (> 65 tahun), karena tingkat churn tertinggi
     - memperbaiki kualitas internet karena ada indikasi kualitas yang kurang baik
     - Memperhatikan daya beli pelanggan, sehingga pelanggan tidak beralih karena alasan tagihan

<br>

- **Perusahaan sebaiknya melakukan :**
     - Perusahaan dapat memilih segmentasi pelanggan, sebaiknya fokus pada pelanggan muda karena mayoritas pelanggan perusahaan adalah kelompok usia muda.
     - Dapat memberlakukan promosi diskon potongan harga, untuk mempertahankan pelanggan yang berlangganan jangka pendek sehingga menghindari pelanggan beralih kepada kompetitor yang memberikan benefit lebih menguntungkan, serta memberikan diskon spesial pada pelanggan usia tua untuk menghindari churn karena masalah biaya. 
     - Kualitas Internet Service harus ditingkatkan karena fitur ini adalah fitur dasar bagi seluruh produk yang dimiliki perusahaan, dan karena ada indikasi kuat pelanggan churn umumnya karena fitur ini.  
     - Memberikan benefit khusus kepada pelanggan loyal untuk menyebarkan strategi wom, karena perusahaan memiliki cukup banyak pelanggan loyal, dan strategi ini akan dapat menghemat banyak biaya operasional. 
     - Perusahaan dapat fokus pada produk Internet Service dan Phone Service, karena kedua produk tersebut merupakan produk unggulan.
     - Kualitas sistem pembayaran harus ditingkatkan, harus mengutamakan proses automasi untuk memotong alur proses pembayaran yang tidak efisien dan tidak efektif.
---


