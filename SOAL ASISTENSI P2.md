# Asistensi Modul 2 Praktikum Dasar Pemrograman

<img src="https://www.its.ac.id/komputer/wp-content/uploads/sites/28/2018/03/image10.png" alt="Teknik Komputer ITS" width="150" height="150">

## Deskripsi

Soal-soal yang diberikan dalam sesi asistensi ini dirancang untuk membantu mahasiswa memahami konsep ekspresi logika, perbandingan, percabangan (if, if-else, if-else-if), nested if, looping, array, dan string dalam bahasa C. Dengan memberikan tantangan yang lebih kompleks dibandingkan soal di modul, asistensi ini bertujuan untuk memperdalam pemahaman mahasiswa dalam menerapkan konsep-konsep tersebut dalam skenario yang lebih realistis dan bervariasi. Melalui sesi asistensi ini, Praktikan diharapkan mampu mengembangkan kemampuan analisis dan problem-solving yang lebih mendalam dalam menyusun alur logika program serta menyelesaikan masalah pemrograman yang lebih rumit.

## Soal Asistensi

1. **Pesta Tiket Konser! Pesan Banyak, Diskon Melayang!**

   Siap-siap datang ke konser favoritmu dengan sistem pemesanan tiket otomatis ini! Beli tiket lebih banyak dan dapatkan diskon gila-gilaan, ditambah kode promo spesial buat potongan harga ekstra. Yuk cek seberapa besar diskon yang bisa kamu dapatkan!
   
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

2. **Lulus atau Tidak? Cek Nilai Ujianmu di Sini!**

   Program ini mengelompokkan nilai mata kuliah mahasiswa dan menentukan apakah kamu layak lulus berdasarkan nilai rata-rata dan kriteria lulus yang ketat. Siapkan nilaimu dan cek sekarang!

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

3. **Crazy Deals: Diskon Gede-Gedean di Toko Elektronikmu!**

   Dapatkan penawaran diskon gila-gilaan dengan jumlah barang yang kamu beli. Semakin banyak, semakin besar diskonmu! Masukkan pesananmu dan hitung diskon yang bakal kamu dapatkan.

   Kriteria Diskon:
   
   - Tidak ada diskon jika jumlah barang yang dibeli ≤ 10.
   - Diskon 5% jika jumlah barang > 10 dan ≤ 20.
   - Diskon 10% jika jumlah barang > 20 dan ≤ 50.
   - Diskon 15% jika jumlah barang > 50.
   
   __Input__:
   
   - Nama barang (string).
   - Jumlah barang yang dibeli (integer).
   - Harga per unit barang (float).

   __Output__:
   
   - Tampilkan nama barang.
   - Tampilkan jumlah barang yang dibeli.
   - Tampilkan harga total sebelum diskon.
   - Tampilkan diskon yang didapat.
   - Tampilkan total harga setelah diskon.
  
      __Contoh Input__:

         Nama barang: Laptop
         Jumlah barang: 25
         Harga per unit: 7500000

      __Contoh Output__:

         Nama Barang: Laptop
         Jumlah Barang: 25
         Harga Total Sebelum Diskon: Rp187.500.000
         Diskon: 10%
         Total Setelah Diskon: Rp168.750.000
5.**Follow Akun Instagram @Re_vamp00**

   lampirkan bukti follow imstagram dengan di print di letakkan di halaman terakhir laporan
   
SELAMAT MENGERJAKAN !!
