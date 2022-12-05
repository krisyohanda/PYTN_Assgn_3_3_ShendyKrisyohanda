## Ulasan Proyek

Tujuan dari proyek ini adalah untuk memprediksi apakah klien akan berlangganan (ya/tidak) deposito berjangka (variabel y). Data tersebut terkait dengan kampanye pemasaran langsung dari lembaga perbankan Portugis. Kampanye pemasaran didasarkan pada panggilan telepon. Seringkali, lebih dari satu kontak ke klien yang sama diperlukan, untuk mengakses apakah produk (deposit berjangka bank) akan ('ya') atau tidak ('tidak') berlangganan.  

Ada 4 dataset:  
1. **bank-additional-full.csv** with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]
2. **bank-additional.csv** with 10% of the examples (4119), randomly selected from 1), and 20 inputs.
3. **bank-full.csv** with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs).
4. **bank.csv** with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs).  

Dataset terkecil disediakan untuk menguji algoritma machine learning yang lebih menuntut komputasi (mis., SVM).  

Kumpulan data ini berisi:  

**bank client data:**
- `age` **(numeric)**
- `job` : **type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')**
- `marital` : **marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)**
- `education` **(categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')**
- `default`: **has credit in default? (categorical: 'no', 'yes', 'unknown')**
- `housing`: **has housing loan? (categorical: 'no', 'yes', 'unknown')**
- `loan`: **has personal loan? (categorical: 'no', 'yes', 'unknown')**

**related with the last contact of the current campaign:**
- `contact`: **contact communication type (categorical: 'cellular', 'telephone')**
- `month`: **last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')**
- `day_of_week`: **last contact day of the week (categorical: 'mon', 'tue', 'wed', 'thu', 'fri')**
- `duration`: **last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.**

**other attributes:**
- `campaign`: **number of contacts performed during this campaign and for this client (numeric, includes last contact)**
- `pdays`: **number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)**
- `previous`: **number of contacts performed before this campaign and for this client (numeric)**
- `poutcome`: **outcome of the previous marketing campaign (categorical: 'failure', 'nonexistent', 'success')**

**social and economic context attributes**
- `emp.var.rate`: **employment variation rate - quarterly indicator (numeric)**
- `cons.price.idx`: **consumer price index - monthly indicator (numeric)**
- `cons.conf.idx`: **consumer confidence index - monthly indicator (numeric)**
- `euribor3m`: **euribor 3 month rate - daily indicator (numeric)**
- `nr.employed`: **number of employees - quarterly indicator (numeric)**

**Output variable (desired target):**
- `y`: **has the client subscribed a term deposit? (binary: 'yes', 'no')**

## Rubrik Proyek

Ulasan Kode

| Kriteria | Memenuhi Harapan 
| ----------- | ----------- |
| Logistic Regression | Mengimplementasikan Logistic Regression Dengan Scikit-Learn.
| K-Nearest Neighbors | Mengimplementasikan K-Nearest Neighbors Dengan Scikit-Learn.
| Support Vector Machine | Mengimplementasikan Support Vector Machine Dengan Scikit-Learn.
| Decision Tree | Mengimplementasikan Decision Tree Dengan Scikit-Learn.
| Random Forest | Mengimplementasikan Random Forest Dengan Scikit-Learn.
| Naive Bayes | Mengimplementasikan Naive Bayes Dengan Scikit-Learn.
| Confusion Matrix | Mengimpelentasikan Confusion Matrix Regression Dengan Scikit-Learn.
| Visualization | Menganalisa Data Menggunakan Setidaknya 2 Tipe Grafik/Plot.
| Preprocessing | Melakukan Preproses Dataset Sebelum Melakukan Penelitian Lebih Dalam.
| Apakah Kode Berjalan Tanpa Ada Eror? | Kode Berjalan Tanpa Ada Eror. Seluruh Kode Berfungsi Dan Dibuat Dengan Benar.
  
Readability/Keterbacaan  

| Kriteria | Memenuhi Harapan 
| ----------- | ----------- |
| Tertata Dengan Baik | Semua Cell Di Notebook Terdokumentasi Dengan Baik Dengan Markdown Pada Tiap Cell Untuk Penjelasan Kode.
  
Analisis

| Kriteria | Memenuhi Harapan 
| ----------- | ----------- |
| Algorithm Analysis | Student Menjelaskan Alasan Mengapa Memilih Menggunakan Algoritma Tersebut Untuk Membuat Model.