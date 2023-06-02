# Ringkasan Minggu Ke-7
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

# 9. Classes <br>
Bagian 9. Classes dalam tutorial Python 3 membahas tentang kelas (classes) dalam Python. Berikut adalah ringkasan yang lebih ringkas namun mudah dipahami:

1. Kelas adalah struktur dasar untuk membuat objek dalam Python.
2. Kelas memiliki atribut (variabel) dan metode (fungsi) yang terkait dengan objek.
3. Atribut adalah variabel dalam kelas yang menyimpan informasi tentang objek.
4. Metode adalah fungsi dalam kelas yang digunakan untuk memanipulasi atribut atau melakukan operasi lain pada objek.
5. Metode kelas adalah metode yang terikat dengan kelas itu sendiri, sedangkan metode statis adalah metode terkait dengan kelas secara umum.
6. Pewarisan memungkinkan kelas baru untuk menggunakan dan memperluas fungsionalitas kelas yang sudah ada.
7. Overriding memungkinkan kelas turunan untuk mengganti metode yang diwarisi dari kelas induk.
8. Multiple inheritance memungkinkan kelas untuk diturunkan dari beberapa kelas.
9. Polymorphism memungkinkan objek untuk memiliki banyak bentuk yang berbeda.

Dengan memahami konsep-konsep ini, kita dapat membuat struktur data yang lebih kompleks dan mengorganisir kode Python dengan lebih baik menggunakan kelas.

## 9.1. A Word About Names and Objects <br>
Bagian 9.1 "A Word About Names and Objects" dalam tutorial Python 3 menjelaskan tentang hubungan antara nama (variabel) dan objek dalam bahasa Python. 

Dalam Python, variabel merupakan nama yang digunakan untuk merujuk pada objek di dalam memori. Ketika kita membuat variabel, sebenarnya kita membuat referensi ke objek tersebut. Objek dalam Python dapat memiliki banyak nama yang merujuk pada mereka.

Perubahan nilai objek yang dilakukan melalui satu variabel akan mempengaruhi semua variabel lain yang merujuk pada objek yang sama. Ini disebabkan oleh fakta bahwa variabel tersebut hanya merupakan referensi ke objek yang sama di dalam memori.

Tipe objek dalam Python ditentukan secara dinamis berdasarkan nilai yang diberikan ke variabel. Tidak perlu mendeklarasikan tipe data secara eksplisit, karena tipe objek akan ditentukan otomatis sesuai dengan nilai yang diberikan.

Beberapa objek dalam Python bersifat tidak dapat diubah (immutable), seperti angka dan string. Ini berarti setelah objek immutable dibuat, nilainya tidak dapat diubah. Jika ada perubahan nilai, sebenarnya objek baru akan dibuat.

Memahami konsep referensi dan objek penting untuk menghindari kesalahan dalam manipulasi nilai objek dan juga untuk mengoptimalkan penggunaan variabel dan objek dalam program Python.

Dengan pemahaman tentang hubungan antara nama dan objek dalam Python, kita dapat lebih efektif dalam manipulasi nilai, pengelolaan variabel, dan penggunaan memori dalam program Python.

## 9.2. Python Scopes and Namespaces <br>
Bagian 9.2 "Python Scopes and Namespaces" dalam tutorial Python 3 membahas tentang cakupan (scope) dan ruang nama (namespace) dalam Python.

Cakupan mengacu pada bagian program di mana nama-nama didefinisikan dan dapat diakses. Python memiliki cakupan lokal untuk fungsi dan cakupan global untuk modul atau skrip.

Ruang nama adalah tempat di mana nama-nama unik disimpan untuk menghindari konflik. Setiap cakupan memiliki ruang nama terkait.

Python mencari nama di dalam cakupan lokal terlebih dahulu, kemudian di dalam cakupan global jika tidak ditemukan.

Ketika menggunakan variabel global di dalam fungsi, kita harus mendeklarasikan variabel tersebut sebagai global.

Ada juga cakupan nonlocal yang memungkinkan akses ke variabel di cakupan luar saat berada di dalam fungsi bersarang.

Cakupan dan ruang nama memainkan peran penting dalam mengatur visibilitas dan penggunaan nama-nama dalam program Python.

### 9.2.1. Scopes and Namespaces Example <br>
Bagian 9.2.1 "Scopes and Namespaces Example" dalam tutorial Python 3 memberikan contoh konkret yang mengilustrasikan konsep cakupan (scope) dan ruang nama (namespace) dalam Python.

Contoh tersebut terdiri dari dua fungsi: "outer_function" dan "inner_function". Setiap fungsi memiliki variabel "x" yang didefinisikan di dalam cakupan lokalnya. Ketika "inner_function" mencoba mengakses variabel "x", Python akan mencari nilainya terlebih dahulu di dalam cakupan lokal fungsi tersebut. Jika tidak ditemukan, Python akan mencari di dalam cakupan lokal fungsi yang mengelilingi. Jika tetap tidak ditemukan, Python akan mencari di dalam cakupan global.

Dalam contoh ini, karena variabel "x" tidak ditemukan di dalam cakupan lokal "inner_function", Python mencari di dalam cakupan lokal "outer_function" dan menemukan variabel "x" yang telah didefinisikan di sana. Oleh karena itu, nilai variabel "x" yang diakses di dalam "inner_function" berasal dari cakupan lokal "outer_function".

Contoh ini memberikan pemahaman praktis tentang bagaimana Python mengorganisir cakupan dan ruang nama, serta bagaimana akses ke variabel ditentukan berdasarkan urutan pencarian dalam berbagai cakupan.

## 9.3. A First Look at Classes <br>
Kelas memperkenalkan sedikit sintaks baru, tiga tipe objek baru, dan beberapa semantik baru

### 9.3.1. Class Definition Syntax <br>
Bagian 9.3.1 "Class Definition Syntax" dalam tutorial Python 3 menjelaskan sintaksis untuk mendefinisikan kelas dalam Python.

Kelas didefinisikan dengan menggunakan kata kunci "class" diikuti dengan nama kelas yang diawali dengan huruf kapital. Setelah deklarasi kelas, blok kode yang mengikuti akan menjadi tubuh kelas.

Tubuh kelas berisi atribut dan metode yang mendefinisikan perilaku dan karakteristik dari objek yang dibuat dari kelas tersebut. Atribut adalah variabel yang terkait dengan kelas dan menyimpan informasi tentang objek. Metode adalah fungsi yang terkait dengan kelas dan digunakan untuk melakukan operasi pada objek.

Metode khusus, seperti "__init__", dipanggil secara otomatis saat objek kelas dibuat. Notasi titik digunakan untuk mengakses atribut atau memanggil metode dari objek kelas.

Selain atribut dan metode, kelas juga dapat memiliki variabel kelas yang bersifat bersama untuk semua objek kelas yang dibuat. Kelas juga dapat memiliki metode kelas yang diakses melalui kelas itu sendiri dan bukan melalui objek kelas.

Dengan memahami sintaksis definisi kelas dalam Python, kita dapat membuat tipe baru yang mengikuti struktur dan perilaku yang telah ditentukan dalam kelas tersebut.

### 9.3.2. Class Objects <br>
Bagian 9.3.2 "Class Objects" dalam tutorial Python 3 menjelaskan tentang objek kelas (class objects).

Objek kelas adalah instansi dari sebuah kelas dan memiliki atribut serta metode yang terkait. Atribut adalah variabel yang terkait dengan objek kelas, sedangkan metode adalah fungsi yang terkait dengan objek tersebut. Atribut dan metode dapat diakses melalui objek kelas menggunakan notasi titik.

Setiap objek kelas memiliki ruang nama yang terpisah, tetapi mereka berbagi struktur dan perilaku yang ditentukan oleh kelas yang sama. Objek kelas dapat dibuat menggunakan sintaksis "nama_kelas()" dan konstruktor kelas, yang merupakan metode khusus, dipanggil saat objek kelas dibuat.

Konstruktor kelas dapat menginisialisasi atribut objek menggunakan argumen yang diteruskan saat pembuatan objek. Objek kelas juga dapat dihapus dari memori menggunakan pernyataan "del" atau ketika tidak lagi direferensikan oleh objek lain.

Pemahaman tentang objek kelas memungkinkan kita untuk membuat dan mengelola instansi dari kelas dengan atribut dan perilaku yang terkait.

### 9.3.3. Instance Objects <br>
Bagian 9.3.3 "Instance Objects" dalam tutorial Python 3 membahas tentang objek instansi (instance objects).

Objek instansi adalah objek yang dibuat dari kelas dan mewakili kasus individu atau instansi khusus dari kelas tersebut. Setiap objek instansi memiliki atribut yang membedakannya dari objek instansi lain yang dibuat dari kelas yang sama.

Atribut objek instansi adalah variabel yang terkait dengan objek tersebut. Atribut dapat diakses dan dimodifikasi melalui objek instansi menggunakan notasi titik. Setiap objek instansi memiliki ruang nama terpisah yang menyimpan nilai unik untuk atributnya.

Ketika objek instansi dibuat, konstruktor kelas dipanggil untuk melakukan inisialisasi awal. Konstruktor kelas adalah metode khusus yang didefinisikan dalam kelas dengan nama "__init__". Dalam konstruktor, kita dapat menginisialisasi atribut objek instansi dengan nilai-nilai awal yang diberikan.

Objek instansi juga dapat memiliki metode, yang merupakan fungsi yang terkait dengan objek tersebut. Metode digunakan untuk melakukan operasi pada objek instansi dan dapat diakses melalui objek menggunakan notasi titik.

Pemahaman tentang objek instansi memungkinkan kita untuk menciptakan objek yang mewakili instansi-individu dengan atribut dan perilaku yang unik dalam kelas yang didefinisikan.

### 9.3.4. Method Objects <br>
Bagian 9.3.4 "Method Objects" dalam tutorial Python 3 menjelaskan tentang objek metode (method objects).

Objek metode adalah objek yang mewakili metode yang terkait dengan sebuah kelas. Metode adalah fungsi yang didefinisikan dalam kelas dan digunakan untuk melakukan operasi pada objek yang dibuat dari kelas tersebut.

Ketika sebuah metode dipanggil, objek metode yang terkait dengan metode tersebut dibuat secara otomatis. Objek metode ini menyimpan referensi ke metode asli bersama dengan objek instansi yang memanggil metode.

Objek metode dapat disimpan dalam variabel dan digunakan untuk memanggil metode yang terkait. Ketika objek metode dipanggil, metode yang terkait dijalankan pada objek instansi yang telah ditentukan sebelumnya.

Objek metode juga dapat diteruskan sebagai argumen ke metode lain atau digunakan dalam ekspresi lambda. Dalam kasus ini, objek metode berfungsi sebagai objek fungsi yang dapat dipanggil.

Pemahaman tentang objek metode memungkinkan kita untuk mengoperasikan metode dengan cara yang lebih fleksibel, seperti menyimpan metode dalam variabel, memanggil metode pada objek instansi yang telah ditentukan sebelumnya, atau mengirimkan objek metode sebagai argumen.

### 9.3.5. Class and Instance Variables <br>
