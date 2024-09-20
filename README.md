# Tugas-2-Praktikum-Pemrograman-Web-2
# A. koneksi1.php
# Coding koneksi1.php
<img width="400" alt="Koneksi" src="https://github.com/user-attachments/assets/4a1a2581-3ff9-4495-948f-c4ab3cc3ccde">

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
- (<h1>): Judul halaman berisi teks "Data Mahasiswa" dan ditampilkan di tengah halaman dengan kelas Bootstrap (text-center) untuk mengatur posisi tengah secara horizontal.
# 4. Tabel untuk Menampilkan Data
- Struktur Tabel:
  A. Bagian utama dari HTML adalah tabel yang dirancang untuk menampilkan data mahasiswa.
  
  B. Ada dua bagian penting dari tabel:
     1. (<thead>): Bagian kepala tabel (header) berisi judul kolom seperti "NO", "NIM", Nama Mahasiswa", "Alamat", "Email", dan "No Telp".
     2. (<tbody>
  

