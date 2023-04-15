# Ringkasan Minggu Ke-5
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

## 7.1. Fancier Output Formatting <br>
membahas tentang teknik-teknik format output yang lebih canggih menggunakan string format pada Python. Tutorial ini memperkenalkan cara untuk menampilkan nilai variabel atau ekspresi dalam sebuah string menggunakan karakter % sebagai operator format. Selain itu, tutorial juga membahas tentang penggunaan fungsi str.format() sebagai alternatif yang lebih modern dan fleksibel. Tutorial juga mencakup penggunaan format string literals yang memungkinkan programmer menentukan nilai variabel dalam sebuah string dengan mudah. Selain itu, tutorial juga membahas beberapa konsep dan contoh praktis dalam menggabungkan format output dengan tipe data seperti list, dictionary, dan tuple

### 7.1.1. Formatted String Literals <br>
menggunakan formatted string literals. Formatted string literals adalah string yang diberi awalan karakter f atau F dan memungkinkan programmer menentukan nilai variabel dalam string dengan mudah menggunakan sintaks {variabel}. Tutorial ini memberikan contoh penggunaan formatted string literals untuk menampilkan nilai variabel dan ekspresi dalam sebuah string dengan cara yang lebih mudah dibaca. Selain itu, tutorial juga memberikan contoh praktis penggunaan formatted string literals untuk menggabungkan tipe data seperti list, dictionary, dan tuple dengan string.

### 7.1.2. The String format() Method <br>
format output menggunakan metode str.format(). Metode ini memungkinkan programmer untuk menampilkan nilai variabel atau ekspresi dalam sebuah string dengan cara yang lebih fleksibel dan modern. Tutorial ini memberikan contoh penggunaan metode str.format() untuk menampilkan nilai variabel dan ekspresi dalam sebuah string dengan sintaks {}. Selain itu, tutorial juga memberikan contoh praktis penggunaan metode str.format() untuk menggabungkan tipe data seperti list, dictionary, dan tuple dengan string. Tutorial ini juga membahas tentang penggunaan argumen dalam metode str.format(), seperti mengatur lebar kolom, presisi, dan rata kanan atau kiri.

### 7.1.3. Manual String Formatting <br>
teknik format output menggunakan metode manual. Metode ini menggabungkan string dan variabel secara manual menggunakan operator + atau metode join(). Tutorial ini memberikan contoh penggunaan metode manual untuk menampilkan nilai variabel dan ekspresi dalam sebuah string dengan cara yang sederhana. Selain itu, tutorial juga membahas tentang kelemahan metode manual dan memberikan saran penggunaan teknik format output yang lebih modern seperti formatted string literals atau metode str.format(). Tutorial ini juga membahas tentang penggunaan karakter escape \ dan konstanta string seperti str.ljust(), str.rjust(), dan str.center() untuk mengatur lebar kolom dan rata kanan atau kiri dalam sebuah string.

### 7.1.4. Old string formatting <br>
teknik format output lama menggunakan operator %. Teknik ini kurang direkomendasikan karena keterbatasannya dalam pengaturan lebar kolom, presisi, dan rata kanan atau kiri dalam sebuah string.

## 7.2. Reading and Writing Files <br>
membahas tentang bagaimana membaca dan menulis file menggunakan bahasa pemrograman Python. Tutorial ini membahas cara membuka file dengan fungsi open(), mode pembukaan file, membaca isi file dengan metode read(), menulis isi file dengan metode write(), menutup file dengan metode close(), dan penggunaan blok with untuk membuka dan menutup file secara otomatis. Tutorial ini juga membahas teknik-teknik tambahan seperti membaca dan menulis file dalam mode binary, membaca file baris per baris, mengubah posisi pointer file dengan metode seek(), dan menghapus file dengan modul os.

### 7.2.1. Methods of File Objects <br>
membahas metode-metode yang dapat digunakan untuk membaca, menulis, dan memanipulasi file dengan bahasa pemrograman Python. Berikut ini adalah penjelasan singkat dari beberapa metode yang dibahas dalam bagian ini:
+ read(size): Metode ini digunakan untuk membaca isi file dalam bentuk string. Parameter size adalah jumlah byte yang akan dibaca, jika tidak diisi maka akan membaca semua isi file.
+ readline(): Metode ini digunakan untuk membaca satu baris dalam file, dimulai dari posisi pointer saat ini hingga karakter newline (\n).
+ readlines(): Metode ini digunakan untuk membaca semua baris dalam file dan mengembalikan list yang berisi setiap baris sebagai elemen list.
+ write(string): Metode ini digunakan untuk menulis string ke dalam file.
+ writelines(seq): Metode ini digunakan untuk menulis urutan string ke dalam file. Parameter seq harus berupa iterable yang berisi string.
+ seek(offset): Metode ini digunakan untuk mengatur posisi pointer file. Parameter offset menunjukkan jumlah byte dari awal file.
+ tell(): Metode ini digunakan untuk mengembalikan posisi pointer saat ini dalam file.
+ close(): Metode ini digunakan untuk menutup file yang sudah dibuka.
+ closed: Atribut ini digunakan untuk mengetahui apakah file sudah ditutup atau belum.

### 7.2.2. Saving structured data with json <br>
membahas cara menggunakan modul json untuk menyimpan dan membaca data terstruktur dalam format JSON.Berikut ini adalah penjelasan singkat dari beberapa metode yang dibahas dalam bagian ini:
+ dump(obj, fp, skipkeys=False, ensure_ascii=True, check_circular=True, allow_nan=True, cls=None, indent=None, separators=None, default=None, sort_keys=False, kw): Metode ini digunakan untuk menulis data terstruktur ke dalam file dalam format JSON. Parameter obj adalah data terstruktur yang akan disimpan, sedangkan fp adalah file object yang akan digunakan untuk menulis data.
+ dumps(obj, skipkeys=False, ensure_ascii=True, check_circular=True, allow_nan=True, cls=None, indent=None, separators=None, default=None, sort_keys=False, kw): Metode ini digunakan untuk mengonversi data terstruktur menjadi string dalam format JSON.
+ load(fp, cls=None, object_hook=None, parse_float=None, parse_int=None, parse_constant=None, object_pairs_hook=None, kw): Metode ini digunakan untuk membaca file yang berisi data dalam format JSON dan mengembalikan objek Python yang sesuai dengan data tersebut.
+ loads(s, cls=None, object_hook=None, parse_float=None, parse_int=None, parse_constant=None, object_pairs_hook=None, kw): Metode ini digunakan untuk mengonversi string dalam format JSON menjadi objek Python.

Tutorial ini juga membahas beberapa parameter yang dapat digunakan untuk mengatur format output JSON, seperti indent, separators, dan sort_keys. Selain itu, tutorial ini juga memberikan contoh penggunaan default dan object_hook, yang dapat digunakan untuk menangani kasus-kasus khusus saat menyimpan atau membaca data dalam format JSON.
