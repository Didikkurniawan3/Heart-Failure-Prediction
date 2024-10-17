# Submission 2 Dicoding : Heart Failure Prediction

Nama: Didik Kurniawan

Username dicoding: didik_kurniawan03

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction) |
| Masalah | Gagal jantung adalah kondisi di mana jantung melemah sehingga tidak mampu memompa darah yang cukup ke seluruh tubuh. Kondisi ini dapat terjadi pada siapa saja, tetapi lebih sering dialami oleh orang yang berusia di atas 65 tahun. Gagal jantung merupakan salah satu penyakit yang mematikan, dengan tingkat kematian yang sangat tinggi. Kematian akibat gagal jantung masih termasuk yang tertinggi di dunia hingga saat ini.|
| Solusi machine learning | Permasalahan di atas menunjukkan tingginya angka kematian akibat penyakit ini, dan teknologi dapat menjadi solusi untuk mengatasinya. Salah satu teknologi yang dapat digunakan adalah machine learning. Dengan mengembangkan sistem prediksi untuk penyakit gagal jantung, diharapkan dapat membantu tenaga medis dan masyarakat dalam mendeteksi penyakit ini lebih dini, sehingga langkah-langkah pencegahan dan pengobatan dapat dilakukan lebih cepat dan efektif. |
| Metode pengolahan | Metode pengolahan data yang digunakan pada proyek ini adalah dengan menghapus atau *drop* beberapa fitur atau kolom yang tidak dibutuhkan, melakukan tahap *Data Ingestion* dengan membagi *dataset* menjadi *data training* dan *data evaluation* dengan rasio 8:2. Kemudian melakukan tahap *Data Validation* dengan cara melihat statistik data, *data schema*. Setelah itu melakukan tahap *Data Preprocessing* dengan melakukan transformasi fitur input pada data.  |
| Arsitektur model | Arsitektur model yang dibangun menggunakan sebuah *input layer* yang menerima data kategorikal dan numerik yang telah diproses terlebih dahulu. Kemudian terdapat dua buah *hidden layer* (Dense layer) dan sebuah Dropout layer serta sebuah *output layer*. |
| Metrik evaluasi | Metric yang digunakan pada model yaitu *AUC*, *Precision*, *Recall*, *ExampleCount*, *TruePositives*, *FalsePositives*, *TrueNegatives*, *FalseNegatives* dan *BinaryAccuracy* untuk mengevaluasi performa model sebuah klasifikasi |
| Performa model | Model yang dibuat menghasilkan performa yang cukup baik dalam memberikan sebuah prediksi dan dari pelatihan yang dilakukan menghasilkan *AUC*(1), *Precision*(90), *Recall*(89), *ExampleCount*(179), *TruePositives*(89), *FalsePositives*(1), *TrueNegatives*(89, *FalseNegatives*(0) dan *BinaryAccuracy*(0.994), Model telah menunjukkan kinerja yang sangat baik dengan akurasi yang tinggi dan nilai-nilai metrik evaluasi yang positif. Hal ini menandakan bahwa model mampu dengan baik. |
| Opsi deployment | Proyek *machine learning* Heart Failure Prediction ini telah di-*deploy* menggunakan [Railway App](https://railway.app) sebagai salah satu Platform as a Service (PaaS) yang menyediakan layanan untuk deploying proyek secara gratis.|
| Web app | Model serving dapat diakses melalui <https://heart-failure-detection-production.up.railway.app/v1/models/heart-failure-model> |
| Monitoring | Proses *monitoring* pada proyek *machine learning* ini dapat dilakukan menggunakan layanan *open-source*, yaitu [Prometheus](https://prometheus.io). Salah satu proses *monitoring* Prometheus adalah melihat perubahan jumlah permintaan yang dilakukan dengan cara menampilkan status dan informasi *request* beserta jamnya (`:tensorflow:serving:request_count`).|
| Kesimpulan | Model yang telah berhasil dibangun telah diuji coba dapat bekerja dan dapat melakukan prediksi untuk penyakit gagal jantung. |
