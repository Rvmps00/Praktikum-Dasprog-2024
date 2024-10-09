# Asistensi Modul 4 Praktikum Dasar Pemrograman

<img src="https://www.its.ac.id/komputer/wp-content/uploads/sites/28/2018/03/image10.png" alt="Teknik Komputer ITS" width="150" height="150">

## Deskripsi

Soal-soal yang diberikan dalam sesi asistensi ini dirancang untuk melatih mahasiswa dalam mengimplementasikan konsep-konsep tingkat lanjut dari pemrograman C. Setiap soal dipilih untuk memberikan pengalaman langsung dalam menggunakan pointer, double pointer, struct, algoritma sorting dan searching, serta pengelolaan memori dinamis.

## Soal Asistensi

1. **Hack the Matrix: Simulasi Sistem Manajemen Data Kompleks dengan C**

   Neo ingin menavigasi sistem Matrix dengan cara yang lebih efisien dan aman. Sebagai programmer ulung, kamu diminta untuk membuat sistem manajemen data yang sangat efisien menggunakan berbagai teknik pemrograman dalam bahasa C. Program yang kamu buat harus bisa menangani database dinamis yang menyimpan data orang-orang dalam Matrix, memproses data tersebut, dan menampilkan informasi yang relevan.

   Kamu diminta untuk melakukan beberapa hal berikut:

   - Struktur Data Dinamis: Buatlah struct untuk menyimpan informasi pengguna di Matrix yang terdiri dari nama, ID, level akses, dan status.

      - Nama: string yang menyimpan nama pengguna.
      - ID: integer unik yang mewakili setiap pengguna.
      - Level Akses: integer yang menyatakan hak akses pengguna (misalnya, dari level 1 sampai 5).
      - Status: string yang bisa berisi "Active" atau "Inactive".
      - Dynamic Memory Allocation: Data pengguna disimpan dalam array dinamis. Program harus dapat menerima data untuk N pengguna di awal, dan memungkinkan pengguna memperbarui jumlah data yang disimpan secara dinamis menggunakan realloc.

   - Sorting dan Searching: Implementasikan algoritma sorting (gunakan quick sort) untuk mengurutkan data berdasarkan ID. Selain itu, implementasikan pencarian binary search untuk menemukan pengguna berdasarkan ID.

   - File Handling: Simpan data yang telah diurutkan ke dalam file "database_matrix.txt". Implementasikan juga fitur untuk membaca data dari file jika ada.

   - Pointer dan Double Pointer: Gunakan pointer dan double pointer untuk menangani array dinamis dan untuk memproses string dan manipulasi data lainnya.

   - Fungsi dan Rekursi: Implementasikan fungsi rekursif untuk menghitung jumlah total pengguna dengan status "Active".

   - Manipulasi Bit: Implementasikan fitur untuk mengenkripsi data ID menggunakan manipulasi bit (misalnya dengan melakukan operasi XOR dengan sebuah key) sebelum disimpan ke file.

   - Error Handling: Pastikan program memiliki error handling untuk kondisi seperti alokasi memori yang gagal atau file yang tidak ditemukan.
   
      __Input__:
  
      - Jumlah pengguna `N`.
      - Data pengguna berupa `nama`, `ID`, `level akses`, dan `status` untuk setiap pengguna.
      - Pilihan untuk melakukan sorting, pencarian, atau pembaruan data.

      __Output__:

      - Data yang diurutkan berdasarkan `ID`.
      - Hasil pencarian pengguna berdasarkan `ID`.
      - Total pengguna dengan status "Active".
      - Penyimpanan data ke file dengan `ID` yang telah dienkripsi.

   __Contoh Input__:

         Masukkan jumlah pengguna: 3
         Masukkan data pengguna:
         Nama: Neo
         ID: 1001
         Level Akses: 5
         Status: Active
         
         Nama: Trinity
         ID: 1003
         Level Akses: 4
         Status: Active
         
         Nama: Morpheus
         ID: 1002
         Level Akses: 3
         Status: Inactive
         
         Pilih aksi:
         1. Urutkan data berdasarkan ID
         2. Cari pengguna berdasarkan ID
         3. Hitung jumlah pengguna Active
         4. Simpan data ke file
         5. Baca data dari file
         Pilihan: 1

   __Contoh Output__:

         Data setelah diurutkan berdasarkan ID:
         Nama: Neo, ID: 1001, Level Akses: 5, Status: Active
         Nama: Morpheus, ID: 1002, Level Akses: 3, Status: Inactive
         Nama: Trinity, ID: 1003, Level Akses: 4, Status: Active
         
         Data disimpan ke dalam file "database_matrix.txt" dengan ID yang telah dienkripsi.

2. **Matrix Flex: Menaklukkan Operasi Matriks Dinamis dengan Double Pointer**

   Kamu diminta untuk merancang algoritma yang dapat mengelola dan melakukan operasi matriks secara efisien. Dalam tantangan ini, buat program C yang memanfaatkan double pointer untuk mengelola matriks dinamis. Program ini harus bisa menerima input ukuran matriks, melakukan penjumlahan dan perkalian, serta memastikan hasil ditampilkan dengan benar. Sebagai programmer berpengalaman, kamu akan mengeksplorasi pengelolaan memori dinamis dan manipulasi data matriks yang fleksibel, menciptakan solusi optimal untuk operasi matriks di sistem ini.

   __Input__:
   
      - Ukuran matriks (baris dan kolom).
      - Elemen-elemen matriks A dan B.

     __Output__:

      - Hasil penjumlahan dan perkalian matriks.

      __Contoh Input/Output__:

         Masukkan ukuran matriks (baris dan kolom): 2 2
         Masukkan elemen matriks A:
         1 2
         3 4
         Masukkan elemen matriks B:
         5 6
         7 8
         
         Hasil Penjumlahan:
         6 8
         10 12
         
         Hasil Perkalian:
         19 22
         43 50

       
3. **Recursive Tower: Implementasi Tower of Hanoi dengan Rekursi**

   Dalam sebuah dunia penuh teka-teki, kamu diminta untuk memecahkan masalah klasik Tower of Hanoi menggunakan kekuatan rekursi. Sebagai programmer handal, tugasmu adalah merancang program C yang mampu memindahkan cakram dari satu tiang ke tiang lain secara efisien. Programmu akan menampilkan setiap langkah pemindahan cakram dengan jelas, sembari menghitung berapa banyak langkah yang dibutuhkan untuk menyelesaikan tantangan ini. Bisakah kamu memecahkan misteri ini dan mengoptimalkan setiap gerakan dengan sempurna?

   __Input__:
   
      - Jumlah cakram.

   __Output__:
      
      - Langkah-langkah pemindahan cakram dan total langkah.

      __Contoh Input/Output__:

         Masukkan jumlah cakram: 3
         
         Langkah-langkah pemindahan:
         Pindahkan cakram dari tiang A ke tiang C
         Pindahkan cakram dari tiang A ke tiang B
         Pindahkan cakram dari tiang C ke tiang B
         ...
         Total langkah: 7

5.**Follow Akun Instagram @Re_vamp00**

   lampirkan bukti follow imstagram dengan di print di letakkan di halaman terakhir laporan


   
SELAMAT MENGERJAKAN!
