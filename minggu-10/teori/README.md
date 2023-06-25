# Ringkasan Minggu Ke-10
Nim: **205410121**<br>
Nama: **Muhammad Syukur**<br>
Kelas: **IF-3**
___
## Bagian menggunakan psycopg2 dengan CockroachDB <br>
bagian ini memberikan tutorial atau petunjuk seputar membuat python app dengan CockroachDB dan psycopg2

adapun langkah-langkahnya adalah sebagai berikut : <br>
#### Step 1. Start CockroachDB <br>
pada langkah ini terdapat petunjuk tentang pembuatan akun dan cluster di CockroachDB, adapun root sertificate dapat di download melalui powershell atau cmd menggunakan link yang di sertakan, dan link general connection string sebagai database url untuk terhubung kedalam cluster CockroahDB.

#### Step 2. Get the sample code <br>
pada langkah ini terdapat petunjuk untuk melakukan klongin data dari github yang nantinya digunakan untuk transfer data antara database lokal dengan cluster CockroachDB.

#### Step 3. Install the psycopg2 driver <br>
pada langkah ini terdapat petunjuk untuk menginstall psycopg2 sebagai dependency yang dibutuhkan untuk proses transfer data.

#### Step 4. Run the code <br>
pada langkah ini terdapat petunjuk untuk melakukan koneksi ke dalam cluster di CockroachDB, dan perintah untuk melakukan transfer data dengan menjalankan example.py.

## Bagian menggunakan SQLAlchemy dengan CockroachDB <br>
bagian ini memberikan tutorial atau petunjuk seputar melaukan CRUD sederhana dengan CockroachDB dan SQLAlchemy

adapun langkah-langkahnya  adalah sebagai berikut : <br>
#### Step 1. Start CockroachDB <br>
langkah ini sama seperti yang ada pada "Bagian menggunakan psycopg2 dengan CockroachDB".

#### Step 2. Get the code <br>
pada langkah ini terdapat petunjuk untuk melakukan klongin data dari github yang nantinya digunakan untuk CRUD ke dalam cluster CockroachDB.

#### Step 3. Install the apllication requirements <br>
pada langkah ini terdapat petunjuk untuk membuat virtual environment yang nantinya di gunakan sebagai direktori untuk melakukan proses CRUD.

#### Step 4. Initialize the database <br>
pada langkah ini terdapat petunjuk untuk melakukan koneksi ke dalam cluster CockroachDB, serta melakukan pembuatan tabel dengan perintah cat dbinit.sql | cockroach sql --url $DATABASE_URL .

#### Step 5. Run the code <br>
pada langkah ini terdapat petunjuk untuk melakukan CRUD ke dalam cluster CockroachDB dengan menjalankan main.py yang telah di kloning sebelumnya dari link github yang disertakan.

adapun beberapa petunjuk tambahan untuk mengganti prefix dan menampilkan hasil CRUD melalui SQL shell.
