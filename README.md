# UTSPrakPM
Repo yang berisi notebook dan file README.md yang berisi penjelasan beserta tahapan yang dilalui dalam proses pembuatan model naive bayes

---

Terdapat beberapa tahapan yang dilalui dalam proses pembuatan model, yaitu :

## 1. Data Loading 
Dataset dalam format csv diunduh dari kaggle menggunakan library kagglehub dan dimuat menggunakan pandas, terdapat 10.000 baris data didalamnya.

## 2.Data Preprocessing
Dataset diperiksa terlebih dahulu untuk mengecek apakah ada data yang duplikat ataupun data yang kosong
Lalu setelah itu dicek apakah dataset memiliki data yang seimbang atau tidak dengan menghitung total jumlah data berdasarkan label
agar dapat mencegah terjadinya gejala overfitting ataupun underfitting, dan ditemukan tidak ada data yang kosong maupun duplikat serta data di dalam
dataset seimbang sehingga tidak memerlukan augmentasi data.
     
## 5. Data Splitting
Dataset dibagi menjadi dua bagian , yaitu data training dan data testing dengan perbandingan 70% untuk data training dan 30% untuk data testing.

## 7. Melatih model
Model Gaussian Naive Bayes digunakan dengan paramter default dan dilatih menggunakan data latih serta diuji menggunakan data testing.
   
## 9. Evaluasi Model
Model yang telah dilatih diukur tingkat akurasinya dengan membandingkan antara data hasil prediksi dengan data testing, serta untuk mengecek apakah model mengalami overfitting atau underfitting
dilakukan pengukuran f1 score serta diukur pula nilai presisi dan nilai recall dari model tersebut. Confusion matrix digunakan untuk mengukur seberapa baik model dalam memprediksi data yang dapat 
dilihat dari nilai TP, TN, FP , dan FN.

# Hasil

Berdasarkan tahapan-tahapan yang telah dilakukan diatas, didapatkan bahwa model Gaussian Naive Bayes yang dibuat mendapatkan skor akurasi sebesar 92.5 dan skor f1 sebesar 92.5 yang menandakan bahwa model tersebut tergeneralisasi dengan baik,
lalu berdasarkan tabel confusion matrix untuk prediksi menggunakan data testing didapatkan TP sebesar 1399 , TN sebesar 1378 , FN sebesar 101 , dan FP sebesar 122.


