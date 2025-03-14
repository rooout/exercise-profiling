![Screenshot 2025-03-14 203929.png](image/Screenshot%202025-03-14%20203929.png)
![Screenshot 2025-03-14 203938.png](image/Screenshot%202025-03-14%20203938.png)
![Screenshot 2025-03-14 203949.png](image/Screenshot%202025-03-14%20203949.png)
![Screenshot 2025-03-14 203959.png](image/Screenshot%202025-03-14%20203959.png)
![Screenshot 2025-03-14 204044.png](image/Screenshot%202025-03-14%20204044.png)
![Screenshot 2025-03-14 204053.png](image/Screenshot%202025-03-14%20204053.png)

all-student

Sebelum dioptimalkan, waktu eksekusi untuk menjalankan permintaan sekitar 80.000 ms. Setelah optimasi, waktu eksekusi berkurang menjadi 3.700 ms.
Optimasi ini menghasilkan peningkatan kecepatan hingga 2.100% lebih cepat.
all-student-name

Sebelum optimasi, waktu eksekusi untuk menjalankan permintaan sekitar 1.800 ms. Setelah optimasi, waktu eksekusi menurun menjadi 80 ms.
Perbaikan ini meningkatkan kecepatan hingga 2.250% lebih cepat.
highest-gpa

Sebelum optimasi, waktu eksekusi untuk menjalankan permintaan sekitar 75 ms. Setelah optimasi, waktu eksekusi berkurang menjadi 15 ms.
Hasil optimasi ini meningkatkan kecepatan hingga 500% lebih cepat.


Refleksi
Perbedaan Pengujian Kinerja dengan JMeter dan Profiling dengan IntelliJ Profiler

JMeter digunakan untuk menguji performa dengan menyimulasikan banyak pengguna dan mengukur respons sistem di bawah beban tertentu. Alat ini berguna untuk mengidentifikasi masalah seperti latensi, throughput, dan pemanfaatan sumber daya dalam kondisi stres.
IntelliJ Profiler, di sisi lain, fokus pada analisis internal aplikasi, termasuk penggunaan CPU, alokasi memori, dan durasi eksekusi metode.
Sederhananya, JMeter memberikan gambaran menyeluruh tentang performa sistem, sementara IntelliJ Profiler memberikan wawasan mendalam tentang hambatan di tingkat kode.
Peran Profiling dalam Mengidentifikasi Kelemahan Aplikasi

Dengan profiling, saya dapat mengidentifikasi bagian kode yang kurang efisien, operasi berlebihan, serta kemungkinan kebocoran memori.
Analisis ini membantu menemukan bagian kode yang memperlambat sistem dan membutuhkan optimasi lebih lanjut.
Efektivitas IntelliJ Profiler dalam Mengidentifikasi Bottleneck

IntelliJ Profiler sangat membantu dalam menemukan hambatan performa dengan menyajikan visualisasi detail tentang penggunaan CPU dan memori.
Dengan alat ini, saya dapat mendeteksi jalur kode yang tidak optimal serta proses yang menghambat efisiensi aplikasi.
Tantangan dalam Pengujian Kinerja dan Profiling

Data yang dihasilkan dari pengujian kinerja dan profiling bisa sangat kompleks, sehingga membutuhkan analisis mendalam untuk mendapatkan kesimpulan yang akurat.
Untuk mengatasi tantangan ini, saya memastikan observasi yang cermat agar dapat mengambil kesimpulan yang tepat dari data yang diperoleh.
Manfaat Menggunakan IntelliJ Profiler

Analisis Mendalam → Memberikan wawasan detail tentang eksekusi kode dan inefisiensi.
Pemantauan Waktu Nyata → Memungkinkan pengamatan perubahan kinerja secara langsung saat aplikasi berjalan.
Integrasi dengan IntelliJ IDEA → Mempermudah debugging dan optimasi melalui integrasi langsung dengan IDE.
Menangani Perbedaan Hasil Profiling dan Pengujian Kinerja

Kadang, hasil profiling dengan IntelliJ Profiler tidak selalu selaras dengan pengujian performa menggunakan JMeter.
Untuk mengatasi hal ini, saya melakukan pengecekan silang antara metrik performa tingkat sistem dan analisis di tingkat kode.
Perbedaan bisa disebabkan oleh faktor eksternal seperti latensi jaringan, kinerja database, atau proses latar belakang yang berjalan.
Strategi Optimalisasi Kode Aplikasi

Refactoring Kode → Memperbaiki algoritma yang kurang efisien dan menghilangkan operasi yang tidak perlu.
Optimasi Memori → Mengidentifikasi serta mengatasi kebocoran memori guna mengurangi penggunaan sumber daya yang berlebihan.
Optimasi Query Database → Memperbaiki interaksi dengan database untuk mengurangi eksekusi query yang lambat.
Untuk memastikan optimasi tidak berdampak negatif terhadap aplikasi, saya mengikuti beberapa langkah:

Melakukan pengujian menyeluruh setelah perubahan kode.
Melakukan pengujian performa sebelum dan sesudah optimasi untuk mengukur perbedaan kinerja.
Memantau metrik performa dunia nyata setelah implementasi guna memvalidasi peningkatan yang telah dilakukan.

