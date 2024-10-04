# Laporan Praktikum Implementasi MVC, Cookies, dan Sessions dengan PHP
### 1. Pendahuluan
Praktikum ini dilaksanakan untuk mempelajari dan mengimplementasikan konsep Model-View-Controller (MVC) dalam pengembangan aplikasi web menggunakan PHP. Selain itu, praktikum ini juga mencakup penggunaan cookies dan sessions untuk manajemen state aplikasi, serta pembuatan sistem CRUD (Create, Read, Update, Delete) untuk pengelolaan data barang.

#### 1.2 Tujuan
- Memahami dan mengimplementasikan arsitektur MVC dalam pengembangan web
- Mempelajari penggunaan cookies dan sessions untuk manajemen state aplikasi
- Mengembangkan sistem CRUD untuk pengelolaan data barang
- Memahami konsep routing dalam aplikasi web

### 2. Dasar Teori
#### 2.1 Model-View-Controller (MVC)
MVC adalah pola arsitektur pengembangan software yang memisahkan aplikasi menjadi tiga komponen utama:

- Model: Menangani logika data dan interaksi dengan database
- View: Menangani tampilan atau antarmuka pengguna
- Controller: Menangani logika aplikasi dan menjadi penghubung antara Model dan View

#### 2.2 Cookies dan Sessions
- Cookies: Data yang disimpan di sisi client (browser)
- Sessions: Data yang disimpan di sisi server untuk tracking informasi user

### 3. Implementasi
#### 3.1 Struktur Proyek
   #### ![image](https://github.com/Jampaaang/Prak.PBW-A/blob/0df5cf997175bbf36f263d3d5041224ebd54f1fe/Tugas5/Image/struktur.jpeg)


#### 3.2 Komponen Utama
#### 3.2.1 Konfigurasi Database
#### phpCopydefine('DB_HOST', 'localhost');
#### define('DB_USER', 'root');
#### define('DB_PASS', '');
#### define('DB_NAME', 'projectmvc');

#### 3.2.2 Struktur Database
sqlCopyCREATE TABLE IF NOT EXISTS `items` (
    `id` int(11) NOT NULL AUTO_INCREMENT,
    `nama` varchar(255) NOT NULL,
    `stok` int(11) NOT NULL,
    `harga` decimal(15,2) NOT NULL,
    PRIMARY KEY (`id`)
);
#### 3.3 Fitur-fitur Aplikasi
#### 3.3.1 Sistem Autentikasi
- Implementasi login menggunakan sessions
- Validasi user dengan username dan password
- Proteksi halaman admin

#### 3.3.2 Manajemen Barang (CRUD)
- Tambah barang baru
- Lihat daftar barang
- Edit informasi barang
- Hapus barang

### 4. Hasil dan Pembahasan
#### 4.1 Implementasi MVC
Implementasi MVC dalam proyek ini memisahkan dengan jelas antara:

- Model: Menangani operasi database untuk tabel items
- View: Menampilkan form login, daftar barang, dan form tambah/edit
- Controller: Menangani logika routing dan proses data

#### 4.2 Manajemen State
Sessions digunakan untuk menyimpan status login user
Implementasi middleware untuk mengecek status login pada halaman admin

#### 4.3 Sistem CRUD
Sistem CRUD diimplementasikan dengan fitur:

- Create: Form tambah barang dengan validasi input
- Read: Tampilan daftar barang dalam bentuk tabel
- Update: Form edit barang dengan data yang telah ada
- Delete: Konfirmasi penghapusan data barang

### 5. Kesimpulan dan Saran
#### 5.1 Kesimpulan
Implementasi MVC membantu dalam organisasi kode dan pemeliharaan aplikasi
Penggunaan sessions efektif untuk manajemen autentikasi
Sistem CRUD berhasil diimplementasikan dengan baik untuk pengelolaan data barang



### AKHIR LAPORAN

## Screenshot

### Halaman Home

![Halaman Home](https://github.com/Jampaaang/Prak.PBW-A/blob/9faba112fd8bac26acf870e714bb57807c8d14d9/Tugas5/Image/Halaman%20Home.jpeg)

### Form Login

![Halaman Login](https://github.com/Jampaaang/Prak.PBW-A/blob/fb1c7329cda52f7ebf74b274684e7186e4537ddb/Tugas5/Image/Halaman%20Login.jpeg)

### Halaman Admin

![Halaman Admin](https://github.com/Jampaaang/Prak.PBW-A/blob/091813fdb89b72c0c61bd7b32054236dad65c2fe/Tugas5/Image/Halaman%20Admin.jpeg)

### Tambah Barang

![Tambah Barang](https://github.com/Jampaaang/Prak.PBW-A/blob/46942f59fc726c0de82dff9e1c68d84b3543eff2/Tugas5/Image/Halaman%20Tambah%20Barang.jpeg)

### Edit Barang

![Edit Barang](https://github.com/Jampaaang/Prak.PBW-A/blob/99a6199226d12699136e5c8f32fc63508e413b79/Tugas5/Image/Halaman%20Edit.jpeg)

## Kontribusi

Dibuat oleh [Jati Rahmatulloh - 4522210039].

## Lisensi

Projek ini dilisensikan di bawah [MIT License](LICENSE).

