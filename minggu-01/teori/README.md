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
ketika perintah di baca dari tty, interpreter akan di buat menjadi mode interaktif, pada mode ini primary prompt untuk perintah biasanya diberi tanda >>> atau biasa di sebut REPL dan untuk prompt selanjutnya atau secondary prompt akan di beri tanda ...

__Interpreter dan Environment nya__<br>
secara default source files dari Python di perlakukan seperti sedang encode di UTF-8

## Bab 3 Pengenalan Python
input dan ouput dapat di bedakan dengan adanya (>>> dan ...). comment dapat di lakukan dengan memberi tanda pagar #
### Menggunakan Python Sebagai Kalkulator
__Numbers__<br>
interpreter pada Python dapat di gunakan sebagai kalkulator sederhana yang menggunakan perintah + (penjumlahan), - (pengurangan), * (perkalian), dan / (pembagian), sama seperti bahasa pemrograman lainnya

integer atau bilangan bulat dapat menggunakan perintah int, sedangkan pecahan dapat menggunakan perintah float

pembagian menggunakan / selalu menghasilkan bilangan pecahan (tipe data float), dan untuk menampilkan bilangan bulat (tipe data integer) dapat menggunakan perintah //, kemudian untuk menampilkan hasil sisa bagi dapat menggunakan perintah %

Python juga dapat membuat kelipatan dengan menggunakan perintah **

perintah = digunakan untuk memasukan value ke dalam variabel dan jika tidak di berikan maka akan menampilkan output name '...' is not defined

ketika bilangan bilangan bulat dan pecahan di gabungkan, maka akan menghasilkan output pecahan, contohnya 4 * 3.75 - 1 , maka akan menghasilkan 14.0

pada mode interaktif expression terakhir yang di print atau output akan di masukan ke dalam variabel _ sehingga ketika ingin memanggil ulang hasil output dari perhitungan sebelumnya cukup dengan menggunakan varibel _ tanpa perlu di deklarasi terlebih dahulu

__Strings__<br>
selain angka, Python juga bisa memanipulasi strings, yang bisa di ekspresikan dengan beberapa cara, bisa menggunakan single quotes ('...') atau double quotes("..."), selain itu bisa menggunakan \ untuk melewati quotes sebelumnya

pada interpreter interaktif, ouput string di tutup dengan quotes atau tanda petik dan karakter spesial dapat di lewati dengan backslashes \ . jika ingin tanda \ tidak dibaca sebagai karakter spesial maka dapat menggunakan r untuk menampilkan raw strings

penulisan string dapat di span menjadi beberapa baris, salah satunya menggunakan triple-quotes: """...""" atau '''...'''

string juga dapat di gabungkan menggunakan tanda + ,serta dapat di ulang menggunakan tanda *

ketika 2 string yang terpisah dan diselubungi oleh quotes atau tanda petik maka kedua string tersebut akan digabungkan, tetapi hanya dapat digunakan oleh literal dan tidak dapat di gunakan pada variabel ataupun expresi, namun jika ingin menggabungkan variabel dengan literal maka dapat menggunakan +

strings juga dapat di indexed atau di pecah ketika hanya ingin menampilkan sebagian dari total string yang ada menggunakan [...], contohnya kata = 'Python', maka ketika ingin memanggil huruf 'P' saja, bisa dengan menuliskan kata[0] (dimulai dari 0), dengan total huruf yang ada yaitu 6 dan huruf 'P' berada di urutan 0 atau paling awal, begitupun ketika ingin menampilkan huruf 'n', maka bisa dengan menuliskan kata[5] (dimulai dari 0), karena huruf 'n' berada di paling akhir

string juga dapat di potong menjadi beberapa kata atau huruf menggunakan [... : ...], contohnya ketika ingin menampilkan kata 'Py' pada 'Python' maka bisa dengan menuliskan kata[0:2], begitu juga ketika ingin menampilkan kata 'tho' maka bisa dengan menuliskan kata[2:5]

string yang sebelumnya telah di potong juga dapat di satukan kembali menggunakan +

string tidak dapat di pecah atau di potong ketika jumlah urutan atau penulisannya melebihi total huruf dari kata yang ada, contohnya kata[42] maka outputnya akan error dikarenakan total huruf dari 'Python' hanya 6 yaitu 0 sampai 5

string pada Python tidak bisa di rubah karena tipe immutable dan jika ingin membuat string yang berbeda maka bisa menggunakan +

total string atau huruf dapat di hitung menggunakan perintah len(...)

__List__<br>
Python juga mengenal nomor tipe data gabungan atau list. ataupun biasa disebut dengan array

sama seperti strings list dapat di pecah atau di potong dengan hanya memanggil nomor indexnya

list juga dapat digabungkan dengan perintah +

berbeda dengan strings, list merupakan tipe mutable atau bisa di rubah

size pada list dapat dirubah jumlah valuenya, baik di tambahkan di kurangi atau bahkan di hilangkan

fungsi len(...) juga dapat digunakan pada list

list dapat dibuat menjadi nested atau list yang berada di dalam list
