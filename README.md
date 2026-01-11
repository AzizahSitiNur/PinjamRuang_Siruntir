## SIRUNTIR - Sistem Informasi Ruang UNTIRTA

SIRUNTIR adalah aplikasi web berbasis **Laravel** untuk mempermudah proses peminjaman ruangan di lingkungan Universitas Sultan Ageng Tirtayasa (UNTIRTA).

> Fokus utama aplikasi ini adalah digitalisasi proses peminjaman ruangan sehingga lebih terstruktur, transparan, dan mudah dipantau baik oleh pengguna biasa maupun admin.

---

## Fitur Utama

- Manajemen user (registrasi, login, role user & admin)
- Manajemen data ruangan (tambah, ubah, hapus, detail ruangan)
- Pengajuan peminjaman ruangan oleh user
- Persetujuan / penolakan peminjaman oleh admin
- Kalender jadwal peminjaman ruangan
- Laporan peminjaman yang dapat diekspor ke format PDF

---

## Teknologi yang Digunakan

- PHP (Laravel)
- MySQL / MariaDB (database)
- Tailwind CSS & Vite (frontend build)

---

## Cara Menjalankan Proyek Secara Lokal

Pastikan sudah terpasang di komputer Anda:

- PHP 8.x
- Composer
- Node.js & npm
- MySQL / MariaDB

### 1. Clone Repository

```bash
git clone https://github.com/USERNAME/Siruntir.git
cd Siruntir
```

> Ganti `USERNAME` dengan username GitHub Anda.

### 2. Install Dependency Backend

```bash
composer install
```

### 3. Install Dependency Frontend

```bash
npm install
```

### 4. Konfigurasi Environment

```bash
cp .env.example .env
```

Lalu sesuaikan konfigurasi database dan pengaturan lain di file `.env`.

### 5. Generate App Key

```bash
php artisan key:generate
```

### 6. Migrasi Database (dan seeder jika diperlukan)

```bash
php artisan migrate --seed
```

### 7. Menjalankan Aplikasi

Jalankan server Laravel:

```bash
php artisan serve
```

Jalankan dev server frontend (jika dibutuhkan):

```bash
npm run dev
```

Setelah itu, buka browser dan akses:

```text
http://127.0.0.1:8000
```

---

## Screenshot & Panduan Singkat

Semua gambar berada di folder `public/screenshots`. Di GitHub, gambar berikut akan otomatis muncul jika folder tersebut ikut dipush.

### Halaman Login
![Tampilan Login](public/screenshots/login.png)
Pengguna akan diarahkan ke halaman login saat pertama kali membuka web.

### Halaman Register
![Tampilan Register](public/screenshots/register.png)
Jika pengguna belum memiliki akun, mereka dapat mendaftar melalui halaman ini.

### Dashboard User
![Tampilan Dashboard User](public/screenshots/dashboard_user.png)
Dashboard berisi ringkasan informasi dan akses cepat ke fitur peminjaman.

### Membuat Peminjaman Ruangan
![Tampilan Membuat Peminjaman Ruangan](public/screenshots/buat_peminjaman.png)
User dapat membuat peminjaman baru melalui halaman **Buat Peminjaman**.

### Daftar Peminjaman User
![Tampilan Daftar Pinjam](public/screenshots/peminjaman_user.png)
Menampilkan daftar ruangan yang sedang atau pernah dipinjam oleh user.

### Kalender Peminjaman
![Kalender](public/screenshots/kalender_user.png)
Jadwal peminjaman ruangan ditampilkan dalam bentuk kalender agar mudah dipantau.

### Dashboard Admin
![Dashboard Admin](public/screenshots/dashboard_admin.png)
Admin yang login akan diarahkan ke dashboard admin untuk memantau seluruh aktivitas peminjaman.

### Daftar Ruangan
![Daftar Ruangan](public/screenshots/daftar_ruangan.png)
Menampilkan seluruh ruangan yang dikelola. Admin dapat menambah, mengubah, atau menghapus ruangan.

### Tambah Ruangan
![Tampilan Tambah Ruangan](public/screenshots/tambah_ruangan.png)
Form untuk menambahkan ruangan baru oleh admin.

### Daftar User
![Daftar User](public/screenshots/daftar_user.png)
Admin dapat melihat daftar user, mengubah profil, serta mengatur role user.

### Tambah User oleh Admin
![Tambah Daftar User](public/screenshots/tambah_user.png)
Admin dapat menambahkan user secara manual melalui halaman ini.

### Daftar Peminjaman (Admin)
![Daftar Peminjaman Pada Halaman Admin](public/screenshots/daftar_peminjaman.png)
Admin dapat melihat daftar pengajuan peminjaman dan memutuskan untuk menyetujui atau menolak permintaan.

### Laporan Peminjaman (PDF)
![Laporan Peminjaman](public/screenshots/laporan_peminjaman.png)
Admin dapat mengekspor laporan peminjaman ke dalam format PDF untuk keperluan dokumentasi.

---

## Lisensi

Tambahkan informasi lisensi proyek Anda di sini (misalnya MIT, proprietary, dsb.).

