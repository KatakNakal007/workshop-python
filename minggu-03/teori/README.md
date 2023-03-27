# Ringkasan Minggu Ke-2
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___
## Bab 5

### 5.1. More on List
List dalam Python adalah tipe data yang terdiri dari kumpulan nilai atau item yang terurut dan dapat diubah. Artikel ini menjelaskan cara membuat list, mengakses elemen list, memotong list, menggabungkan list, dan menggunakan fungsi built-in untuk mengoperasikan list seperti len(), max(), dan min().

Artikel ini juga membahas operator identitas "in" dan "not in" untuk memeriksa apakah sebuah nilai atau item ada atau tidak ada di dalam list, serta operator "+=" untuk menambahkan nilai ke dalam list. Selain itu, artikel ini juga membahas perbedaan antara penggunaan operator "=" dan "copy()" untuk meng-copy list.

Terakhir, artikel ini membahas beberapa metode built-in untuk memanipulasi list seperti append(), insert(), remove(), pop(), dan index(). Metode-metode ini memungkinkan pengguna untuk menambah, menghapus, dan mengubah elemen di dalam list.

### 5.1.1 Using List as Stacks
cara menggunakan list sebagai tumpukan (stack).

Tumpukan adalah struktur data yang memungkinkan item-item baru ditambahkan atau dihapus hanya dari satu ujung. List dalam Python dapat digunakan sebagai tumpukan dengan menggunakan metode built-in seperti append() untuk menambahkan item ke ujung list dan pop() untuk menghapus item dari ujung list.

Artikel ini menjelaskan cara menggunakan metode-metode tersebut untuk membuat tumpukan, mengakses dan menghapus item dari tumpukan, dan memeriksa apakah tumpukan kosong atau tidak. Selain itu, artikel ini juga membahas penggunaan fungsi len() untuk menghitung jumlah item dalam tumpukan.

Terakhir, artikel ini memberikan contoh penggunaan tumpukan dalam sebuah program untuk membalikkan sebuah string. 

### 5.1.2. Using List as Queues
cara menggunakan list sebagai antrian (queue).

Antrian adalah struktur data yang memungkinkan item-item baru ditambahkan ke salah satu ujung dan dihapus dari ujung yang lain. List dalam Python juga dapat digunakan sebagai antrian dengan menggunakan metode built-in seperti append() untuk menambahkan item ke ujung list dan pop() dengan argumen 0 (nol) untuk menghapus item dari awal list.

Artikel ini menjelaskan cara menggunakan metode-metode tersebut untuk membuat antrian, menambahkan dan menghapus item dari antrian, dan memeriksa apakah antrian kosong atau tidak. Selain itu, artikel ini juga membahas penggunaan fungsi len() untuk menghitung jumlah item dalam antrian.

Namun, artikel juga menekankan bahwa penggunaan list sebagai antrian tidak efisien karena ketika sebuah item dihapus dari awal list, seluruh item di dalam list perlu bergeser ke posisi yang lebih rendah. Oleh karena itu, jika digunakan secara intensif, lebih baik menggunakan struktur data khusus seperti collections.deque atau queue.Queue yang dirancang khusus untuk operasi antrian.

Terakhir, artikel ini memberikan contoh penggunaan antrian dalam sebuah program untuk mensimulasikan antrian pelanggan dalam sebuah restoran.

### 5.1.3. List Comprehensions
cara menggunakan list comprehension untuk membuat list secara lebih singkat dan efisien.

List comprehension adalah sintaksis ringkas yang memungkinkan kita membuat list baru dengan mengambil nilai dari list atau urutan yang ada, melakukan operasi pada nilai tersebut, dan mengembalikan hasil dalam bentuk list. Sintaksis list comprehension terdiri dari tanda kurung siku yang berisi ekspresi, diikuti oleh satu atau lebih klausa for dan kondisi opsional.

Artikel ini menjelaskan cara menggunakan list comprehension untuk membuat list angka kuadrat, list angka genap, dan list kombinasi elemen dari dua list. Selain itu, artikel ini juga membahas penggunaan klausa if dalam list comprehension untuk memfilter elemen yang memenuhi kondisi tertentu.

List comprehension merupakan cara yang efisien dan elegan untuk membuat list dalam Python, karena menggabungkan proses filter, transformasi, dan pembuatan list dalam satu baris kode.

### 5.1.4. Nested List Comprehensions
cara membuat list comprehension bersarang (nested) untuk menghasilkan list multidimensional atau list yang lebih kompleks.

Nested list comprehension adalah list comprehension yang mengandung satu atau lebih ekspresi for yang tertulis secara bertingkat, sehingga dapat memproses elemen dari dua atau lebih list secara bersamaan.

Artikel ini menjelaskan cara menggunakan nested list comprehension untuk membuat list berisi elemen dari beberapa list secara teratur dan secara acak, serta cara menggunakan klausa if dan else dalam nested list comprehension.

Selain itu, artikel ini juga membahas bagaimana menggabungkan nested list comprehension dengan fungsi built-in seperti zip() dan enumerate() untuk membuat list dengan lebih efisien dan elegan.

Nested list comprehension dapat membuat kode kita lebih ringkas dan mudah dibaca. Namun, perlu diingat bahwa semakin dalam tingkat nesting, semakin sulit memahami kode tersebut, sehingga perlu dipertimbangkan antara keefektifan dan keterbacaan kode.

### 5.2. The del statement
