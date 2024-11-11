# image_identifications
Project Exercise untuk Bootcamp DBS Foundation. Project ini bertujuan untuk mengidentifikasi apakah suatu gambar termasuk gunting, batu atau kertas.

# Pendahuluan
## Definisi Image Identifikasi
Image identifikasi adalah proses pengenalan objek, karakter, atau pola dalam gambar menggunakan teknologi komputer, sering kali melibatkan algoritma pembelajaran mesin. Ini memungkinkan sistem untuk menganalisis dan memahami konten visual, seperti mengenali wajah, kendaraan, atau produk, untuk aplikasi seperti keamanan, otomasi, dan pencarian gambar.

## Metode Image Identifikasi
Dalam project ini, image identifikasi dilakukan dengan membangun model sequential. 
### Definisi Model Sequential
Model Sequential adalah arsitektur dalam deep learning yang mengatur lapisan-lapisan neuron secara berurutan, dimana output dari satu lapisan menjadi input bagi lapisan berikutnya. Model ini sering digunakan dalam tugas pemodelan yang memerlukan urutan data, seperti dalam pengenalan citra dan pemrosesan bahasa alami.
#### Peran Model Sequential dalam Image Identifikasi
- Model Sequential dalam image identifikasi berfungsi sebagai arsitektur dasar untuk merancang jaringan saraf dalam mengklasifikasikan gambar.
- Dalam model ini, lapisan-lapisan neural disusun secara linier, di mana setiap lapisan terhubung langsung ke lapisan berikutnya.
- Pada umumnya, lapisan convolutional digunakan untuk mengekstrak fitur dari gambar, diikuti oleh lapisan pooling untuk mengurangi dimensi, dan akhirnya lapisan fully connected untuk membuat keputusan klasifikasi.
- Keuntungan dari model Sequential adalah kesederhanaannya dalam membangun dan mengimplementasikan jaringan, memungkinkan pengembang untuk fokus pada eksperimen dengan hyperparameter dan arsitektur.

# Algoritma-algoritma dalam Image Identifikasi
Dalam proses image identifikasi, penggunaan library seperti linear_model (dari scikit-learn), TensorFlow, dan keras.preprocessing memiliki peran yang penting, masing-masing untuk berbagai aspek dalam pelatihan dan evaluasi model. Berikut ini adalah penjelasan detail mengenai fungsinya:

## linear_model (scikit-learn):
1. Libray ini menawarkan berbagai algoritma pembelajaran mesin, dengan fokus khusus pada algoritma pembelajaran yang diawasi. Meskipun algoritma ini biasanya digunakan untuk data berbasis fitur, model seperti Regresi Logistik dan Support Vector Machines (SVM) dapat digunakan untuk klasifikasi gambar setelah fitur-fiturnya diekstraksi.
2. Peran algoritma ini dalam identifikasi gambar adalah sebagai berikut:
   Dalam konteks identifikasi gambar, algoritma ini dapat digunakan untuk memproses fitur dari gambar (misalnya, ekspektasi dari CNN) untuk melakukan klasifikasi, terutama untuk set data yang lebih kecil atau sebagai bagian dari pipeline model ensemble.

## TensorFlow:
1. Fungsinya adalah sebagai adalah kerangka kerja pembelajaran mesin dan pembelajaran mendalam bersumber terbuka yang memungkinkan pengguna untuk membangun dan melatih model jaringan saraf.
2. TensorFlow berperan dalam identifikasi gambar. Dalam bidang identifikasi gambar, TensorFlow digunakan untuk mengembangkan model jaringan syaraf yang mampu menganalisis pola dalam data gambar. Hal ini mencakup pembangunan arsitektur seperti Convolutional Neural Networks (CNN), yang sangat efektif dalam pengenalan gambar. TensorFlow juga menawarkan dukungan untuk pelatihan dan pengoptimalan model berskala besar melalui GPU.

## keras.preprocessing:
1. Fungsi: Modul ini dalam Keras menyediakan fungsi untuk memproses dan mempersiapkan data gambar sebelum memasukkannya ke dalam model. Ini termasuk fungsi untuk augmentasi gambar, pengubahan ukuran, dan normalisasi.
2. Peran dalam Image Identifikasi: Persiapan data adalah tahap penting dalam image identifikasi. keras.preprocessing membantu memastikan bahwa data gambar berada dalam format yang tepat dan dalam kondisi optimal untuk pelatihan model. Augmentasi dapat meningkatkan keragaman data, membantu model menjadi lebih robust terhadap variasi input.

Secara keseluruhan, kombinasi library ini memungkinkan proses image identifikasi yang lebih efisien dan efektif, dengan masing-masing berkontribusi pada aspek yang berbeda dari pipeline machine learning: fitur ekstraksi, model pembuatan, dan preprocessing data.

# Hasil Image Identifikasi 
- Menunjukkan proses evaluasi yang telah berlangsung pada 5 batch yang dievaluasi.
- Menghasilkan nilai loss sebesar 0.3149 dan nilai akurasi sebesar 0.9000 (atau 90%).
- Menunjukkan akurasi yang lebih spesifik (99.9997%) hasil evaluasi model pada data validasi.
