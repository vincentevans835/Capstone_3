## Latar Belakang


Dalam beberapa tahun terakhir, penggunaan travel insurance telah meningkat secara signifikan. Hal ini disebabkan oleh kesadaran akan risiko yang terkait dengan perjalanan, seperti pembatalan perjalanan, kehilangan bagasi, kecelakaan, atau keadaan darurat medis saat berada di luar negeri. Travel insurance memberikan perlindungan finansial bagi pelancong dalam menghadapi risiko-risiko ini.

Namun, bagi perusahaan asuransi, manajemen klaim travel insurance bisa menjadi proses yang rumit. Data yang dihasilkan dari klaim-klaim sebelumnya dapat memberikan wawasan berharga, namun memproses data ini secara manual sangatlah tidak efisien dan rentan terhadap kesalahan.
Oleh karena itu, perusahaan asuransi semakin beralih ke teknologi machine learning untuk membantu dalam menganalisis data klaim travel insurance.

## Feature Engineering
Target Kolom: Claim

Feature yang digunakan:
1. Agency
2. Agency Type
3. Distribution Channel
4. Product Name
5. Duration
6. Destination
7. Age

## Model Machine Learning:
1. Logistic Regression
2. Decision Tree
3. Random Forrest
4. XG Boost
5. Ada Boost

## Metrics

Type 1 error (False Positive): 
Diprediksi mengclaim asuransi tetapi sebenarnya tidak claim

Type 2 error (False Negative):
Diprediksi tidak claim asuransi tetapi sebenarnya mengclaim

Metrix yang digunakan: Recall

Mengunnakan Recall karena dalam kasus error jauh lebih baik False Positive karena jika False Negative maka client akan mendapatkan premi yang murah namun ternyata client tersebut mengclaim asuransi sehingga terjadi kerugian secara financial

## Pre Processing

1. Encoding:  
   a. Binary Encode,Kolom : Agency, Product Name, Destination  
   b. One Hot Encode,Kolom : Agency Type, Distribution Channel  
2. Scaling, Jenis: Robust Scaler, Kolom: Duration, Age
3. Resampling, Jenis: Random Under Sampler


