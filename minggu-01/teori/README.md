# Ringkasan Minggu Ke-1
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___
## Bab 1 Apa Itu Python
Python merupakan bahasa pemrograman yang lebih simpel digunakan di bandingkan C, C++, ataupun Java

Python merupakan bahasa interpreted yang mana lebih cepat di jalankan karena Python tidak melakukan kompilasi terlebih dahulu
 
Python mempunyai struktur dan support untuk berbagai masalah jauh lebih banyak di bandingkan shell scripts atau batch files, selain itu juga Python menawarkan error checking yang lebih banyak di bandingkan C
 
Python merupakan very-high-level language atau bahasa tingkat tinggi, yang mana di Python sendiri terdapat data tingkat tinggi seperti arrays yang lebih fleksibel dan dictionaries yang lebih baik
 
Python banyak digunakan untuk mengelolah data
 
Python mempunyai struktur penulisan yang lebih compact dan mudah di pahami di bandingkan bahasa pemrograman C, C++, ataupun Java, contohnya tipe data tingkat tinggi yang kompleks dapat di buat dalam satu statement ketika menggunakan Python, kemudian pengelompokkan statement dapat dilakukan tanpa menggunakan brackets, serta tidak wajib mendeklarasikan variable atau argument terlebih dahulu
 
nama Python di ambil dari acara "Monty Python's Flying Circus" dan tidak ada hubungannya dengan reptil

## Bab 2 Interpreter Pada Python
Python versi terbaru yaitu versi 3.11, dan dapat di download di Microsoft Store untuk pengguna windows, secara default interpreter Python terinstall di dalam /usr/local/bin/python3.11 namun dapat di sesuaikan berdasarkan keinginan user

untuk mengeluarkan interpreter Python dari prompt dapat menekan key CTRL+Z atau mengetikan quit()

line-editing pada interpreter Python mempunyai beberapa fitur, seperti interactive editing, history substitution, dan code completion pada system yang mendukung GNU Readline

interpreter Python berkerja agak mirip seperti Unix shell: ketika dipanggil dengan input standar yang terkoneksi ke device maka ia akan membaca serta mengeksekusi secara interaktif dan ketika di panggil dengan argumen nama file atau file sebagai standar input maka ia akan membaca dan mengeksekusi script dari file tersebut

__Argument Passing__<br>
ketika dapat dibaca atau diketahui oleh interpreter, nama script dan argument tambahan kemudian dirubah menjadi list atau daftar strings, dan dimasukkan ke dalam variabel argv di dalam sys module, dan dapat di akses dengan mengeksekusi import sys. panjang atau isi dari list setidaknya harus satu; ketika tidak terdapat script atau argumen yang diberikan, sys.argv[0] menjadi empty string atau kosong. ketika nama script diberikan sebagai '-' (maksudnya adalah standar input), sys.argv[0] akan diset menjadi '-'. ketika command -c digunakan, sys.argv[0] akan diset menjadi '-c'. ketika -m module digunakan, sys.argv[0] akan diset menjadi full name dari lokasi modul.

__Interactive Mode__<br>
ketika 
