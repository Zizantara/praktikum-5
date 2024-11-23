# Data Diri
 
 Nama   : Zizantara Arzeva Cakra Kahana

 NIM    : 312410398

 Kelas  : TI.24.A.3

# Flowchart

<img src="flowchart.jpg" widht=500 height=500>

# Program Input Nilai

## Input Program 

<img src="Inputprog.png">

## Output Program 
 
 - Output yang di hasilkan ketika menginput ( L )

    <img src="L.png">

 - Output yang di hasilkan ketika menginput ( T )

    <img src="T.png">

 - Output yang di hasilkan ketika menginput ( L ) setelah Menginput ( T )

    <img src="L2.png">

 - Output yang di hasilkan ketika menginput ( U )

    <img src="U.png">

 - Output yang di hasilkan ketika menginput ( L ) setelah Menginput ( U )

    <img src="LU.png">

 - Output yang di hasilkan ketika menginput ( H )

    <img src="H.png">

 - Output yang di hasilkan ketika menginput ( L ) setelah Menginput ( H )

    <img src="LH.png">

 - Output yang di hasilkan ketika menginput ( C )

    <img src="C.png">

 - Output yang di hasilkan ketika menginput ( K )

    <img src="K.png">

# Deskripsi Program 

1. STRUKTUR CLASS DAN INISIALISASI

    <img src="d1.png">

    - Program menggunakan class StudentGradeSystem untuk mengorganisir kode dan data.

    - __init__ adalah constructor yang dijalankan saat objek dibuat.

    - self.students adalah dictionary kosong yang akan menyimpan data dengan struktur:

    <img src="d2.png">

2. PERHITUNGAN NILAI AKHIR

    <img src="d3.png">

    - Method untuk menghitung nilai akhir sesuai bobot yang ditentukan:

        - Tugas: 30% (0.30)

        - UTS: 35% (0.35)

        - UAS: 35% (0.35)

    - Menerima 3 parameter: nilai tugas, UTS, dan UAS

    - Mengembalikan hasil perhitungan sebagai nilai float

3. PENAMBAHAN DATA MAHASISWA

    <img src="d4.png">

    - Memulai dengan mengecek duplikasi NIM

    - Jika NIM sudah ada, tampilkan pesan error dan keluar dari fungsi

    <img src="d5.png">

    - Input data mahasiswa dengan validasi:

        - Mengkonversi input nilai ke float

        - Memastikan semua nilai antara 0-100

        - Menggunakan try-except untuk menangani input non-numerik

    <img src="d6.png">

   - Menghitung nilai akhir

   - Menyimpan data dalam dictionary dengan struktur nested

4. PEMBARUAN DATA MAHASISWA

    <img src="d7.png">

    - Mencari NIM yang akan diupdate

    - Validasi keberadaan NIM sebelum melakukan update

    <img src="d8.png">

    - Proses input dan validasi sama seperti penambahan data

    <img src="d9.png">

    - Menggunakan method update() untuk memperbarui data yang ada

5. PENGHAPUSAN DATA

    <img src="d10.png">

    - Menggunakan operator del untuk menghapus data dari dictionary

    - Validasi keberadaan NIM sebelum menghapus

6. PENCARIAN DATA

    <img src="d11.png">

    - Mencari data berdasarkan NIM

    - Menampilkan data dalam format tabel jika ditemukan

    - Menggunakan string formatting untuk alignment:

        - ^ untuk center alignment

        - < untuk left alignment

        - .2f untuk format float dengan 2 desimal

7. MENAMPILKAN DATA

    <img src="d12.png">

    - Mengecek apakah dictionary kosong

    - Menampilkan pesan khusus jika tidak ada data

    <img src="d13.png">

    - Menggunakan enumerate() untuk memberikan nomor urut

    - Iterasi melalui dictionary menggunakan items()

    - Menampilkan data dalam format tabel yang rapi

8. MENU UTAMA

    <img src="d14.png">

    - Menggunakan dictionary untuk memetakan pilihan menu ke method yang sesuai

    - Memudahkan penambahan menu baru di masa depan

    <img src="d15.png">

    - Loop utama program

    - Mengkonversi input ke lowercase untuk fleksibilitas

    - Eksekusi method sesuai pilihan menu

    - Validasi input menu

9. MENJALANKAN PROGRAM

    <img src="end.png">

    - Membuat instance dari class StudentGradeSystem

    - Menjalankan program saat file dieksekusi langsung

# FITUR KEAMANAN DAN VALIDASI:

1. Validasi Input:

    -  Pengecekan duplikasi NIM

    - Validasi rentang nilai (0-100)

    - Penanganan input non-numerik dengan try-except

    - Validasi menu yang dipilih

2. Keamanan Data:

    - Data tersimpan dalam struktur dictionary yang terorganisir

    - Tidak ada akses langsung ke data dari luar class

    - Validasi sebelum modifikasi data

3. User Interface:

    - Menu yang jelas dan mudah dipahami

    - Pesan error yang informatif

    - Format tampilan yang konsisten dan rapi

    - Konfirmasi untuk operasi penting