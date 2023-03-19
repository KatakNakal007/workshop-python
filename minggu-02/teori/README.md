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
