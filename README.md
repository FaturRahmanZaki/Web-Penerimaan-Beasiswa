# Web Penerimaan Beasiswa

Aplikasi **Web Penerimaan Beasiswa** ini dirancang untuk membantu proses pendaftaran beasiswa, baik dari sisi **admin** maupun **user**. Dengan menggunakan **PHP** dan **MySQL**, aplikasi ini memungkinkan **admin** untuk mengelola data pendaftaran, sementara **user** dapat mengajukan permohonan beasiswa secara online.

## 🎯 Fitur Utama

### Untuk **Admin**:
- **Login Admin**: Admin dapat mengakses dashboard dengan login menggunakan username dan password yang telah ditentukan.
- **Manajemen Pendaftaran**: Admin dapat melihat, mengedit, dan menghapus data pendaftaran beasiswa yang diajukan oleh user.
- **Manajemen Beasiswa**: Admin dapat menambahkan, mengedit, dan menghapus informasi beasiswa yang tersedia untuk pendaftaran.

### Untuk **User**:
- **Pendaftaran Beasiswa**: User dapat mendaftar untuk berbagai jenis beasiswa yang tersedia.
- **Melihat Status Pendaftaran**: User dapat melihat status pendaftaran beasiswa yang telah mereka ajukan.
  
## 🛠️ Teknologi yang Digunakan

- **Frontend**: 
  - HTML5
  - CSS3
  - Bootstrap 5
- **Backend**:
  - PHP 7.x atau lebih tinggi
  - MySQL
- **Other Tools**:
  - XAMPP atau LAMP sebagai server lokal

## 🚀 Instalasi dan Pengaturan

1. **Clone Repository**:
   - Pertama, clone repositori ini ke dalam folder lokal:
     ```bash
     git clone https://github.com/username/web-penerimaan-beasiswa.git
     ```

2. **Set Up Database**:
   - Buat database baru di MySQL, misalnya `db_beasiswa`.
   - Jalankan script SQL untuk membuat tabel-tabel yang dibutuhkan (biasanya terdapat di dalam file `database.sql` di repositori ini).

3. **Konfigurasi Koneksi Database**:
   - Sesuaikan konfigurasi koneksi database di file `config/database.php` dengan pengaturan MySQL lokal kamu:
     ```php
     <?php
     $servername = "localhost";
     $username = "root";
     $password = "";
     $dbname = "db_beasiswa";

     // Create connection
     $conn = new mysqli($servername, $username, $password, $dbname);

     // Check connection
     if ($conn->connect_error) {
         die("Connection failed: " . $conn->connect_error);
     }
     ?>
     ```

4. **Jalankan Server Lokal**:
   - Gunakan XAMPP atau LAMP untuk menjalankan server lokal.
   - Akses aplikasi dengan membuka browser dan pergi ke `http://localhost/web-penerimaan-beasiswa`.

## 🖥️ Demo

Tampilan antarmuka aplikasi menggunakan **Bootstrap 5** untuk desain yang responsif dan modern:

- **Halaman Admin**:
  - Dashboard admin untuk mengelola pendaftaran beasiswa.
  - Formulir untuk menambah dan mengedit beasiswa.

- **Halaman User**:
  - Formulir pendaftaran beasiswa untuk user.
  - Tampilan status pendaftaran yang diajukan oleh user.

## 📈 Fitur Tambahan yang Akan Datang

- **Notifikasi Email**: Kirim notifikasi email kepada user ketika status pendaftaran beasiswa berubah.
- **Autentikasi Pengguna**: Implementasi autentikasi menggunakan sesi atau JWT untuk meningkatkan keamanan.

## 🔧 Kontribusi

1. Fork repositori ini.
2. Buat branch baru untuk fitur atau perbaikan.
3. Commit perubahan yang telah kamu buat.
4. Kirim pull request ke repositori utama.

## 📄 Lisensi

MIT License. Lihat file [LICENSE](LICENSE) untuk detail lebih lanjut.

---

Terima kasih telah mengunjungi proyek ini! Jika ada pertanyaan atau saran, silakan buka **Issues** atau kirim **Pull Request** untuk kontribusi.
