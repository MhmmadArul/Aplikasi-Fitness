# Aplikasi Manajemen Fitness 🏋️‍♂️
![image]({https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white})
&#x20; &#x20;

> Sistem sederhana untuk mengelola member, paket, dan transaksi gym. Dibuat sebagai studi kasus workshop Universitas Pamulang.

## Daftar Isi

- [Fitur](#fitur)
- [Teknologi](#teknologi)
- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Struktur Proyek](#struktur-proyek)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)
- [Tim Pengembang](#tim-pengembang)

## Fitur

- **Sistem Login Admin**: autentikasi berbasis sesi untuk mengamankan dashboard.
- **Dashboard Ringkasan**: statistik cepat tentang total member, paket, dan transaksi.
- **Manajemen Member**: tambah, lihat detail, dan hapus member.
- **Manajemen Paket**: CRUD paket latihan atau berlangganan.
- **Manajemen Transaksi**: pencatatan pembayaran member beserta histori.

## Teknologi

| Layer        | Teknologi   |
| ------------ | ----------- |
| Backend      | PHP 8.x     |
| Database     | MySQL 8.x   |
| Local Server | XAMPP       |
| Front‑end    | HTML5, CSS3 |

## Instalasi

> Contoh instalasi menggunakan Windows & XAMPP. Sesuaikan bila Anda memakai stack berbeda.

1. **Clone repositori**

   ```bash
   git clone https://github.com/username/aplikasi-manajemen-fitness.git
   cd aplikasi-manajemen-fitness
   ```

2. **Siapkan basis data**

   - Buka `phpMyAdmin` melalui `http://localhost/phpmyadmin`.
   - Buat database baru mis. `fitness_db`.
   - Impor berkas `database/fitness_db.sql` yang terdapat di folder `database/`.

3. **Konfigurasi aplikasi**

   - Salin `.env.example` menjadi `.env` (atau buka `config/Database.php`).
   - Ubah kredensial MySQL sesuai konfigurasi XAMPP Anda:
     ```ini
     DB_HOST=127.0.0.1
     DB_USER=root
     DB_PASS=
     DB_NAME=fitness_db
     ```

4. **Jalankan server lokal**

   - Buka XAMPP Control Panel, **Start** Apache & MySQL.
   - Akses aplikasi di browser: `http://localhost/aplikasi-manajemen-fitness`.

5. **Login awal**

   - Username: `admin`
   - Password: `admin123`
     > Segera ubah password melalui menu Profil demi keamanan.

## Penggunaan

- Tambah data member & paket melalui menu navigasi di sidebar.
- Semua transaksi tercatat otomatis ke histori pembayaran dan dapat diunduh sebagai CSV.
- Gunakan fitur pencarian untuk memfilter member/paket.

## Struktur Proyek

```
.
├── app/                # source PHP utama (controller, model, view)
├── config/             # konfigurasi DB & konstanta
├── database/
│   └── fitness_db.sql  # skrip SQL
├── public/             # asset yang di‑serve (CSS, JS, gambar)
└── README.md
```

## Kontribusi

Kontribusi sangat terbuka! Silakan `fork` repo, buat branch feature/bugfix baru, lalu kirim *pull request*.\
Ikuti pedoman commit konvensional dan sertakan deskripsi perubahan yang jelas.

## Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).

## Tim Pengembang

| Nama          | Peran                                      |
| ------------- | ------------------------------------------ |
| Muhammad Arul | Full‑stack Developer / Instruktor Workshop |
| Anda?         | Tambah nama Anda di sini!                  |

