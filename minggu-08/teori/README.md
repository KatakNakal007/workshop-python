# Ringkasan Minggu Ke-7
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

# 10. Brief Tour of the Standard Library <br>

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

# 11. Brief Tour of the Standard Library — Part II <br>

## 11.1. Output Formatting <br>
Bagian 11.1 dari tutorial modul standar library Python membahas pemformatan output. Modul "string" dan "reprlib" digunakan untuk mengontrol format tampilan objek dan teks yang dihasilkan.

Modul "string" menyediakan berbagai metode untuk memanipulasi dan memformat string, seperti "string.format()" untuk menggabungkan nilai ke dalam string format, dan "string.Template()" untuk penggantian string berbasis placeholder.

Modul "reprlib" digunakan untuk menghasilkan representasi terbatas dari objek kompleks, yang berguna untuk menghindari keluaran yang terlalu panjang atau berulang.

Dengan menggunakan modul-modul ini, kita dapat mengontrol format tampilan output dan memformat string sesuai dengan kebutuhan. Ini berguna dalam penampilan data yang terstruktur, pembuatan pesan, atau keperluan format khusus lainnya dalam program Python.

## 11.2. Templating <br>
Bagian 11.2 dari tutorial modul standar library Python membahas templating. Modul "string" dan "template" digunakan untuk membuat dan mengelola templat string.

Dalam bagian ini, modul "string" menyediakan metode-metode untuk memanipulasi dan memformat string, sedangkan modul "template" menyediakan kelas "Template" yang memungkinkan pembuatan templat string dengan placeholder yang dapat digantikan.

Dengan menggunakan modul "template", kita dapat membuat template string yang mengandung placeholder yang akan diisi dengan nilai yang ditentukan. Kemudian, Anda dapat menggantikan placeholder tersebut dengan nilai nyata untuk menghasilkan output yang diinginkan.

Pemanfaatan templating memudahkan pembuatan teks yang dinamis, seperti pembuatan pesan atau email, penghasilan kode, atau pembuatan dokumen yang terstruktur.

Dengan menggunakan modul-modul ini, Anda dapat membuat dan mengelola template string dengan mudah, sehingga memungkinkan fleksibilitas dalam pembuatan dan pemformatan teks dalam program Python.

## 11.3. Working with Binary Data Record Layouts <br>
Bagian 11.3 dari tutorial modul standar library Python membahas bekerja dengan format data biner dan layout catatan (record layout). Modul "struct" digunakan untuk membaca, menulis, dan memanipulasi data dalam format biner.

Dalam bagian ini, modul "struct" menyediakan fungsi-fungsi untuk mengonversi data antara representasi biner dan representasi Python yang dapat dioperasikan. kita dapat mengatur format data biner dengan menggunakan spesifikasi format yang ditentukan oleh modul "struct".

Dengan menggunakan modul "struct", kita dapat membaca data dari file biner, memanipulasi data biner, dan menulis data ke file biner sesuai dengan format yang ditentukan.

Modul "struct" sangat berguna dalam memproses data biner yang terstruktur, seperti file biner, protokol jaringan, atau format data yang dihasilkan oleh perangkat keras.

Dengan menggunakan modul ini, kita dapat bekerja dengan data biner secara efisien dan akurat dalam program Python.

## 11.4. Multi-threading <br>
Bagian 11.4 dari tutorial modul standar library Python membahas multi-threading. Modul "threading" digunakan untuk membuat dan mengelola thread dalam program Python.

Dalam bagian ini, modul "threading" menyediakan kelas "Thread" yang memungkinkan pembuatan dan pengelolaan thread. kita dapat membuat thread baru, mengontrol eksekusi paralel, dan berkomunikasi antar thread menggunakan objek "Lock" atau "Condition".

Dengan menggunakan multi-threading, kita dapat menjalankan tugas-tugas secara paralel untuk meningkatkan kinerja dan responsivitas program. Ini sangat berguna dalam situasi di mana tugas-tugas dapat dilakukan secara independen atau saat program perlu merespons input atau kejadian secara real-time.

Namun, perlu diingat bahwa penggunaan multi-threading membutuhkan pemikiran dan pengelolaan yang hati-hati untuk menghindari masalah seperti race condition atau deadlock.

Dengan modul "threading", kita dapat mengimplementasikan multi-threading dengan lebih mudah dalam program Python dan memanfaatkannya untuk meningkatkan kinerja dan responsivitas program Anda.

## 11.5. Logging <br>
Bagian 11.5 dari tutorial modul standar library Python membahas logging. Modul "logging" digunakan untuk mencatat pesan dan kejadian dalam program Python.

Dalam bagian ini, modul "logging" menyediakan kelas "Logger" yang memungkinkan pencatatan pesan dengan tingkat prioritas yang berbeda. kita dapat mengonfigurasi logger untuk menentukan output log, tingkat log, dan format pesan.

Dengan menggunakan logging, kita dapat mencatat informasi penting, kesalahan, atau kejadian di dalam program. Ini membantu dalam pemantauan, pemecahan masalah, dan analisis program.

Modul "logging" memiliki fleksibilitas yang tinggi dan dapat diatur sesuai dengan kebutuhan yang di butuhkan. kita dapat mengarahkan output log ke berbagai target, seperti file, konsol, atau sistem log eksternal.

Dengan menggunakan modul ini, kita dapat dengan mudah mengimplementasikan sistem pencatatan yang kuat dan terstruktur dalam program Python.

## 11.6. Weak References <br>
Bagian 11.6 dari tutorial modul standar library Python membahas weak references. Modul "weakref" digunakan untuk membuat referensi yang lemah (weak references) terhadap objek.

Dalam bagian ini, modul "weakref" menyediakan kelas "WeakRef" yang memungkinkan kita membuat referensi yang tidak mempengaruhi siklus referensi dan tidak mencegah penghapusan objek.

Dengan menggunakan weak references, kita dapat membuat referensi yang fleksibel dan tidak permanen terhadap objek. Ini berguna dalam skenario di mana kita ingin melakukan tindakan terhadap objek yang tidak mencegah objek tersebut dihapus oleh pengumpul sampah (garbage collector).

Modul "weakref" memungkinkan kita untuk mengikuti referensi terhadap objek yang terhapus secara otomatis dan mengatasi masalah dengan siklus referensi yang dapat menghambat penghapusan objek.

Dengan menggunakan modul ini, kita dapat mengimplementasikan strategi pengelolaan objek yang lebih efisien dan menghindari masalah yang terkait dengan siklus referensi dalam program Python.

## 11.7. Tools for Working with Lists <br>
Bagian 11.7 dari tutorial modul standar library Python membahas alat-alat untuk bekerja dengan daftar (lists). Modul "array" dan "collections" digunakan untuk operasi yang efisien pada elemen-elemen dalam daftar.

Dalam bagian ini, modul "array" menyediakan kelas "array" yang memungkinkan kita menyimpan dan memanipulasi data dalam bentuk array yang diketahui tipe datanya. Hal ini dapat menghemat ruang dan meningkatkan kinerja saat bekerja dengan data numerik.

Modul "collections" menyediakan kelas-kelas seperti "deque" (antrian ganda) dan "Counter" yang menyediakan fitur-fitur tambahan untuk memanipulasi daftar. Misalnya, "deque" memungkinkan operasi penghapusan dan penambahan elemen di kedua ujung antrian dengan kinerja yang baik.

Dengan menggunakan modul-modul ini, kita dapat memperluas fungsionalitas daftar dengan alat-alat yang lebih efisien dan khusus, tergantung pada kebutuhan program yang di inginkan.

Modul "array" dan "collections" memberikan fleksibilitas dan kinerja yang lebih baik dalam memanipulasi dan mengelola daftar dalam program Python.

## 11.8. Decimal Floating Point Arithmetic <br>
Bagian 11.8 dari tutorial modul standar library Python membahas aritmetika titik desimal (decimal floating point). Modul "decimal" digunakan untuk melakukan operasi matematika yang akurat dengan bilangan desimal.

Dalam bagian ini, modul "decimal" menyediakan kelas "Decimal" yang memungkinkan penghitungan dengan presisi yang tinggi dan pengendalian yang lebih baik terhadap pembulatan dan presisi desimal.

Dengan menggunakan modul "decimal", kita dapat menghindari kesalahan pembulatan yang umum terkait dengan aritmatika floating point biasa. Ini sangat penting dalam kasus-kasus di mana presisi yang tepat atau penanganan desimal yang benar sangat penting, seperti dalam keuangan atau perhitungan ilmiah.

Modul "decimal" memungkinkan kita untuk mengatur jumlah digit desimal yang diinginkan, mengendalikan pembulatan, dan menangani angka desimal dengan akurasi tinggi.
