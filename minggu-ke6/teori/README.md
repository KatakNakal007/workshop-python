# Ringkasan Minggu Ke-5
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___

## 8.1. Syntax Errors <br>
Bagian 8.1. Syntax Errors menjelaskan tentang kesalahan sintaksis dalam Python. Kesalahan sintaksis terjadi ketika Anda menulis kode yang melanggar aturan tata bahasa Python, sehingga interpreter tidak dapat memahami atau mengeksekusi kode tersebut.

Tutorial ini menjelaskan bahwa kesalahan sintaksis biasanya terjadi saat menuliskan pernyataan yang tidak valid, seperti menggunakan karakter yang tidak diperbolehkan, lupa menambahkan tanda kutip, atau salah menempatkan tanda kurung. Pesan kesalahan akan memberikan petunjuk tentang lokasi dan jenis kesalahan sintaksis yang terjadi.

Untuk memperbaiki kesalahan sintaksis, Anda perlu memeriksa dengan teliti kode yang Anda tulis dan mencari tanda-tanda kesalahan seperti tanda kurung yang tidak seimbang atau penulisan yang salah. Tutorial ini juga memberikan beberapa contoh kesalahan sintaksis umum beserta solusi yang tepat.

Dengan memahami kesalahan sintaksis dan cara memperbaikinya, Anda dapat menghindari masalah sintaksis dalam kode Python Anda dan memastikan bahwa program Anda dapat dijalankan dengan benar.

## 8.2. Exceptions <br>
Bagian 8.2. Exceptions menjelaskan tentang pengecualian (exceptions) dalam Python. Pengecualian adalah kondisi yang tidak normal atau kesalahan yang terjadi selama eksekusi program, yang mengganggu alur normal program.

Tutorial ini menjelaskan bahwa pengecualian dapat terjadi karena beberapa alasan, seperti pembagian oleh nol, mengakses indeks yang tidak valid dalam daftar, atau kesalahan file yang tidak ditemukan. Ketika pengecualian terjadi, program akan berhenti dan pesan kesalahan yang terkait dengan pengecualian akan ditampilkan.

Dalam tutorial ini, Anda akan mempelajari cara menangani pengecualian menggunakan pernyataan try-except. Pernyataan try digunakan untuk menjalankan blok kode yang mungkin menghasilkan pengecualian, sedangkan pernyataan except digunakan untuk menangkap dan menangani pengecualian yang terjadi. Anda dapat menentukan jenis pengecualian yang ingin Anda tangani secara spesifik.

## 8.3. Handling Exceptions <br>
Bagian 8.3. Handling Exceptions membahas tentang penanganan pengecualian (exceptions) dalam Python dengan lebih rinci.

Tutorial ini menjelaskan bahwa penanganan pengecualian adalah proses mengatasi pengecualian yang terjadi dalam program dengan cara yang diinginkan. Dalam penanganan pengecualian, Anda dapat menentukan bagaimana program akan bereaksi terhadap pengecualian tertentu.

Pertama, tutorial menjelaskan tentang struktur umum penanganan pengecualian menggunakan pernyataan try-except. Blok try digunakan untuk menempatkan kode yang mungkin menyebabkan pengecualian, sedangkan blok except digunakan untuk menangkap dan menangani pengecualian yang spesifik. Anda dapat menentukan jenis pengecualian yang ingin Anda tangani dengan lebih rinci.

Selanjutnya, tutorial membahas penggunaan blok finally yang digunakan untuk menentukan kode yang harus dijalankan terlepas dari apakah pengecualian terjadi atau tidak. Blok finally berguna untuk membersihkan sumber daya atau melakukan tindakan akhir yang penting dalam program.

Tutorial juga mencakup penggunaan pernyataan raise yang memungkinkan Anda memicu pengecualian secara manual. Anda dapat menggunakan pernyataan raise untuk menghentikan eksekusi program dan menghasilkan pengecualian khusus yang sesuai dengan kebutuhan Anda.

Selain itu, tutorial mengulas konsep penanganan pengecualian yang lebih kompleks dengan menggunakan blok try-except-finally yang bersarang. Ini memungkinkan Anda untuk menangani pengecualian yang terjadi dalam blok try dalam cara yang lebih terperinci dan fleksibel.

Dengan memahami penanganan pengecualian dalam Python, Anda dapat mengendalikan perilaku program Anda ketika pengecualian terjadi. Hal ini membantu Anda dalam mengatasi situasi yang tidak diharapkan, menjaga keandalan program, dan memberikan pengalaman yang lebih baik kepada pengguna.

## 8.4. Raising Exceptions <br>
Bagian 8.4. Raising Exceptions menjelaskan tentang penimbulan pengecualian (raising exceptions) secara manual dalam Python.

Tutorial ini menjelaskan bahwa dalam beberapa kasus, Anda mungkin perlu memicu pengecualian secara manual untuk menghentikan eksekusi program dan memberikan pesan yang sesuai dengan kondisi yang tidak diinginkan. Penimbulan pengecualian memungkinkan Anda untuk membuat pengecualian khusus yang sesuai dengan kebutuhan Anda.

Dalam penimbulan pengecualian, Anda menggunakan pernyataan raise yang diikuti oleh jenis pengecualian yang ingin Anda timbulkan. Anda dapat menyertakan pesan yang menjelaskan alasan pengecualian dalam tanda kurung setelah jenis pengecualian.

Tutorial ini juga memberikan contoh penggunaan penimbulan pengecualian untuk situasi yang berbeda, seperti pengecualian ValueError saat menerima input yang tidak valid atau pengecualian FileNotFound saat mencoba membuka file yang tidak ada.

Dengan memahami penimbulan pengecualian, Anda dapat membuat kode yang lebih responsif dan memberikan pesan yang jelas dan informatif ketika terjadi kondisi yang tidak diinginkan dalam program Anda.

## 8.5. Exception Chaining <br>
Bagian 8.5. Exception Chaining membahas tentang penggabungan pengecualian (exception chaining) dalam Python.

Tutorial ini menjelaskan bahwa penggabungan pengecualian memungkinkan Anda untuk mengaitkan beberapa pengecualian bersama sehingga Anda dapat melacak jejak pengecualian yang terjadi secara hierarkis. Hal ini bermanfaat ketika Anda ingin melacak asal usul pengecualian atau memberikan informasi yang lebih rinci tentang kesalahan yang terjadi.

Dalam Python, saat menangani pengecualian, Anda dapat menggunakan kata kunci from diikuti dengan pengecualian lainnya untuk menghubungkannya secara hierarkis. Dengan melakukan ini, Anda dapat membentuk rantai pengecualian yang menggambarkan alur pengecualian yang terjadi.

Tutorial ini memberikan contoh penggunaan penggabungan pengecualian dengan mengaitkan pengecualian yang ditimbulkan di dalam blok try-except dengan pengecualian yang lebih umum di luar blok try-except. Hal ini memungkinkan Anda untuk menjaga jejak pengecualian yang terjadi dan memberikan informasi yang lebih lengkap tentang kesalahan tersebut.

Dengan memahami penggabungan pengecualian, Anda dapat membuat penanganan pengecualian yang lebih terperinci dan lebih informatif dalam program Python Anda. Hal ini membantu dalam pemecahan masalah dan pemeliharaan program yang lebih efektif.

## 8.6. User-defined Exceptions <br>
Bagian 8.6. User-defined Exceptions menjelaskan tentang pengecualian yang didefinisikan oleh pengguna (user-defined exceptions) dalam Python.

Tutorial ini menjelaskan bahwa dalam Python, Anda dapat membuat pengecualian khusus yang sesuai dengan kebutuhan Anda. Pengecualian yang didefinisikan oleh pengguna memungkinkan Anda untuk membuat kategori pengecualian khusus yang dapat digunakan dalam program Anda.

Untuk membuat pengecualian khusus, Anda perlu membuat kelas yang mewarisi dari kelas dasar Exception atau salah satu kelas pengecualian yang sudah ada. Dalam kelas tersebut, Anda dapat menentukan perilaku dan properti khusus yang ingin Anda tambahkan.

Tutorial ini memberikan contoh pembuatan pengecualian khusus dengan membuat kelas baru yang mewarisi Exception. Anda dapat menambahkan metode khusus dalam kelas tersebut untuk menyesuaikan perilaku pengecualian yang Anda buat.

Dengan pengecualian yang didefinisikan oleh pengguna, Anda dapat mengatur penanganan pengecualian yang lebih spesifik dan memberikan pesan yang sesuai dengan konteks program Anda. Hal ini membantu dalam pemeliharaan program dan mempermudah pemecahan masalah yang berkaitan dengan kesalahan yang terjadi.

## 8.7. Defining Clean-up Actions <br>
Bagian 8.7. Defining Clean-up Actions membahas tentang definisi tindakan pembersihan (clean-up actions) dalam Python.

Tutorial ini menjelaskan bahwa terkadang Anda perlu menjalankan kode tertentu setelah blok try-except selesai dieksekusi, terlepas dari apakah pengecualian terjadi atau tidak. Tindakan pembersihan ini dapat berupa penutupan file, pembebasan sumber daya, atau tugas lain yang harus dilakukan untuk membersihkan program.

Dalam Python, Anda dapat menggunakan blok finally untuk mendefinisikan tindakan pembersihan. Blok finally akan dijalankan setelah blok try-except selesai, terlepas dari apakah pengecualian terjadi atau tidak.

Tutorial ini memberikan contoh penggunaan blok finally dalam beberapa skenario. Misalnya, Anda dapat menggunakan blok finally untuk memastikan bahwa sumber daya yang dibuka, seperti file, ditutup dengan benar tanpa memperhatikan pengecualian yang terjadi di dalam blok try.

Dengan menggunakan blok finally, Anda dapat memastikan bahwa tindakan pembersihan penting dilakukan setelah eksekusi blok try-except selesai. Ini membantu dalam menjaga kebersihan dan keandalan program Anda, serta mencegah kebocoran sumber daya yang tidak diinginkan.

## 8.8. Predefined Clean-up Actions <br>
Bagian 8.8. Predefined Clean-up Actions menjelaskan tentang tindakan pembersihan yang telah ditentukan sebelumnya (predefined clean-up actions) dalam Python.

Tutorial ini menjelaskan bahwa Python menyediakan beberapa mekanisme bawaan untuk melakukan tindakan pembersihan secara otomatis. Beberapa contoh tindakan pembersihan yang telah ditentukan sebelumnya termasuk:

Menggunakan pernyataan with: Pernyataan with digunakan untuk mengelola sumber daya eksternal seperti file atau koneksi database. Dengan menggunakan pernyataan with, Anda dapat memastikan bahwa sumber daya tersebut ditutup secara otomatis setelah digunakan.

Menggunakan fungsi close(): Beberapa objek seperti file dan socket memiliki metode close() yang dapat dipanggil untuk menutupnya. Anda dapat memanggil metode close() secara manual setelah selesai menggunakan objek tersebut.

Menggunakan manajer konteks: Python menyediakan manajer konteks yang memungkinkan Anda untuk menentukan tindakan pembersihan khusus untuk suatu blok kode. Manajer konteks dapat digunakan dengan pernyataan with untuk menjalankan kode sebelum dan setelah blok with dieksekusi.

Tutorial ini memberikan contoh penggunaan pernyataan with dan manajer konteks untuk melakukan tindakan pembersihan yang telah ditentukan sebelumnya. Dengan menggunakan mekanisme ini, Anda dapat memastikan bahwa sumber daya eksternal ditutup dengan benar setelah digunakan, menghindari kebocoran sumber daya yang mungkin terjadi.

Dengan memanfaatkan tindakan pembersihan yang telah ditentukan sebelumnya dalam Python, Anda dapat menulis kode yang lebih bersih, efisien, dan dapat diandalkan dalam pengelolaan sumber daya eksternal.

## 8.9. Raising and Handling Multiple Unrelated Exceptions <br>
Bagian 8.9. Raising and Handling Multiple Unrelated Exceptions membahas tentang penimbulan dan penanganan beberapa pengecualian yang tidak terkait dalam Python.

Tutorial ini menjelaskan bahwa dalam beberapa situasi, Anda mungkin perlu menimbulkan atau menangani beberapa pengecualian yang tidak terkait secara bersamaan. Misalnya, Anda dapat memiliki beberapa blok kode yang mungkin menimbulkan pengecualian yang berbeda, dan Anda ingin menangani pengecualian tersebut secara terpisah.

Dalam Python, Anda dapat menimbulkan pengecualian yang tidak terkait dengan menggunakan pernyataan raise di berbagai blok kode yang relevan. Anda dapat menentukan jenis pengecualian yang berbeda dan pesan yang sesuai dengan setiap pengecualian.

Selanjutnya, tutorial membahas tentang penanganan pengecualian yang tidak terkait. Anda dapat menggunakan beberapa blok except untuk menangkap dan menangani pengecualian yang berbeda secara terpisah. Setiap blok except akan menangani jenis pengecualian tertentu, sehingga Anda dapat memberikan penanganan yang sesuai berdasarkan jenis pengecualian yang terjadi.

Tutorial ini memberikan contoh penggunaan penimbulan dan penanganan pengecualian yang tidak terkait. Dengan memahami konsep ini, Anda dapat mengelola dan mengatasi pengecualian yang terjadi secara terpisah dan memberikan penanganan yang sesuai berdasarkan kondisi dan jenis pengecualian yang terjadi.

Dengan kemampuan untuk menimbulkan dan menangani beberapa pengecualian yang tidak terkait, Anda dapat menulis kode yang lebih fleksibel dan tanggap terhadap situasi yang beragam dalam program Python Anda.

## 8.10. Enriching Exceptions with Notes <br>
Bagian 8.10. Enriching Exceptions with Notes membahas tentang pengayaan pengecualian (exceptions) dengan catatan (notes) tambahan dalam Python.

Tutorial ini menjelaskan bahwa terkadang Anda mungkin ingin menambahkan informasi tambahan atau catatan khusus ke dalam pengecualian yang ditimbulkan. Hal ini berguna untuk memberikan detail atau konteks yang lebih spesifik tentang kondisi yang menyebabkan pengecualian.

Dalam Python, Anda dapat menggunakan atribut args dalam kelas pengecualian untuk menyimpan catatan atau informasi tambahan. Atribut args adalah tuple yang berisi argumen yang diberikan saat pengecualian ditimbulkan. Anda dapat menambahkan catatan atau informasi tambahan ke dalam tuple ini.

Tutorial ini memberikan contoh penggunaan atribut args untuk mengayaikan pengecualian dengan catatan tambahan. Anda dapat mengatur nilai atribut args saat menimbulkan pengecualian atau mengaksesnya kemudian untuk membaca atau memodifikasinya.

Dengan kemampuan untuk mengayaikan pengecualian dengan catatan tambahan, Anda dapat memberikan informasi yang lebih spesifik dan bermanfaat tentang kondisi yang menyebabkan pengecualian. Hal ini membantu dalam pemecahan masalah dan mempermudah pemeliharaan program yang mengandalkan pengecualian.
