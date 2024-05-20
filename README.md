# DwiExpress - Sale of stasiun Tickets

_Place where you can easily order stasiun tickets for your travel plans_

## 📚 About

Platform [`DwiExpress`](https://DwiExpress.my.id/) adalah platform yang digunakan untuk memesan tiket pesawat dalam rencana perjalanan anda.
Kunjungi website `DwiExpress` untuk mengetahui lebih lanjut, Silahkan klik [DwiExpress](https://DwiExpress.my.id/).

## 🧰 Tools

-   PHP versi >8.X.X (Disarankan)
-   Composer
-   DBMS - MySQL

Apabila terjadi `error` saat proses instalasi, silahkan update PHP dan Composer ke versi yang sudah disarankan.

## 💫 Feature

-   Platform dapat memasukkan dan menampilkan data-data pribadi tiap _user_.
-   Platform dapat memberikan kemudahan _user_ dalam memesan tiket yang _available_
-   Platform dapat memberikan fitur percakapan berupa _chat_ antara _user_ dengan _role_ pelanggan dan _admin_
-   Platform dapat memberikan kemudahan bagi _user_ dengan _role admin_ dalam fitur CMS ketika _admin_ berusaha untuk menambahkan, mengubah, atau menghapus data-data terkait Stasiun, Kelas Kursi, Rute Kereta, dan metode penerbangan.
-   Terdapat beberapa menu yang dapat dipilih ketika _user_ sudah _login_ dan memverifikasi akun gmail, yaitu:
    -   _Dashboard_
    -   Daftar Tiket
    -   Buat Pesanan
    -   Riwayat
    -   _Users_
    -   Stasiun
    -   Kelas Kursi
    -   Rute Kereta
    -   Metode Pembayaran

## 📜 Technical

-   Platform menggunakan _framework_ Laravel dalam pengembangan aplikasi berbasis _web_
-   Platform terintegrasi dengan sistem `authentication` dari laravel
-   Total jumlah tabel yang digunakan pada project ini sebanyak 21 tabel
-   Platform menggunakan library `Bootstrap` untuk bagian _front-end_

## 🛠️ Development

### Pre-Requirement

-   Sebelum menggunakan platform, terlebih dahulu perlu menginstall bahasa pemrograman `PHP` dan `Composer`

### Add Remote via GIT

> #### Add Remote to Folder - [GIT DwiExpress Link](https://github.com/FikriDean/DwiExpress_final.git)
>
> Jalankan perintah git untuk menyalin project ke local system

```sh
git remote add talent https://github.com/FikriDean/DwiExpress_final.git
```

### Download Via ZIP

#### Atau download versi ZIP dibawah ini

[Download ZIP DwiExpress](https://github.com/FikriDean/DwiExpress_final/archive/refs/heads/main.zip)

### DwiExpress Project Setup

#### Create `.env` File

-   Jika belum terdapat file .env pada projek, Gunakan file .env.example untuk membuat file `.env` baru. Silahkan atur sesuai keperluan.

```sh
cp .env.example .env
```

#### `.env` File Configuration

-   Konfigurasi Database di file `.env`

```sh
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=DwiExpress
DB_USERNAME=root
DB_PASSWORD=password
```

-   Konfigurasi `APP` di file `.env` (Opsional)

```sh
APP_NAME=DwiExpress
APP_ENV=local
APP_KEY=base64:Oi6PGVLIZlDebARvU6HyrBT1E3jBWyH5IfOsgGYnFds=
APP_DEBUG=true
APP_URL=http://127.0.0.1:8000/
```

-   Jalankan perintah `generate key`

```sh
php artisan key:generate
```

#### Make Database

-   Buat `database` dengan nama yang sesuai dengan nama database yang ada di file `.env`.

#### Migration and Database Seeder

-   Gunakan database seeder yang terdapat di project `DwiExpress` ini. Jalankan perintah berikut

```sh
php artisan migrate:fresh --seed
```

#### Run Application

-   Jalankan perintah untuk menjalankan aplikasi di local system

```sh
php artisan serve
```
