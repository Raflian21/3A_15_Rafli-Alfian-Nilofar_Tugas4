# Rafli Alfian Nilofar / TI - 3A / 15

# Tugas 4
| 1. SystemCommandsOutput.scala |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/d8c1c4c4e7504b66a917b414926c5d6ae300304e/SystemCommandsOutput.scala#L1-L3 |
| ![image](https://user-images.githubusercontent.com/95726593/231009979-58557000-35b5-45b9-8cdc-a26407abba02.png)
![image](https://user-images.githubusercontent.com/95726593/231009999-eb536917-28fd-4405-97d1-df17f154a07f.png)
![image](https://user-images.githubusercontent.com/95726593/231010015-5bf5b19a-b28a-4cfa-bc73-8a4c1a0925c1.png)|
|import sys.process berfungsi untuk mengimport library sys.process|

| 2. SystemCommandsReturnCode.scala |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/ddf78d46c4d6fc6290e216a7ea7e8192e60eb723/SystemCommandsReturnCode.scala#L1-L3 |
| ![image](https://user-images.githubusercontent.com/95726593/231028674-4c5b7667-1c61-4377-a8d1-4206c710bd26.png)![image](https://user-images.githubusercontent.com/95726593/231028718-932c4486-685a-4ba5-93f3-5670e13d5629.png)|
|import sys.process berfungsi untuk mengimport library sys.process|

| 3. Accumulator.py |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/27ee8696c1d1dff6088b71e4cfe72dd477e3adbc/Accumulator.py#L1-L4 |
| ![image](https://user-images.githubusercontent.com/95726593/231029612-a6d17169-7f64-4206-a6c1-3ea3dcffcbdd.png) |
| parallelize merupakan metode pada objek SparkContext yang mengubah koleksi objek menjadi RDD (Resilient Distributed Datasets) yang terdistribusi secara paralel di beberapa node dalam kluster Spark. |
| accumulator merupakan suatu objek di Spark yang dapat diakses secara paralel dan dapat digunakan untuk menjalankan operasi agregasi seperti penghitungan jumlah atau rata-rata dalam lingkungan yang terdistribusi. |
| value berfungsi untuk mengembalikan nilai dalam variabel yang diakses secara bersamaan dalam lingkungan yang terdistribusi. |
| lambda merupakan fungsi anonim dalam Python yang digunakan untuk operasi pemetaan atau filtering pada data RDD. | 

| 4. BroadCast.py |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/73c95b4a4303174692deddaa6601d4f625aef7c3/BroadCast.py#L1-L2 |
| ![image](https://user-images.githubusercontent.com/95726593/231029852-4b496b87-d352-4fe8-81e4-19ff6cc6bd73.png) |
|range merupakan fungsi dalam Python yang menghasilkan urutan angka dalam rentang tertentu|
|broadcast adalah mekanisme dalam Spark untuk mengirim data besar ke setiap node dalam kluster tanpa mengulanginya untuk setiap tugas pemrosesan.|
|list merupakan struktur data dalam Python yang digunakan untuk menyimpan kumpulan elemen yang terurut dan dapat diakses dengan indeks.|

| 5. PairRDD.py |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/daa32022c38d2b9bdcd50a8a6df5bdc95b8933ef/PairRDD.py#L1-L11 |
| ![image](https://user-images.githubusercontent.com/95726593/231030025-78df7a0b-8e2c-46c1-937e-50b27b65ed0d.png) |
|collect digunakan untuk mengumpulkan semua elemen RDD menjadi suatu koleksi pada driver program.|
|keys berfungsi untuk mengembalikan RDD baru yang hanya terdiri dari kunci dalam setiap pasangan kunci dan nilai di RDD.|
|map berfungsi untuk mengaplikasikan fungsi pada setiap elemen PairRDD dan mengembalikan RDD baru yang terdiri dari pasangan kunci dan nilai baru.|
|len berfungsi untuk menghitung jumlah elemen dalam RDD.|
|values berfungsi untuk mengembalikan RDD baru yang hanya terdiri dari nilai dalam setiap pasangan kunci dan nilai di RDD.|

| 6. LogAnalytics.py |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/5f572711294d9de182c86587dbbd803a825c8cac/LogAnalytics.py#L1-L27 |
| ![image](https://user-images.githubusercontent.com/95726593/231031238-98ec6b4f-c7b4-41e7-ba46-1989a3b1aad3.png) |
|cache berfungsi untuk menyimpan RDD di memori untuk mengoptimalkan kinerja proses pengolahan data berulang.|
|count berfungsi untuk menghitung jumlah elemen dalam RDD.|
|filter berfungsi untuk memfilter baris-baris teks yang mengandung pola tertentu dalam RDD.|
|textFile berfungsi untuk membaca file log dan mengembalikan RDD baru dengan satu baris teks sebagai elemen RDD.|

| 7. WordCount.py |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/90f36e1a876d521c95c06028e024be0a4047bca6/WordCount.py#L1-L8 |
| ![image](https://user-images.githubusercontent.com/95726593/233122626-f6e547cd-3fb2-42e2-815b-a5e4d9065285.png) |
|reduceByKey berfungsi untuk menghitung jumlah kemunculan kata pada RDD.|
|flatMap berfungsi untuk memisahkan setiap baris dalam teks menjadi kata-kata terpisah.|
|split berfungsi untuk memecah setiap baris teks menjadi array kata-kata yang terpisah berdasarkan pemisah spasi atau karakter lain yang ditentukan.|

| 8. UnderstandingRDDs.py |
| ------  |
| https://github.com/Raflian21/3A_15_Rafli-Alfian-Nilofar_Tugas4/blob/a06ec570da5aea44310096e070aadd7546cdaeca/UnderstandingRDDs.py#L11-L40 |
| ![image](https://user-images.githubusercontent.com/95726593/233124121-53147de1-ac72-40f8-93c4-c8b593f64057.png) |
|mapPartitionsWithIndex berfungsi untuk menerapkan fungsi pada setiap partisi RDD dengan indeks partisi sebagai parameter masukan.|
|getNumPartitions berfungsi untuk mendapatkan jumlah partisi yang digunakan oleh RDD saat ini.|
|defaultParallelism berfungsi untuk mendapatkan jumlah partisi default yang digunakan oleh RDD.|
|coalesce berfungsi untuk menggabungkan beberapa partisi menjadi satu partisi.|
|repartition berfungsi untuk memecah ulang RDD menjadi sejumlah partisi yang baru.|
