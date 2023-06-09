# Ringkasan Minggu Ke-7
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

## 10.1. Operating System Interface <br>

Bagian 10.1 dari tutorial modul standar library Python membahas antarmuka sistem operasi (Operating System Interface). Bagian ini memberikan kemampuan untuk berinteraksi dengan sistem operasi melalui modul "os". Fungsi-fungsi yang dibahas dalam bagian ini meliputi:

- Membuat direktori baru menggunakan fungsi "os.mkdir(path)".
- Menghapus direktori kosong menggunakan fungsi "os.rmdir(path)".
- Menghapus file menggunakan fungsi "os.remove(path)".
- Mengubah nama file atau direktori menggunakan fungsi "os.rename(src, dst)".
- Modul "os.path" menyediakan fungsi-fungsi untuk operasi pada jalur file dan direktori, seperti menggabungkan jalur, membagi jalur, dan menguji keberadaan jalur.

## 10.2. File Wildcards <br>
Bagian 10.2 dari tutorial modul standar library Python membahas penggunaan wildcard pada nama file (File Wildcards)

## 10.3. Command Line Arguments <br>
Bagian 10.3 dari tutorial modul standar library Python membahas penggunaan argumen baris perintah (Command Line Arguments). Modul "sys" digunakan untuk mengakses argumen baris perintah dalam program Python melalui "sys.argv". Ini memungkinkan program untuk menerima input dinamis saat dijalankan melalui baris perintah atau terminal, memberikan fleksibilitas yang lebih besar. Argumen baris perintah dapat digunakan untuk mengubah perilaku program atau melakukan operasi berdasarkan argumen yang diberikan.

## 10.4. Error Output Redirection and Program Termination <br>
Bagian 10.4 dari tutorial modul standar library Python membahas pengalihan output error dan terminasi program. Modul "sys" digunakan untuk mengakses aliran output error ("sys.stderr") dan menghentikan program secara paksa ("sys.exit()"). Ini memungkinkan kita untuk mengontrol output error dan menghentikan program dengan cara yang terkendali.

## 10.5. String Pattern Matching <br>
Bagian 10.5 dari tutorial modul standar library Python membahas pencocokan pola string (String Pattern Matching). Modul "re" digunakan untuk bekerja dengan ekspresi reguler (regular expressions) dalam Python. Ekspresi reguler adalah pola yang digunakan untuk mencocokkan dan memanipulasi string. Dengan modul "re", Anda dapat mencocokkan pola, mencari, mengganti, dan memanipulasi string berdasarkan pola yang ditentukan. Ini sangat berguna dalam memproses teks yang kompleks dan memanipulasi string dengan kriteria tertentu.

## 10.6. Mathematics <br>
Bagian 10.6 dari tutorial modul standar library Python membahas modul "math" yang menyediakan fungsi matematika untuk operasi matematika yang kompleks. Dengan menggunakan modul "math", Anda dapat melakukan perhitungan trigonometri, logaritma, eksponensial, akar kuadrat, dan lainnya. Modul ini sangat berguna dalam pengolahan data numerik dan analisis matematika.

## 10.7. Internet Access <br>
Bagian 10.7 dari tutorial modul standar library Python membahas akses internet menggunakan modul "urllib". Modul ini memungkinkan kita untuk mengambil konten dari URL, berinteraksi dengan API, dan melakukan operasi akses internet lainnya. Ini sangat berguna dalam pengembangan web scraping, pengambilan data, dan komunikasi dengan sumber daya online dalam program Python.

## 10.8. Dates and Times <br>
Bagian 10.8 dari tutorial modul standar library Python membahas tanggal dan waktu menggunakan modul "datetime". Modul ini memungkinkan manipulasi dan operasi pada tanggal, waktu, dan durasi. yang dapat membuat objek untuk merepresentasikan tanggal dan waktu, melakukan operasi aritmatika dengan "timedelta", dan mengubah format tampilan. Modul "datetime" sangat berguna dalam pengelolaan waktu, penjadwalan, dan manipulasi data tanggal dan waktu dalam program Python.

## 10.9. Data Compression <br>
Bagian 10.9 dari tutorial modul standar library Python membahas kompresi data menggunakan modul "zlib" dan "gzip". Modul ini memungkinkan kompresi dan dekompresi data menggunakan algoritma zlib dan format gzip. Dengan menggunakan modul-modul ini, kita dapat mengurangi ukuran file atau payload yang dikirimkan melalui jaringan. Modul ini sangat berguna dalam pengarsipan file, komunikasi jaringan, dan manajemen data yang efisien.

## 10.10. Performance Measurement <br>
Bagian 10.10 dari tutorial modul standar library Python membahas pengukuran kinerja (performance measurement) menggunakan modul "timeit". Modul ini memungkinkan kita untuk mengukur waktu eksekusi kode Python dengan presisi tinggi. Dengan menggunakan "timeit.timeit()", kita dapat membandingkan kinerja kode, mengidentifikasi bagian yang memakan waktu eksekusi lama, dan memperbaiki efisiensi program. Modul "timeit" memberikan alat yang kuat untuk melakukan pengukuran kinerja dalam program Python.

## 10.11. Quality Control <br>
Bagian 10.11 dari tutorial modul standar library Python membahas kontrol kualitas kode. Modul "doctest" digunakan untuk pengujian dan verifikasi dokumentasi kode, sedangkan modul "unittest" menyediakan kerangka kerja pengujian unit. Terdapat juga tools eksternal seperti "pylint" dan "flake8" yang membantu menganalisis dan meningkatkan kualitas kode Python. Dengan menggunakan modul dan alat ini, kita dapat memastikan kualitas kode dengan melakukan pengujian, verifikasi dokumentasi, dan penerapan praktik yang baik dalam penulisan kode.

## 11.1. Output Formatting <br>
Bagian 11.1 dari tutorial modul standar library Python membahas pemformatan output. Modul "string" dan "reprlib" digunakan untuk mengontrol format tampilan objek dan teks yang dihasilkan.

Modul "string" menyediakan berbagai metode untuk memanipulasi dan memformat string, seperti "string.format()" untuk menggabungkan nilai ke dalam string format, dan "string.Template()" untuk penggantian string berbasis placeholder.

Modul "reprlib" digunakan untuk menghasilkan representasi terbatas dari objek kompleks, yang berguna untuk menghindari keluaran yang terlalu panjang atau berulang.

Dengan menggunakan modul-modul ini, kita dapat mengontrol format tampilan output dan memformat string sesuai dengan kebutuhan. Ini berguna dalam penampilan data yang terstruktur, pembuatan pesan, atau keperluan format khusus lainnya dalam program Python.

## 11.2. Templating <br>
