# Asistensi Modul 2 Praktikum Dasar Pemrograman

<img src="https://www.its.ac.id/komputer/wp-content/uploads/sites/28/2018/03/image10.png" alt="Teknik Komputer ITS" width="150" height="150">

## Deskripsi

Soal-soal yang diberikan dalam sesi asistensi ini dirancang untuk membantu mahasiswa memahami konsep dasar pemrograman dalam bahasa C dengan fokus pada penggunaan fungsi input-output dasar (scanf dan printf). Asistensi ini bertujuan untuk memberikan pengalaman langsung dalam menerapkan teori yang telah dipelajari di Praktikum.

## Soal Asistensi

1. **Printf vs Scanf: Siapa yang Lebih Kuat?**

   Anda diminta membuat program sistem pemesanan tiket konser. Program ini harus mampu menerima nama pengguna, jenis tiket yang dipilih, dan jumlah tiket yang ingin dibeli. Sistem juga harus memvalidasi input pengguna, menghitung total harga tiket, memberikan diskon berdasarkan kondisi tertentu, dan mencetak faktur yang rapi.

   Ketentuan Tiket:

   Terdapat tiga jenis tiket:
   - VIP dengan harga Rp1.500.000 per tiket
   - Reguler dengan harga Rp750.000 per tiket
   - Economy dengan harga Rp300.000 per tiket
   - Jika pengguna membeli lebih dari 5 tiket, mereka akan mendapatkan diskon 10% dari total harga.
   - Jika pengguna memasukkan kode promo DISKON50, mereka akan mendapatkan diskon tambahan 50% dari total harga setelah diskon pembelian di atas 5 tiket.

   Validasi:

   - Nama tidak boleh kosong atau lebih dari 50 karakter.
   - Jenis tiket harus salah satu dari VIP, Reguler, atau Economy.
   - Jumlah tiket harus lebih dari 0 dan tidak lebih dari 10.
   - Kode promo bersifat opsional, tetapi jika diisi harus valid, yaitu DISKON50.

   __Input__:
   - Nama pengguna (string).
   - Jenis tiket yang dipilih (string: VIP, Reguler, Economy).
   - Jumlah tiket yang dibeli (integer).
   - Kode promo (opsional) (string).   
 
   __Output__:
   - Tampilkan nama pengguna.
   - Tampilkan jenis tiket yang dipilih.
   - Tampilkan jumlah tiket yang dibeli.
   - Tampilkan total harga tiket sebelum dan setelah diskon.
   - Jika ada kode promo, tampilkan harga setelah diskon promo.

   __Contoh Input 1__:

         Nama: Budi Setiawan
         Jenis tiket: VIP
         Jumlah tiket: 6
         Kode promo: DISKON50

   __Contoh Output 1__:

         Faktur Pemesanan Tiket Konser:
         Nama: Budi Setiawan
         Jenis Tiket: VIP
         Jumlah Tiket: 6
         Total Harga Sebelum Diskon: Rp9.000.000
         Diskon Pembelian Lebih Dari 5 Tiket: 10%
         Total Setelah Diskon: Rp8.100.000
         Kode Promo: DISKON50
         Total Setelah Promo: Rp4.050.000

   __Contoh Input 2__

         Nama: Ana Dewi
         Jenis tiket: Reguler
         Jumlah tiket: 3
         Kode promo: 

   __Contoh Output 2__:

         Faktur Pemesanan Tiket Konser:
         Nama: Ana Dewi
         Jenis Tiket: Reguler
         Jumlah Tiket: 3
         Total Harga Sebelum Diskon: Rp2.250.000
         Tidak ada diskon pembelian lebih dari 5 tiket.
         Total Setelah Diskon: Rp2.250.000
         Tidak ada kode promo.

1. **Data Entry Aman: Nama, NRP, dan Umur Tanpa Drama!**

   Anda diminta membuat program yang mengelompokkan nilai mata kuliah mahasiswa berdasarkan beberapa kriteria. Program ini harus menerima input berupa NIM, nama, dan nilai dari 5 mata kuliah. Program kemudian akan menghitung nilai rata-rata, menampilkan hasil dari setiap mata kuliah, dan memberikan keterangan apakah mahasiswa tersebut lulus atau tidak berdasarkan rata-rata nilai. Mahasiswa dinyatakan lulus jika rata-rata nilainya ≥ 60 dan tidak ada nilai yang di bawah 50.

   Ketentuan Nilai:
   
   Mahasiswa dinyatakan LULUS jika:
   - Rata-rata nilai dari 5 mata kuliah ≥ 60, dan Tidak ada satu pun nilai mata kuliah di bawah 50.
   - Jika ada mata kuliah dengan nilai di bawah 50, mahasiswa TIDAK LULUS meskipun nilai rata-rata ≥ 60.

     __Input__:
      
     - NIM mahasiswa (string).
     - Nama mahasiswa (string).
     - Nilai dari 5 mata kuliah (integer).

     __Output__:

     - Tampilkan NIM dan nama mahasiswa.
     - Tampilkan nilai dari setiap mata kuliah.
     - Tampilkan nilai rata-rata dari 5 mata kuliah.
     - Tampilkan status kelulusan mahasiswa (LULUS atau TIDAK LULUS).

      __Contoh Input__:

         NIM: 12345678
         Nama: Budi Setiawan
         Nilai Mata Kuliah 1: 70
         Nilai Mata Kuliah 2: 55
         Nilai Mata Kuliah 3: 65
         Nilai Mata Kuliah 4: 80
         Nilai Mata Kuliah 5: 45

      __Contoh Output 1__:

         NIM: 12345678
         Nama: Budi Setiawan
         Nilai Mata Kuliah:
         1: 70
         2: 55
         3: 65
         4: 80
         5: 45
         Rata-rata: 63.0
         Status: TIDAK LULUS

4. **Ganjil atau Genap: Siapakah Kamu?**

   Cuma satu angka, tapi dia bisa menentukan apakah kamu berada di sisi ganjil atau genap. Buat program sederhana yang memutuskan apakah sebuah bilangan adalah ganjil atau genap. Yuk, buktikan kekuatan logika sederhana ini!

   __Input__: Satu baris yang berisi satu bilangan bulat.

   __Output__: Tampilkan pesan apakah bilangan tersebut ganjil atau genap dalam format berikut:
      
      - Jika genap: Angka <angka> adalah genap.
      - Jika ganjil: Angka <angka> adalah ganjil.
  
      __Contoh Input 1__:

         7

      __Contoh Output 1__:

         Angka 7 adalah ganjil.

      __Contoh Input 2__:

         8

      __Contoh Output 2__:

         Angka 8 adalah genap.


SELAMAT MENGERJAKAN !!
   
