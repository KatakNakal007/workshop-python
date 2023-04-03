# Ringkasan Minggu Ke-4
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

### 6.1. More on Modules <br>
membahas topik yang lebih lanjut tentang modul, termasuk cara mengimpor modul sebagai alias, penggunaan dari from...import statement, dan cara mengatur urutan pencarian modul dengan mengatur variabel lingkungan sys.path. Tutorial ini juga membahas tentang namespace packages dan namespace packages bertingkat. Bagian ini juga memberikan contoh penggunaan modul yang lebih spesifik seperti __name__ dan __main__.

### 6.1.1 Executing modules as scripts <br>
menjelaskan bagaimana sebuah file modul dapat dijalankan sebagai script. Dalam kasus ini, kode pada modul akan dijalankan sebagai program utama. Tutorial ini menjelaskan bahwa ketika file modul dijalankan sebagai script, variabel global __name__ akan diatur sebagai "__main__". Tutorial ini juga memberikan contoh sederhana dan menjelaskan penggunaan if __name__ == "__main__" untuk membedakan apakah kode dijalankan sebagai modul atau sebagai program utama.

### 6.1.2 The Module Search Path <br>
membahas tentang urutan pencarian modul ketika diimpor. Tutorial ini menjelaskan bahwa ketika sebuah modul diimpor, Python akan mencari modul tersebut di direktori saat ini, di direktori yang terdaftar dalam variabel lingkungan PYTHONPATH, dan di direktori bawaan Python. Tutorial ini juga menjelaskan bahwa urutan pencarian dapat diatur dengan mengubah variabel lingkungan sys.path. Tutorial ini memberikan contoh penggunaan sys.path untuk menambahkan direktori baru ke dalam urutan pencarian modul.

### 6.1.3 "Compliled" Python files <br>
membahas tentang file Python yang telah dikompilasi (bytecode). Tutorial ini menjelaskan bahwa ketika sebuah modul diimpor, Python akan mencari file .pyc (atau .pyo dalam mode optimasi) yang terkait. Jika file .pyc ditemukan dan tanggal pembuatannya lebih baru dari tanggal pembuatan file .py, maka Python akan menggunakan file .pyc tersebut. Tutorial ini juga menjelaskan cara untuk mengoptimalkan performa aplikasi dengan mengkompilasi file Python menggunakan opsi -O pada command line.

### 6.2. Standard Modules <br>
membahas tentang beberapa modul bawaan yang tersedia di Python dan dapat langsung digunakan tanpa perlu mengunduh atau menginstal modul tambahan. Tutorial ini memperkenalkan beberapa modul bawaan Python yang populer, seperti os, sys, math, dan random. Tutorial ini memberikan contoh penggunaan modul-modul tersebut dan menjelaskan beberapa fungsi penting yang tersedia dalam modul tersebut. Tutorial ini juga memberikan panduan untuk menjelajahi dokumentasi modul bawaan Python dan menemukan modul yang sesuai untuk kebutuhan pengembangan aplikasi.

### 6.3. The dir() Function <br>
membahas tentang fungsi bawaan dir() yang dapat digunakan untuk mendapatkan daftar atribut dan metode yang terdapat pada sebuah objek, baik itu modul, fungsi, kelas, atau instance dari kelas. Tutorial ini memberikan contoh penggunaan fungsi dir() pada beberapa objek, seperti modul bawaan Python, fungsi, dan kelas. Tutorial ini juga menjelaskan bahwa beberapa atribut atau metode mungkin tidak terlihat dengan fungsi dir() karena bersifat "private" atau dimulai dengan underscore (_).

### 6.4 Packages <br>
membahas tentang konsep paket (package), yaitu sebuah direktori yang berisi beberapa modul terkait yang dapat diimpor sebagai satu kesatuan. Tutorial ini menjelaskan cara membuat paket dengan membuat sebuah direktori dan menambahkan file __init__.py pada direktori tersebut. Tutorial ini juga membahas tentang penggunaan relative imports untuk mengimpor modul dari paket yang sama atau subpakat, dan memberikan contoh penggunaan from . import module dan from ..subpackage import module. Tutorial ini juga menjelaskan tentang penggunaan paket bawaan Python dan bagaimana menavigasi struktur direktori dari paket tersebut.

### 6.4.1. Importing * From a Package <br>
membahas tentang penggunaan pernyataan from package import * untuk mengimpor semua nama yang didefinisikan dalam paket ke dalam ruang nama saat ini. Tutorial ini menjelaskan bahwa penggunaan import * dianggap buruk karena dapat menyebabkan konflik nama dan membuat kode sulit dipahami. Tutorial ini menyarankan untuk mengimpor modul secara eksplisit dan menggunakan aliasing (penamaan ulang) jika diperlukan. Tutorial ini juga menjelaskan bahwa jika modul paket memiliki atribut __all__, maka hanya nama-nama yang terdaftar dalam atribut tersebut yang akan diimpor saat menggunakan from package import *.

### 6.4.2. Intra-package References <br>
membahas tentang cara mengimpor modul dari paket yang sama menggunakan relative imports. Tutorial ini menjelaskan bahwa relative imports memungkinkan kita untuk menggunakan nama modul yang relatif terhadap modul saat ini, dengan menggunakan tanda titik (.) sebagai pemisah. Tutorial ini memberikan contoh penggunaan relative imports pada modul dalam paket yang sama dan subpakat, menggunakan pernyataan from . import module dan from ..subpackage import module. Tutorial ini juga memberikan panduan tentang cara menggunakan relative imports secara aman, dengan memeriksa apakah modul diimpor sebagai modul top-level atau sebagai modul yang diimpor dari modul lain.

### 6.4.3. Packages in Multiple Directories <br>
membahas tentang cara membuat paket yang terdiri dari beberapa direktori. Tutorial ini menjelaskan bahwa untuk membuat paket yang terdiri dari beberapa direktori, kita dapat menggunakan file __init__.py di setiap direktori yang terkait untuk mengekspor modul dari direktori tersebut. Tutorial ini memberikan contoh struktur direktori untuk paket yang terdiri dari beberapa direktori, dan bagaimana modul dapat diimpor dari direktori tersebut. Tutorial ini juga memberikan panduan tentang cara mengelola search path untuk modul dan paket menggunakan variabel lingkungan PYTHONPATH atau dengan menambahkan direktori ke sys.path.
