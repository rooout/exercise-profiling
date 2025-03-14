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

Result:
2025-03-14 20:59:35,406 INFO o.a.j.u.JMeterUtils: Setting Locale to en_EN
2025-03-14 20:59:35,417 INFO o.a.j.JMeter: Loading user properties from: user.properties
2025-03-14 20:59:35,417 INFO o.a.j.JMeter: Loading system properties from: system.properties
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: Copyright (c) 1998-2024 The Apache Software Foundation
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: Version 5.6.3
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: java.version=21.0.4
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: java.vm.name=OpenJDK 64-Bit Server VM
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: os.name=Windows 11
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: os.arch=amd64
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: os.version=10.0
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: file.encoding=UTF-8
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: java.awt.headless=true
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: Max memory     =1073741824
2025-03-14 20:59:35,422 INFO o.a.j.JMeter: Available Processors =16
2025-03-14 20:59:35,428 INFO o.a.j.JMeter: Default Locale=English (EN)
2025-03-14 20:59:35,429 INFO o.a.j.JMeter: JMeter  Locale=English (EN)
2025-03-14 20:59:35,429 INFO o.a.j.JMeter: JMeterHome=C:\Main Storage\Downloads\Download from Chrome\apache-jmeter-5.6.3\apache-jmeter-5.6.3
2025-03-14 20:59:35,429 INFO o.a.j.JMeter: user.dir  =C:\Main Storage\Downloads\Download from Chrome\apache-jmeter-5.6.3\apache-jmeter-5.6.3\bin
2025-03-14 20:59:35,429 INFO o.a.j.JMeter: PWD       =C:\Main Storage\Downloads\Download from Chrome\apache-jmeter-5.6.3\apache-jmeter-5.6.3\bin
2025-03-14 20:59:35,430 INFO o.a.j.JMeter: IP: 192.168.100.52 Name: LAPTOP-IDSJA4PC FullName: LAPTOP-IDSJA4PC
2025-03-14 20:59:35,445 INFO o.a.j.s.FileServer: Default base='C:\Main Storage\Downloads\Download from Chrome\apache-jmeter-5.6.3\apache-jmeter-5.6.3\bin'
2025-03-14 20:59:35,449 INFO o.a.j.s.FileServer: Set new base='C:\Main Storage\Downloads\Download from Chrome\apache-jmeter-5.6.3\apache-jmeter-5.6.3\bin'
2025-03-14 20:59:35,590 INFO o.a.j.s.SaveService: Testplan (JMX) version: 2.2. Testlog (JTL) version: 2.2
2025-03-14 20:59:35,621 INFO o.a.j.s.SaveService: Using SaveService properties version 5.0
2025-03-14 20:59:35,623 INFO o.a.j.s.SaveService: Using SaveService properties file encoding UTF-8
2025-03-14 20:59:35,626 INFO o.a.j.s.SaveService: Loading file: TestAdpro.jmx
2025-03-14 20:59:35,670 INFO o.a.j.p.h.s.HTTPSamplerBase: Parser for text/html is org.apache.jmeter.protocol.http.parser.LagartoBasedHtmlParser
2025-03-14 20:59:35,670 INFO o.a.j.p.h.s.HTTPSamplerBase: Parser for application/xhtml+xml is org.apache.jmeter.protocol.http.parser.LagartoBasedHtmlParser
2025-03-14 20:59:35,670 INFO o.a.j.p.h.s.HTTPSamplerBase: Parser for application/xml is org.apache.jmeter.protocol.http.parser.LagartoBasedHtmlParser
2025-03-14 20:59:35,670 INFO o.a.j.p.h.s.HTTPSamplerBase: Parser for text/xml is org.apache.jmeter.protocol.http.parser.LagartoBasedHtmlParser
2025-03-14 20:59:35,670 INFO o.a.j.p.h.s.HTTPSamplerBase: Parser for text/vnd.wap.wml is org.apache.jmeter.protocol.http.parser.RegexpHTMLParser
2025-03-14 20:59:35,670 INFO o.a.j.p.h.s.HTTPSamplerBase: Parser for text/css is org.apache.jmeter.protocol.http.parser.CssParser
2025-03-14 20:59:35,703 INFO o.a.j.JMeter: Creating summariser <summary>
2025-03-14 20:59:35,718 INFO o.a.j.e.StandardJMeterEngine: Running the test!
2025-03-14 20:59:35,718 INFO o.a.j.s.SampleEvent: List of sample_variables: []
2025-03-14 20:59:35,718 INFO o.a.j.s.SampleEvent: List of sample_variables: []
2025-03-14 20:59:35,721 INFO o.a.j.e.u.CompoundVariable: Note: Function class names must contain the string: '.functions.'
2025-03-14 20:59:35,721 INFO o.a.j.e.u.CompoundVariable: Note: Function class names must not contain the string: '.gui.'
2025-03-14 20:59:35,779 INFO o.a.j.JMeter: Running test (1741960775779)
2025-03-14 20:59:35,796 INFO o.a.j.e.StandardJMeterEngine: Starting ThreadGroup: 1 : Thread Group
2025-03-14 20:59:35,796 INFO o.a.j.e.StandardJMeterEngine: Starting 10 threads for group Thread Group.
2025-03-14 20:59:35,796 INFO o.a.j.e.StandardJMeterEngine: Thread will continue on error
2025-03-14 20:59:35,796 INFO o.a.j.t.ThreadGroup: Starting thread group... number=1 threads=10 ramp-up=1 delayedStart=false
2025-03-14 20:59:35,801 INFO o.a.j.t.ThreadGroup: Started thread group number 1
2025-03-14 20:59:35,801 INFO o.a.j.e.StandardJMeterEngine: Starting ThreadGroup: 2 : Thread Group
2025-03-14 20:59:35,801 INFO o.a.j.e.StandardJMeterEngine: Starting 10 threads for group Thread Group.
2025-03-14 20:59:35,801 INFO o.a.j.e.StandardJMeterEngine: Thread will continue on error
2025-03-14 20:59:35,801 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-1
2025-03-14 20:59:35,801 INFO o.a.j.t.ThreadGroup: Starting thread group... number=2 threads=10 ramp-up=1 delayedStart=false
2025-03-14 20:59:35,802 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-1
2025-03-14 20:59:35,803 INFO o.a.j.t.ThreadGroup: Started thread group number 2
2025-03-14 20:59:35,803 INFO o.a.j.e.StandardJMeterEngine: Starting ThreadGroup: 3 : Thread Group
2025-03-14 20:59:35,803 INFO o.a.j.e.StandardJMeterEngine: Starting 10 threads for group Thread Group.
2025-03-14 20:59:35,804 INFO o.a.j.e.StandardJMeterEngine: Thread will continue on error
2025-03-14 20:59:35,804 INFO o.a.j.t.ThreadGroup: Starting thread group... number=3 threads=10 ramp-up=1 delayedStart=false
2025-03-14 20:59:35,804 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-1
2025-03-14 20:59:35,805 INFO o.a.j.t.ThreadGroup: Started thread group number 3
2025-03-14 20:59:35,805 INFO o.a.j.e.StandardJMeterEngine: All thread groups have been started
2025-03-14 20:59:35,813 INFO o.a.j.p.h.s.HTTPHCAbstractImpl: Local host = LAPTOP-IDSJA4PC
2025-03-14 20:59:35,817 INFO o.a.j.p.h.s.HTTPHC4Impl: HTTP request retry count = 0
2025-03-14 20:59:35,818 INFO o.a.j.s.SampleResult: Note: Sample TimeStamps are START times
2025-03-14 20:59:35,818 INFO o.a.j.s.SampleResult: sampleresult.default.encoding is set to UTF-8
2025-03-14 20:59:35,818 INFO o.a.j.s.SampleResult: sampleresult.useNanoTime=true
2025-03-14 20:59:35,818 INFO o.a.j.s.SampleResult: sampleresult.nanoThreadSleep=5000
2025-03-14 20:59:35,898 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-2
2025-03-14 20:59:35,903 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-2
2025-03-14 20:59:35,906 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-2
2025-03-14 20:59:36,000 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-3
2025-03-14 20:59:36,003 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-3
2025-03-14 20:59:36,005 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-3
2025-03-14 20:59:36,099 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-4
2025-03-14 20:59:36,102 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-4
2025-03-14 20:59:36,105 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-4
2025-03-14 20:59:36,199 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-5
2025-03-14 20:59:36,202 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-5
2025-03-14 20:59:36,206 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-5
2025-03-14 20:59:36,297 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-6
2025-03-14 20:59:36,301 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-6
2025-03-14 20:59:36,304 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-6
2025-03-14 20:59:36,397 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-7
2025-03-14 20:59:36,401 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-7
2025-03-14 20:59:36,404 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-7
2025-03-14 20:59:36,498 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-8
2025-03-14 20:59:36,503 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-8
2025-03-14 20:59:36,505 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-8
2025-03-14 20:59:36,598 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-9
2025-03-14 20:59:36,603 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-9
2025-03-14 20:59:36,605 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-9
2025-03-14 20:59:36,618 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-3
2025-03-14 20:59:36,618 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-3
2025-03-14 20:59:36,705 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 1-10
2025-03-14 20:59:36,707 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 2-10
2025-03-14 20:59:36,708 INFO o.a.j.t.JMeterThread: Thread started: Thread Group 3-10
2025-03-14 20:59:37,238 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-1
2025-03-14 20:59:37,238 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-1
2025-03-14 20:59:37,295 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-2
2025-03-14 20:59:37,295 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-2
2025-03-14 20:59:38,804 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-4
2025-03-14 20:59:38,804 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-4
2025-03-14 20:59:40,346 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-5
2025-03-14 20:59:40,346 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-5
2025-03-14 20:59:58,072 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-2
2025-03-14 20:59:58,072 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-3
2025-03-14 20:59:58,072 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-2
2025-03-14 20:59:58,072 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-3
2025-03-14 20:59:58,220 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-1
2025-03-14 20:59:58,220 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-1
2025-03-14 20:59:58,784 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-4
2025-03-14 20:59:58,784 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-4
2025-03-14 20:59:59,212 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-6
2025-03-14 20:59:59,213 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-6
2025-03-14 20:59:59,582 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-5
2025-03-14 20:59:59,582 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-5
2025-03-14 20:59:59,664 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-7
2025-03-14 20:59:59,664 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-7
2025-03-14 21:00:03,408 INFO o.a.j.r.Summariser: summary +     13 in 00:00:28 =    0.5/s Avg: 15084 Min:   612 Max: 27102 Err:     0 (0.00%) Active: 18 Started: 30 Finished: 12
2025-03-14 21:00:03,409 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-6
2025-03-14 21:00:03,409 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-6
2025-03-14 21:00:03,739 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-8
2025-03-14 21:00:03,739 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-8
2025-03-14 21:00:04,470 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-7
2025-03-14 21:00:04,470 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-7
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-9
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-9
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-10
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-9
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-9
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-9
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-10
2025-03-14 21:00:06,902 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-9
2025-03-14 21:00:07,064 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 3-10
2025-03-14 21:00:07,064 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 3-10
2025-03-14 21:00:07,266 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-10
2025-03-14 21:00:07,266 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-10
2025-03-14 21:00:07,653 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 2-8
2025-03-14 21:00:07,654 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 2-8
2025-03-14 21:01:12,396 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-2
2025-03-14 21:01:12,397 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-2
2025-03-14 21:01:12,399 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-1
2025-03-14 21:01:12,400 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-1
2025-03-14 21:01:13,004 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-4
2025-03-14 21:01:13,004 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-4
2025-03-14 21:01:14,126 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-3
2025-03-14 21:01:14,126 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-3
2025-03-14 21:01:23,263 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-5
2025-03-14 21:01:23,263 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-5
2025-03-14 21:01:23,579 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-6
2025-03-14 21:01:23,579 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-6
2025-03-14 21:01:24,368 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-7
2025-03-14 21:01:24,368 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-7
2025-03-14 21:01:26,243 INFO o.a.j.t.JMeterThread: Thread is done: Thread Group 1-8
2025-03-14 21:01:26,243 INFO o.a.j.t.JMeterThread: Thread finished: Thread Group 1-8
2025-03-14 21:01:26,244 INFO o.a.j.e.StandardJMeterEngine: Notifying test listeners of end of test
2025-03-14 21:01:26,244 INFO o.a.j.r.Summariser: summary +     17 in 00:01:23 =    0.2/s Avg: 64033 Min: 27232 Max: 109744 Err:     6 (35.29%) Active: 0 Started: 30 Finished: 30
2025-03-14 21:01:26,245 INFO o.a.j.r.Summariser: summary =     30 in 00:01:50 =    0.3/s Avg: 42822 Min:   612 Max: 109744 Err:     6 (20.00%)

timeStamp,elapsed,label,responseCode,responseMessage,threadName,dataType,success,failureMessage,bytes,sentBytes,grpThreads,allThreads,URL,Latency,IdleTime,Connect
1741960776005,612,HTTP Request,200,,Thread Group 3-3,text,true,,269,127,9,27,http://localhost:8080/highest-gpa,608,0,1
1741960775878,1359,HTTP Request,200,,Thread Group 3-1,text,true,,269,127,9,29,http://localhost:8080/highest-gpa,1359,0,19
1741960775907,1388,HTTP Request,200,,Thread Group 3-2,text,true,,269,127,8,28,http://localhost:8080/highest-gpa,1388,0,0
1741960776105,2699,HTTP Request,200,,Thread Group 3-4,text,true,,269,127,7,27,http://localhost:8080/highest-gpa,2699,0,1
1741960776206,4139,HTTP Request,200,,Thread Group 3-5,text,true,,269,127,6,26,http://localhost:8080/highest-gpa,4139,0,1
1741960776003,22069,HTTP Request,200,,Thread Group 2-3,text,true,,936982,132,10,25,http://localhost:8080/all-student-name,22065,0,1
1741960775904,22168,HTTP Request,200,,Thread Group 2-2,text,true,,936982,132,10,25,http://localhost:8080/all-student-name,22164,0,1
1741960775878,22341,HTTP Request,200,,Thread Group 2-1,text,true,,936982,132,8,23,http://localhost:8080/all-student-name,22337,0,19
1741960776102,22681,HTTP Request,200,,Thread Group 2-4,text,true,,936982,132,7,22,http://localhost:8080/all-student-name,22679,0,1
1741960776305,22907,HTTP Request,200,,Thread Group 3-6,text,true,,269,127,5,21,http://localhost:8080/highest-gpa,22907,0,0
1741960776202,23379,HTTP Request,200,,Thread Group 2-5,text,true,,936982,132,6,20,http://localhost:8080/all-student-name,23377,0,1
1741960776405,23259,HTTP Request,200,,Thread Group 3-7,text,true,,269,127,4,19,http://localhost:8080/highest-gpa,23259,0,0
1741960776302,27102,HTTP Request,200,,Thread Group 2-6,text,true,,936982,132,5,18,http://localhost:8080/all-student-name,27100,0,0
1741960776506,27232,HTTP Request,200,,Thread Group 3-8,text,true,,269,127,3,17,http://localhost:8080/highest-gpa,27232,0,0
1741960776402,28068,HTTP Request,200,,Thread Group 2-7,text,true,,936982,132,4,16,http://localhost:8080/all-student-name,28066,0,1
1741960776707,30195,HTTP Request,500,,Thread Group 1-10,text,false,,256,127,10,15,http://localhost:8080/all-student,30194,0,1
1741960776598,30304,HTTP Request,500,,Thread Group 1-9,text,false,,256,127,10,15,http://localhost:8080/all-student,30303,0,1
1741960776605,30297,HTTP Request,500,,Thread Group 3-9,text,false,,256,127,2,15,http://localhost:8080/highest-gpa,30296,0,1
1741960776603,30299,HTTP Request,500,,Thread Group 2-9,text,false,,261,132,3,15,http://localhost:8080/all-student-name,30298,0,1
1741960776708,30355,HTTP Request,500,,Thread Group 3-10,text,false,,256,127,1,11,http://localhost:8080/highest-gpa,30355,0,1
1741960776707,30559,HTTP Request,500,,Thread Group 2-10,text,false,,261,132,2,10,http://localhost:8080/all-student-name,30558,0,1
1741960776504,31149,HTTP Request,200,,Thread Group 2-8,text,true,,936982,132,1,9,http://localhost:8080/all-student-name,31146,0,0
1741960775899,96497,HTTP Request,200,,Thread Group 1-2,text,true,,1428528,127,8,8,http://localhost:8080/all-student,96493,0,0
1741960775878,96521,HTTP Request,200,,Thread Group 1-1,text,true,,1428332,127,7,7,http://localhost:8080/all-student,96516,0,19
1741960776100,96904,HTTP Request,200,,Thread Group 1-4,text,true,,1429048,127,6,6,http://localhost:8080/all-student,96901,0,0
1741960776001,98125,HTTP Request,200,,Thread Group 1-3,text,true,,1428851,127,5,5,http://localhost:8080/all-student,98122,0,0
1741960776199,107064,HTTP Request,200,,Thread Group 1-5,text,true,,1437681,127,4,4,http://localhost:8080/all-student,107061,0,1
1741960776298,107281,HTTP Request,200,,Thread Group 1-6,text,true,,1437744,127,3,3,http://localhost:8080/all-student,107278,0,1
1741960776398,107970,HTTP Request,200,,Thread Group 1-7,text,true,,1438287,127,2,2,http://localhost:8080/all-student,107967,0,1
1741960776499,109744,HTTP Request,200,,Thread Group 1-8,text,true,,1440106,127,1,1,http://localhost:8080/all-student,109742,0,0
