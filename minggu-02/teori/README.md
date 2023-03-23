# Ringkasan Minggu Ke-2
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___
## Bab 4 Lebih banyak alat kontrol flow
selain while statement yang telah di perkenalkan sebelumnya, Python juga biasa menggunakan statement flow
kontrol yang biasa digunakan oleh bahasa pemrograman lain, dengan beberapa twist

### Statement if
salah satu tipe statement yang cukup terkenal adalah if statement dan Python juga bisa menggunakannya

### Statement for
for statement yang ada di Python sedikit berbeda dengan apa yang biasa di gunakan C atau Pascal. 
Dibandingkan harus selalu meng iterasikan progres aritmatik dari nomor (seperti dalam Pasca), atau memberikan
user kemampuan untuk mengdefinisikan langkah iterasi kemudian memberikan jeda (seperi C), statement for pada
Python langsung meng iterasikan item dari berbagai urutan (list ataupun string), yang secara otomatis berurutan

codingan yang memodifikasi collection saat sedang di iterasi dengan collection yang sama biasa cukup tricky untuk benarkan
malahan biasanya lebih mudah untuk mengulangi salinan collection atau membuat collection baru

### Function range()
jika ingin meng iterasikan sekumpulan angka, built-in function range() bisa sangan membantu. ia dapat membuat proses aritmatik

bagian end point yang di berikan tidak akan menjadi bagian dari urutan yang di hasilkan

untuk meng iterasikan beberapa index dari sebuah urutan, bisa dengan menggabungkan range() dan len()

dalam banyak hal objek yang dikembalikan oleh range() berperilaku seolah-olah itu adalah list, 
tetapi sebenarnya bukan. itu adalah objek yang mengembalikan item berturut-turut dari urutan yang di inginkan saat di iterasikan
tetapi tidak benar-benar membuat list sehingga lebih menghemat ruang

bisa dikatakan objek seperti itu dapat diubah, yaitu cocok sebagai target untuk fungsi dan konstruksi yang mengharapkan sesuatu dari mana mereka 
dapat memperoleh item berturut-turut hingga persediaan habis.

### Statement break dan continue, dan klausa else pada perulangan
break statemen yang ada di Python sama seperti di C, breaks keluar dari for atau perulangan while yang telampir

statement perulangan mungkin saja mempunyai klausa else; yang di eksekusi ketika perulangan berakhir (dengan for) 
atau ketika kondisi menjadi false (dengan while), tetapi tidak ketika perulangan di akhiri dengan peryantaan break.

statement continue pun di teruskan dari bahasa C

### Statement pass
statement pass di melakukan apa-apa, ia bisa digunakan ketika statement di butuhkan secara sintaksis, 
tetapi program tidak membutuhkan aksi apapun

### Statement match
statement match mengambil ekspresi dan membandingkan nilai nya dengan pola berturut-turut yang berikan sebagai
satu atau beberapa case blocks, mirip-mirip seperti statement switch yang ada di C, Javam atau JavaScript
(dan bahasa pemrograman lainnya)
 
kamu bisa mengkombinasikan beberapa literasi dalam satu pola menggunakan | ("or")

kamu bisa menggunakan positional parameters dengan beberapa kelas yang memberikan sebuah urutan untuk atributnya (misalnya dataclasses). kamu juga bisa mendefinisikan posisi yang spesifik untuk atribut pada pola dengan mengatur __match_args__ atribut spesial di dalam kelasmu.

kita bisa menambahkan klausa if pada pola, yang di kenal sebagai "guard". jika guard adalah false, match akan mencoba case block selanjutnya. perlu di ingat nilai tangkapan terjadi sebelum guard di evaluasi

kebanyakan literasi di komparisikan dengan dengan persamaan, namun jika hanya satu True, False, dan None maka akan di komparasikan dengan identitas.

pola bisa saja menggunakan nama konstan. ia harus di berika tanda titik untuk mencegah nya di interpretasikan sebagai capture variabel

### Mendefinisikan Functions
kata kunci def memperkenalkan definisi function. ia harus diikuti dengan nama function dan daftar dalam kurung dari formal parameters.

eksekusi function memperkenalkan tabel simbol baru yang digunakan untuk local variabel dari sebuah function. lebih tepatnya, semua tugas variabel di dalam function menyimpan nilai di local tabel simbol; sedangkan referensi variabel di lihat dulu di local tabel simbol, lalu di local tabel simbol dari enclosing function, lalu di global simbol tabel, dan akhirnya di dalam nama built-in tabel. demikian global variabel dan variabel enclosing function tidak bisa langsung di beri nilai di antara function (kecuali, untuk global variabel, nama pada global statement, atau, for variabel dari enclosing function, dinamai di nonlocal statement).

parameter yang sebenarnya (arguments) dari function call di perkenalkan di local tabel simbol dari called function ketika ia di panggil; demikian, argument di lewatkan menggunakan call by value atau dipanggil dari nilai (dimana value atau nilai selalu merupakan objek referensi, bukan value atau nilai dari objek).

ketika function memanggil function lain atau memanggil dirinya secara rekursif, tabel simbol baru akan di buat setelah function di panggil.

definisi function mengasosiasikan nama function dengan function objek di dalam simbol tabel saat ini. interpreter mengenali objek yang di tunjuk dari nama sebagai user-defined function.

return statement dikembalikan dengan value dari function. return tanpa sebuah expression argument di kembalikan None atau kosong.

### Mendefinisikan function lainnya

sangat dimungkinkan untuk mendefenisikan function dengan variabel number dari arguments. ada tiga form, yang bisa di kombinasikan

#### Nilai argument default
merupakan form yang paling berguna untuk menspesifik nilai default dari satu argumen atau lebih. ia dapat membuat function yang bisa di panggil hanya dengan beberapa argumen dari apa yang dibutuhkan.

function ini dapat di panggil dengan beberapa cara:
* cukup dengan memberikan argument yang wajib
* memberikan salah satu argument pilihan
* atau bahkan memberikan semua argument sekaligus

**Peringatan :** nilai default hanya dapat di evaluasi sekali. ini memberikan perbedaan ketika default adalah mutable objek seperti list, dictionary, atau instansi dari kebanyakan kelas.

#### Argument kata kunci
function juga bisa di panggil menggunakan kata kunci argumen dari bentuk kwarg=value.

dalam pemanggilan function, kata kunci argument harus mengikuti posisional argument. semua kata kunci argumen yang lewat harus cocok dengan salah satu argument yang diterima oleh function (misalnya, actor bukan merupakan argument yang valid dengan function parrot), dan urutunnya tidak penting. ini juga termasuk non-optional argument (misalnya, parrot(voltage=1000) juga valid). tidak ada argument yang mungkin bisa menerima value atau nilai lebih dari sekali.

ketika final parameter dari form **name ditampilkan, ia menerima dictionary yang memuat semua kata kunci argument kecuali yang sesuai dengan formal parameter. ia mungkin bisa di kombinasikan dengan formal parameter dari form *name yang menerima tuple yang memuat posisional argument di luar dari list formal parameter (*name harus ada terlebih dahulu sebelum **name).

#### Parameters spesial
secara default, argument di lewatkan ke function Python dapat melalui posisi ataupun secara explisit menggunakan kata kunci. secara keterbacaan dan performa, sangat masuk akal untuk membatasi cara argument di lewatkan sehingga developar hanya butuh melihat definisi function untuk menentukan jika items di lewatkan melalui posisi, melalui posisi atau kata kunci, atau melalui kunci

#### Argument posisional atau kata kunci
jika / dan * tidak di muncul pada definis function, argument mungkin saja di lewatkan ke function melalui posisi atau melalui kata kunci.

#### Positional-Only Parameters
sangat di mungkinkan untuk menandai beberapa parameter sebagai position-only. jika positional-only, urutan parameter diperhitungkan, dan parameter tidak bisa di lewatkan dengan kata kunci. positional-only parameters ditempatkan sebelum / (garis miring). / digunakan untuk secara logis memisahkan positional-only parameters dari parameters yang lain. jika tidak terdapat / pada definisi function, maka tidak ada positional-only parameters

#### Keyword-Only Arguments
untuk menandai parameters sebagai keyword-only, menunjukkan parameter harus di lewatkan menggunakan argumen kata kunci, tempatkan * pada argument list sebelum keyword-only parameter pertama.

#### Contoh function
