# Tugas-2-Praktikum-Pemrograman-Web-2
# A. Koneksi1.php
# Coding koneksi1.php
<img width="398" alt="koneksi1 1" src="https://github.com/user-attachments/assets/88dc5f87-4c20-4ddb-81e8-06a14ee5e758">

# Penjelasan
# 1. Deklarasi Kelas (Mahasiwa)
- Kelas mahasiswa dibuat untuk mengelola koneksi ke database dan menjalankan query untuk mengambil data dari tabel.
- Terdapat beberapa properti yang didefinisikan:
  
   A. $localhost: Variabel ini digunakan untuk menyimpan alamat server database.
  
  B. $user: Nama pengguna database.
  
  C. $pass: Kata sandi untuk pengguna.
  
  D. $dbname: Nama database yang akan digunakan.
  
  E. $conn: Objek koneksi ke database yang diinisialisasi dalam constructor.
# 2. Constructor (__construct())
- Saat objek dari kelas Mahasiswa dibuat, fungsi ini otomatis dipanggil.
- Constructor menerima parameter ($localhost, $user, $pass, dan $dbname) untuk menginisialisasi koneksi ke database.
# 3. Metode (tampilkantugas2())
- Fungsi ini bertujuan untuk mengambil semua data dari tabel tugas2 di database.
- Langkah-langkanya:

  A. Query SQL (SELECT * FROM tugas2) digunakan untik mengambil semua data dari tabel (tugas2).

  B. Hasil query disimpan dalam variabel ($result) dan dikembalikan dengan (return $result).
# 4. Inisialisasi dan Pemanggilan Kelas (Mahasiswa)
- Objek dari kelas (mahasiswa) dibuat dengan menggunakan nilai-nilai variabel.
- Constructor akan dijalankan dan koneksi ke database diinisialisasi.
- Setelah objek terbentuk, metode ($tampilkantugas2()) dipanggil mengambil data dari tabel (tugas2).
- Hasil query akan disimpan dalam variabel ($datamahasiswa).

# B. Mahasiswa2.php
# Codingan Mahasiswa2.php
<img width="542" alt="Mahasiswa1" src="https://github.com/user-attachments/assets/10adb41f-8707-4f46-b6b6-edaea015325e">
<img width="314" alt="Mahasiswa2" src="https://github.com/user-attachments/assets/f64e9b8e-035a-44a1-aef0-b2be3fcb0f8a">
<img width="173" alt="Mahasiswa3" src="https://github.com/user-attachments/assets/29ce7c04-116d-4ce2-8a43-e982caa0e355">

# Penjelasan
# 1. Kelas (mahasiswa)
Fungsi fetchData():
Kelas Mahasiswa mendefinisikan sebuah metode bernama fetchData() yang mengembalikan sebuah array yang berisi data beberapa mahasiswa.
Setiap elemen dari array ini berisi array asosiatif dengan informasi berikut:

A. nim: Nomor Induk Mahasiswa.

B. nama: Nama mahasiswa.
        
C. alamat: Alamat tempat tinggal mahasiswa.

D. email: Alamat email mahasiswa.

E. no_telp: Nomor telepon mahasiswa.

# 2. Bagian HTML
- HTML Structure
  
  A Bootsrap CSS: File CSS dari Boostrap diambil dari web dan diintegerasikan ke halaman untuk memudahkan styling.
  
  B. Bootstrap JS: Library JavaScript Bootstrap juga diambil dari CDN untuk mendukung fitur interaktif.
  
  C. Background Styling: Halaman memiliki latar belakang berwarna (aquamarine), yang diatur langsung dalam elemen (<body>).

# 3. Judul Halaman
- Judul halaman berisi teks "Data Mahasiswa" dan ditampilkan di tengah halaman dengan kelas Bootstrap (text-center) untuk mengatur posisi tengah secara horizontal.
  
# 4. Tabel untuk Menampilkan Data

- Struktur Tabel:
  
  A. Bagian utama dari HTML adalah tabel yang dirancang untuk menampilkan data mahasiswa.
  
  B. Ada dua bagian penting dari tabel:
  - thead: Bagian kepala tabel (header) berisi judul kolom seperti "NO", "NIM", Nama Mahasiswa", "Alamat", "Email", dan "No Telp". 
  - tbody: Bagian tubuh tabel, berisi data mahasiswa dalam bentuk baris.
        
# 5. Penjelasan Setiap Baris Tabel
- Setiap baris didalam <tbody> mewakili data dari seorang mahasiswa:
   - Kolom pertama (NO) berisi nomor urut.
   - Kolom kedua berisi NIM mahasiswa.
   - Kolom ketiga berisi nama mahasiswa.
   - Kolom keempat berisi alamat mahasiswa.
   - Kolom kelima berisi email mahasiswa.
   - Kolom keenam berisi no telepon mahasiswa.

 # Output
 <img width="959" alt="Output mahasiswa2" src="https://github.com/user-attachments/assets/06d0ed04-124c-422e-9069-951558cc394b">

# C. Nilai_perbaikan.php
# Codingan Nilai_perbaikan.php
<img width="538" alt="Nilai_perbaikan1" src="https://github.com/user-attachments/assets/b84ee909-5db0-433b-9c9c-d8d22e32ccf6">
<img width="308" alt="Nilai_perbaikan2" src="https://github.com/user-attachments/assets/4a7e58b9-5721-4070-a5b5-f91781e0088d">
<img width="191" alt="Nilai_perbaikan3" src="https://github.com/user-attachments/assets/99221cd8-b232-4502-88d5-f4a444f19922">

# Penjelasan
# 1. Kelas (Mahasiswa)
- Kelas ini berfungsi untuk menyediakan data mahasiswa yang berisi informasi terkait perbaikan nilai mereka.
- Fungsi fetchData() mengembalikan data dalam bentuk array yang berisi beberapa informasi, seperti:
  - tanggal_perbaikan: Tanggal dilakukannya perbaikan nilai.
  - keterangan: Jenis perbaikan (contoh: remidi atau UAS).
  - mahasiswa_ID: ID dari mahasiswa.
  - mata_kuliah_ID: ID mata kuliah terkait perbaikan.
  - semester_ID: ID semester.
  - nilai_ID: ID nilai yang diperbaiki.
  - dosen_ID: ID dosen yang terkait dengan perbaikan nilai tersebut.

# 2. Struktur Halaman

- Judul halaman: (h1 class="text-center")Data Nilai Perbaikan mahasiswa (/h1) menampilkan judul di tengah halaman. 
-  Tabel data:
    - Menggunakan elemen (table) dengan kelas Bootstrap table untuk membuat     tabel yang sudah diformat.
    - Kepala tabel (thead) ditambahkan kelas table-dark untuk memberi warna   gelap pada header tabel.
    - Setiap baris berisi informasi perbaikan mahasiswa (tanggal, keterangan,   ID mahasiswa, ID mata kuliah, ID semester, nilai, dan dosen).

 # 3. Isi Tabel
 - Kolom NO: Digunakan untuk menunjukan nomor urut.
 - Data perbaikan ditampilkan baris per baris untuk setiap mahasiswa.
 - Data statis di tabel ini mencerminkan apa yang dikembalikan oleh fungsi fetchData() dari kelas mahasiswa.

# 4. Contoh Data Tabel yang Ditampilkan
- Baris Pertama:
    - NO: 1
    - Tanggal Perbaikan: 1-12-2024
    - Keterangan: Remidi
    - Mahasiswa ID: 12345
    - Mata Kuliah ID: 67890
    - Semester ID: 0001
    - Nilai ID: 100
    - Dosen ID: 1000
- Baris kedua:
    - NO: 2
    - Tanggal Perbaikan: 2-12-2024
    - Keterangan: Remidi
    - Mahasiswa ID: 12346
    - Mata Kuliah ID: 67891
    - Semester ID: 0002
    - Nilai ID: 200
    - Dosen ID: 2000
- Begitu seterusnya sampai baris kelima.
# Output
<img width="959" alt="Output perbaikan" src="https://github.com/user-attachments/assets/73e79a60-7b2f-4564-82ad-1636a63e218a">






 
  

