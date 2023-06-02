# Ringkasan Minggu Ke-7
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

# 9. Classes <br>
Bagian 9. Classes dalam tutorial Python 3 membahas tentang kelas (classes) dalam Python:

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
Bagian 9.3.5 "Class and Instance Variables" dalam tutorial Python 3 menjelaskan tentang variabel kelas dan variabel instansi.

Variabel kelas adalah variabel yang terkait dengan kelas itu sendiri, bukan dengan objek instansi yang dibuat dari kelas. Variabel kelas dapat diakses melalui kelas atau objek instansi dan berlaku untuk semua objek instansi yang dibuat dari kelas tersebut.

Variabel instansi adalah variabel yang terkait dengan objek instansi tertentu. Setiap objek instansi memiliki salinan terpisah dari variabel instansi, dan perubahan pada variabel instansi tidak mempengaruhi objek instansi lain.

Variabel kelas didefinisikan di dalam tubuh kelas, di luar metode kelas. Mereka dapat diakses melalui notasi titik menggunakan nama kelas atau objek instansi. Variabel kelas juga dapat diakses melalui metode kelas dan metode instansi.

Variabel instansi biasanya didefinisikan di dalam metode kelas, terutama dalam konstruktor kelas "__init__". Setiap objek instansi memiliki salinan terpisah dari variabel instansi tersebut.

Pemahaman tentang variabel kelas dan variabel instansi memungkinkan kita untuk mengatur dan membagikan data antara kelas dan objek instansi. Variabel kelas cocok untuk menyimpan informasi yang bersifat bersama untuk semua objek instansi, sementara variabel instansi cocok untuk menyimpan informasi yang spesifik untuk setiap objek instansi.

## 9.4. Random Remarks <br>
Bagian 9.4 "Random Remarks" dalam tutorial Python 3 berisi beberapa catatan acak yang berkaitan dengan pemrograman berorientasi objek dalam Python.

Penggunaan penamaan konvensi PEP 8 direkomendasikan dalam pemrograman berorientasi objek Python. Ini mencakup penggunaan huruf kecil dengan pemisah garis bawah untuk nama kelas, penggunaan huruf kapital dengan pemisah garis bawah untuk nama metode, dan sebagainya.

Python mendukung warisan tunggal, yang berarti sebuah kelas hanya dapat mewarisi dari satu kelas dasar.

Metode dan atribut dalam kelas dapat diwarisi dan diubah oleh kelas turunan.

Keyword "super" digunakan untuk mengakses metode yang diwarisi dari kelas dasar saat mendefinisikan metode yang sama di kelas turunan.

Polimorfisme adalah kemampuan objek untuk memiliki banyak bentuk. Dalam Python, polimorfisme dapat dicapai melalui metode yang sama dengan perilaku yang berbeda pada kelas-kelas yang berbeda.

Metode "isinstance()" dan "issubclass()" digunakan untuk memeriksa hubungan antara objek dan kelas dalam hierarki pewarisan.

Encapsulation adalah konsep untuk menyembunyikan implementasi internal objek dan hanya memungkinkan akses melalui antarmuka publik.

Python mendukung multiple inheritance, yang memungkinkan kelas untuk mewarisi dari lebih dari satu kelas dasar. Namun, penggunaan multiple inheritance harus diperhatikan dengan hati-hati untuk menghindari ambiguitas dan konflik.

Duck typing adalah prinsip dalam Python yang berfokus pada perilaku objek daripada tipe kelasnya. Jika objek bertindak seperti bebek dan berbunyi seperti bebek, maka dianggap sebagai bebek.

Perubahan pada kelas induk tidak secara otomatis tercermin pada kelas turunannya. Jika perubahan diperlukan, kelas turunan harus secara eksplisit mengimplementasikan perubahan tersebut.

## 9.5. Inheritance <br>
Bagian 9.5 "Inheritance" dalam tutorial Python 3 membahas tentang warisan (inheritance) dalam pemrograman berorientasi objek.

Warisan adalah konsep yang memungkinkan kelas untuk mewarisi atribut dan metode dari kelas lain yang disebut kelas dasar atau superclass. Kelas yang mewarisi atribut dan metode disebut kelas turunan atau subclass.

Dalam warisan, kelas turunan dapat menggunakan atribut dan metode yang sudah ada dalam kelas dasar tanpa perlu mendefinisikannya ulang. Ini memungkinkan untuk mengorganisir dan mengelompokkan kode secara hierarkis.

Untuk mewarisi dari kelas dasar, sintaksis "class NamaKelasTurunan(NamaKelasDasar):" digunakan. Dalam definisi kelas turunan, kita dapat menambahkan atribut dan metode baru atau mengubah yang sudah ada.

Konsep warisan juga mendukung konsep polimorfisme, di mana objek kelas turunan dapat digunakan sebagai objek kelas dasar. Hal ini memungkinkan fleksibilitas dalam penggunaan objek dan memungkinkan penggunaan pola desain seperti polimorfisme dan substitusi Liskov.

Pemahaman tentang warisan memungkinkan kita untuk mengorganisir kode secara hierarkis dan memanfaatkan kembali atribut dan metode yang sudah ada dalam kelas dasar, sehingga mempercepat pengembangan dan meningkatkan keterbacaan dan pemeliharaan kode.

### 9.5.1. Multiple Inheritance <br>
Bagian 9.5.1 "Multiple Inheritance" dalam tutorial Python 3 menjelaskan tentang multiple inheritance atau pewarisan ganda.

Multiple inheritance adalah konsep di mana sebuah kelas dapat mewarisi atribut dan metode dari lebih dari satu kelas dasar. Dalam hal ini, kelas turunan memiliki beberapa kelas dasar.

Dalam Python, untuk menggunakan multiple inheritance, kita dapat menyebutkan beberapa kelas dasar dipisahkan oleh tanda koma setelah kata kunci "class". Kelas turunan akan mewarisi atribut dan metode dari semua kelas dasar yang diberikan.

Multiple inheritance dapat memberikan fleksibilitas dalam merancang hierarki kelas yang kompleks dan memungkinkan untuk menggabungkan fungsionalitas dari berbagai kelas dasar. Namun, penggunaan multiple inheritance harus dilakukan dengan hati-hati untuk menghindari kebingungan dan konflik yang mungkin terjadi.

## 9.6. Private Variables <br>
Bagian 9.6 "Private Variables" dalam tutorial Python 3 menjelaskan tentang variabel pribadi (private variables) dalam pemrograman berorientasi objek.

Variabel pribadi adalah variabel yang dianggap bersifat pribadi dan seharusnya tidak diakses atau dimodifikasi langsung dari luar kelas. Variabel pribadi dimulai dengan garis bawah ganda (underscore) di awal namanya, seperti "_namaVariabel".

Variabel pribadi diimplementasikan menggunakan konvensi dan aturan tertentu, tetapi secara teknis masih dapat diakses dan dimodifikasi dari luar kelas. Namun, penggunaan garis bawah ganda menandakan bahwa variabel tersebut seharusnya digunakan secara pribadi dan tidak dianggap sebagai bagian publik antarmuka kelas.

Pemahaman tentang variabel pribadi memungkinkan untuk membatasi akses dan modifikasi langsung pada variabel dalam kelas, sehingga mendorong enkapsulasi dan penggunaan metode sebagai antarmuka publik untuk berinteraksi dengan data kelas tersebut.

## 9.7. Odds and Ends <br>
Bagian 9.7 "Odds and Ends" dalam tutorial Python 3 berisi beberapa informasi tambahan yang berkaitan dengan pemrograman berorientasi objek dalam Python.

Mengakses atribut dan metode kelas langsung menggunakan notasi titik, seperti "NamaKelas.namaAtribut" atau "NamaKelas.namaMetode()".

Dalam Python, objek fungsi juga dapat digunakan sebagai metode kelas dan diakses melalui objek instansi.

Menggunakan fungsi built-in "getattr()" untuk mengakses atribut atau metode dari objek secara dinamis.

Dalam Python, semua tipe data adalah objek, termasuk tipe data dasar seperti angka dan string.

Konstruktor kelas, "__init__()", dapat digunakan untuk melakukan inisialisasi saat objek instansi dibuat.

"self" digunakan dalam definisi metode kelas untuk mengacu pada objek instansi yang sedang dikerjakan.

Penerusan metode ("method delegation") adalah konsep yang memungkinkan objek delegasi untuk memanggil metode pada objek lain.

Dalam Python, tidak ada kewajiban untuk mendeklarasikan tipe parameter dalam definisi metode. Ini dikenal sebagai "duck typing".

Konsep "getter" dan "setter" digunakan untuk mengakses dan memodifikasi atribut dengan cara yang terkontrol.

## 9.8. Iterators <br>
Bagian 9.8 "Iterators" dalam tutorial Python 3 membahas tentang konsep iterator dalam pemrograman Python.

Iterator adalah objek yang digunakan untuk mengiterasi atau mengulang secara berurutan melalui elemen-elemen dari suatu koleksi atau struktur data. Iterasi adalah proses melalui elemen-elemen satu per satu.

Untuk mendukung iterasi, suatu objek harus mengimplementasikan dua metode khusus: "__iter__()" dan "__next__()". Metode "__iter__()" mengembalikan objek iterator itu sendiri, sementara metode "__next__()" mengembalikan elemen berikutnya dalam iterasi. Jika tidak ada elemen berikutnya, metode "__next__()" harus menghasilkan pengecualian StopIteration untuk menghentikan iterasi.

Iterasi dapat dilakukan menggunakan pernyataan "for" yang umum digunakan dalam Python. Pernyataan "for" akan secara otomatis memanggil metode "__iter__()" untuk mendapatkan iterator dan menggunakan metode "__next__()" untuk mendapatkan elemen-elemen selama iterasi.

Dalam Python, banyak struktur data bawaan seperti list, tuple, set, dan dictionary telah diimplementasikan dengan dukungan untuk iterasi. Selain itu, kita juga dapat membuat iterator kustom dengan mengimplementasikan metode "__iter__()" dan "__next__()" pada kelas kita sendiri.

Pemahaman tentang konsep iterator memungkinkan kita untuk melintasi dan memanipulasi elemen-elemen dalam koleksi dengan cara yang efisien dan mudah dipahami.

## 9.9. Generators <br>
Bagian 9.9 "Generators" dalam tutorial Python 3 membahas tentang konsep generator dalam pemrograman Python.

Generator adalah fungsi khusus yang menghasilkan serangkaian nilai secara bertahap, satu nilai pada satu waktu, tanpa harus menyimpan seluruh rangkaian nilai dalam memori. Generator memungkinkan kita untuk menghasilkan nilai-nilai secara efisien dalam situasi di mana menghasilkan seluruh rangkaian nilai sekaligus akan memakan banyak memori.

Untuk membuat generator, kita menggunakan kata kunci "yield" dalam fungsi. Ketika "yield" dieksekusi, generator akan menghasilkan nilai tersebut dan menyimpan keadaan internalnya. Pada pemanggilan berikutnya, generator akan melanjutkan dari keadaan terakhirnya dan menghasilkan nilai berikutnya.

Ketika sebuah generator dieksekusi, itu mengembalikan objek generator yang dapat diiterasi. Kita dapat menggunakan pernyataan "for" untuk mengiterasi melalui nilai-nilai yang dihasilkan oleh generator, atau menggunakan fungsi bawaan seperti "next()" untuk mendapatkan nilai berikutnya.

Generator sangat berguna dalam situasi di mana kita perlu menghasilkan serangkaian nilai yang besar atau tak terbatas secara efisien. Mereka juga memungkinkan pemrogram untuk menggunakan konsep "lazy evaluation" di mana nilai-nilai dihasilkan hanya ketika mereka benar-benar diperlukan.

Pemahaman tentang konsep generator memungkinkan kita untuk membuat fungsi yang menghasilkan serangkaian nilai secara efisien dan membantu menghemat sumber daya memori.

## 9.10. Generator Expressions <br>
Bagian 9.10 "Generator Expressions" dalam tutorial Python 3 membahas tentang ekspresi generator, yang merupakan cara singkat untuk membuat generator dalam Python.

Generator expression mirip dengan list comprehension, tetapi menggunakan tanda kurung () daripada tanda kurung siku []. Mereka memungkinkan kita untuk membuat generator secara langsung dalam satu baris kode, tanpa perlu mendefinisikan fungsi terpisah.

Dalam generator expression, kita menuliskan ekspresi yang menghasilkan nilai untuk setiap elemen dalam rangkaian yang diinginkan. Generator expression akan secara otomatis menghasilkan nilai-nilai ini satu per satu saat diminta, tanpa perlu menyimpan semua nilai dalam memori.

Kita dapat menggunakan generator expression dalam berbagai konteks, seperti argumen fungsi, dalam konstruksi perulangan, atau dalam fungsi lain yang menerima iterator.

Generator expression sangat berguna ketika kita hanya perlu menghasilkan serangkaian nilai sementara, tanpa membutuhkan struktur data list yang lengkap. Ini dapat menghemat penggunaan memori dan mempercepat eksekusi kode.

Pemahaman tentang generator expression memungkinkan kita untuk menggunakan pendekatan yang lebih ringkas dan efisien dalam menghasilkan dan memanipulasi serangkaian nilai dalam Python.
