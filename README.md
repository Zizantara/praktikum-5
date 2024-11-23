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

def update_student(self):
        """Mengubah data mahasiswa"""
        print("\nUbah Data")
        nim = input("Masukkan NIM yang akan diubah: ")
        if nim not in self.students:
            print("NIM tidak ditemukan!")
            return

