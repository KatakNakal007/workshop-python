# Ringkasan Minggu Ke-2
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___
## Bab 5

### 5.1. More on List
tipe data list mempunyai beberapa metode tambahan. yaitu

list.append(x)<br>
Menambahkan item pada di akhir pada list. Setara dengan a[len(a):] = [x].

list.extend(iterable)<br>
Meng extend list dengan menambahkan semua item dari iterable. Setara dengan a[len(a):] = iterable.

list.insert(i, x)<br>
Meng insert item pada posisi yang ditentukan. argumen pertama merupakan index dari elemen sebelum di insert, misalnya a.insert(0, x) di insert pada bagian terdepan dari list, dan a.insert(len(a), x) setara dengan a.append(x).

list.remove(x)<br>
Menghapus item pertama dari list yang valuenya sama dengan x.

list.pop([i])<br>
Mengahapus item dari posisi yang ditentukan pada list, dan me return nya. jika tidak terdapat index yang spesifik, a.pop() menghapus dan me returns item terakhir dari list.

list.clear()<br>
Menghapus semua item dari list. Setara dengan del a[:].

list.index(x[, start[, end]])<br>
Me return zero-bassed index pada list dari item pertama yang value nya sama dengan x.

list.count(x)<br>
Me return berapa kali x muncul pada list

list.sort(*, key=None, reverse=False)<br>
Meng sortir item dari list yang ada

list.reverse()<br>
Me return salinan dangkal dari list. Setara dengan a[:].

dapat dilihat bahwa method seperti insert, remove, atau sort hanya memodifikasi list yang tidak menampilkan return value - tapi me return default None.

5.1.1 Using List as Stacks
Method list mempermudah penggunaan list sebagai stack, dimana elemen terakhir yang di tambahkan merupakan elemen pertama yang di terima ("last-in, first-out"). Untuk menambahkan item pada bagian atas stack, dapat menggunakan append(). Untuk menerima item pada bagian atas stack, bisa menggunakan pop() tanpa explicit index. 
