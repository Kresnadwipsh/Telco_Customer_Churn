# FINAL PROJECT - TELCO COSTUMER CHURN PREDICTION
by : PURWADHIKA JSDS - Scipy Team
 - Kresna Dwipayana S H
 - Dimas
 
 Dataset : WA_Fn-UseC_-Telco-Customer-Churn.csv
 
 Source :  <a href="https://www.kaggle.com/blastchar/telco-customer-churn">Kaggle</a>
 
 ---
 
 # Background

Dalam bisnis, mendapatkan pelanggan merupakan tujuan utama perusahaan. Namun ada kala pelanggan memilih beralih dengan berbagai alasan, yang nanti akan berdampak pada perusahaan.
 Peralihan itu disebut _Customer Churn_. Sehingga perlu diperhatikan _Churn Rate_ supaya memastikan retensi pelanggan pada suatu perusahaan tetap baik.
 
 Dalam proyek ini, kami memposisikan diri sebagai bagian dari tim Data Scientist pada sebuah perusahaan _Telco_ di Indonesia.
 Kami ingin meneliti perilaku pelanggan dan memastikan pelanggan mana yang bertahan dan tidak. Kami ingin membantu tim Pemasaran dengan membuat pemetaan pelanggan, supaya tim Pemasaran dapat melakukan kegiatan pemasaran tepat sasaran. 
 
 ---
 
 # I. Problem Statement
 
 ## 1. Problem Definition
 
 Dalam kasus ini, kami menemukan bahwa beberapa pelanggan memilih beralih atau menghentikan interaksi mereka terhadap perusahaan, namun kami tidak mengetahui alasan pelanggan tersebut memilih beralih. Perusahaan tidak mengetahui dampak keuangan dari beralihnya pelanggan.
 
 Selain itu tim marketing kesulitan untuk menentukan pelanggan yang mana diperkirakan akan beralih untuk nanti diberikan sejumlah benefit atau diskon, sehingga menghindari dari pelanggan memilih beralih.
 
 <img src="https://www.jojonomic.com/wp-content/uploads/2020/11/34.-Churn1.jpg" width="500" />
 
 Untuk mengatasi masalah tersebut, perusahaan memerlukan :
 - Pemetaan mengenai produk unggulan dan non-unggulannya untuk kedepannya dapat dioptimalisasikan pelayanannya 
 - Pemetaan pelanggan mana yang di prediksi beralih atau tidak beralih supaya tim marketing dapat menyesuaikan kegiatan pemasarannya dengan karakteristik pelanggan. 
 - Visualisasi dampak dari _customer churn_ terhadap keuangan perusahaan

Hasil yang diharapkan dari proyek ini adalah dapat menghasilkan sistem yang dapat mengklasifikasikan pelanggan yang berpotensi melakukan _churn_ dan pelanggan yang bertahan secara akurat dengan menggunakan pendekatan Machine Learning, sehingga dapat memberikan informasi pada stakeholder dan dapat dimanfaatkan untuk mencapai tujuan bisnis. 

## 2. Business Objective 

Adapun terdapat beberapa tujuan bisnis yang ingin dicapai melalui proyek ini, yakni sebagai berikut :
- Memaksimalkan keuntungan dengan memastikan pelanggan untuk tidak memutuskan interaksi bisnis atau memilih beralih dari perusahaan
- Memastikan pelanggan yang mendapat sejumlah benefit atau diskon tepat sasaran dan menjadi pelanggan yang loyal atau bertahan
- Meminimalisir kerugian dengan mengoptimalkan layanan unggulan

## 3. Data Requirements
 
Dalam proyek ini, berdasarkan _problem definition_ yang telah didefinisikan , maka kami membutuhkan data sebagai fitur meliputi daftar pelanggan, perilaku pelanggan, karakteristik pelanggan,  total tagihan, DLL.
 
## 4. Analytic Approach

### Machine Learning Technique :
Pada proyek ini, karena kami ingin memprediksi pelanggan mana yang akan memilih beralih atau bertahan , dan kami memiliki label yakni _Churn_ dan _Not churn_, sehingga hal ini dapat diatasi dengan metode _supervised learning_ yang fokus pada klasifikasi. Kami akan memberikan data pada model dengan algortima klasifikasi untuk dipelajari atau di _training_, yang hasilnya kami harap dapat membuat prediksi yang baik dan akurat untuk memprediksi pelanggan mana yang akan memilih beralih atau bertahan. 

### Risk :
Terdapat beberapa resiko yang dapat disebabkan kesalahan prediksi dari model, yakni :
- Kesalahan proporsi prediksi pelanggan yang ditandai sebagai _Churn_ lebih besar dari yang ditandai _Not Churn_, sehingga kemungkinan perusahaan dapat berlebihan mengeluarkan anggaran promosi dan merugikan keuangan perusahaan karena memberikan benefit pada pelanggan yang sebenarnya memilih bertahan atau loyal.
- Kebalikan dari poin pertama, Kesalahan proporsi prediksi pelanggan yang ditandai sebagai _Not Churn_ lebih besar dari yang ditandai _Churn_, sehingga perusahaan akan merasa pada posisi aman namun tidak menyadari bahwa pelanggan mulai meninggalkan perusahaan.

### Performance Measure
Metrik yang digunakan untuk mengukur kemampuan model dalam melakukan prediksi, yakni :
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Median Absolute Error dan Koefisien Determinasi (R²).

## 5. Action
Para _Stakeholder_ dapat memanfaatkan hasil prediksi untuk menentukan standar pelanggan loyal dan pelanggan tidak loyal.

## 6. Value
Hasil atau nilai tambah yang dapat diciptakan dari proyek ini yakni adanya peningkatan dalam proses penentuan keputusan dalam kegiatan pemasaran, dan acuan dalam standar penetuan pelanggan diklasifikasikan sebagai pelanggan loyal, yang mana pelanggan loyal adalah sumber terbesar keuntungan perusahaan, tidak hanya dampak baik pada keuangan tetapi juga pada citra perusahaan, sehingga perusahaan harus dapat mempertahankan retensi pelanggan dan terus membina hubungan baik dengan pelanggan, yang nanti dapat memaksimalkan keuntungan dan menurunkan kerugian.

---

# II. Data Understanding

---

# III. Data Preparation

---

# IV. Modeling

---

# V. Evaluation

---

# VI. Deployment & Feedback

---


