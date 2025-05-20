# Aplikasi To-Do List CRUD (Flutter + Laravel)

## Deskripsi Aplikasi
Aplikasi **To-Do List** ini adalah aplikasi CRUD (Create, Read, Update, Delete) berbasis **Flutter** sebagai frontend dan **Laravel** sebagai backend API. Aplikasi ini memungkinkan pengguna untuk:
- Menambahkan tugas dengan title, prioritas, dan deadline
- Mengatur tanggal dan jam `created_at` dan `updated_at **sesuai tanggal dan waktu di laptop saat membuat dan mengedit tugaS**
- Mengedit tugas
- Menghapus tugas (otomatis jika dichecklist)
- Menampilkan semua tugas dengan tampilan modern menggunakan Flutter Card

### Halaman Aplikasi
- **Halaman Utama**: Menampilkan daftar semua tugas
- **Form Tambah/Edit**: Input title, prioritas, deadline, created_at, updated_at
- **Checklist**: Menandai tugas selesai dan langsung menghapusnya

### Database
Menggunakan database **MySQL** dengan tabel `tasks` dan field berikut:
- `id`
- `title`
- `priority` (low, medium, high)
- `due_date`
- `is_done`
- `created_at`
- `updated_at`

### API (Laravel)
API berada di folder `/api/` dengan endpoint:
- `GET /api/tasks` — Menampilkan semua tugas
- `POST /api/tasks` — Menambah tugas baru
- `PUT /api/tasks/{id}` — Mengupdate tugas
- `DELETE /api/tasks/{id}` — Menghapus tugas

## Software yang Digunakan
- **Flutter** (versi terbaru)
- **Laravel 10**
- **MySQL**
- **Postman** (untuk testing API)
- **VS Code**
- **Laragon**

---

## Cara Instalasi

### 1. Clone Repository
```bash
git clone https://github.com/Rifai-hub24/todolist
cd todolist

###2. Backend (Laravel)
'''Masuk folder api/

Jalankan:
composer install
cp .env.example .env
php artisan key:generate

Sesuaikan .env:
DB_DATABASE=todo_app
DB_USERNAME=root
DB_PASSWORD= // kosongkan jika tidak pakai password

Jalankan migrasi:

php artisan migrate
php artisan serve

###3. Frontend (Flutter)
Masuk ke folder flutter_app/ (atau lib/ jika semua di main.dart)

Jalankan:
flutter pub get
flutter run

###Cara Menjalankan
Jalankan Laravel API:
php artisan serve

Jalankan Flutter:
flutter run

###Demo Aplikasi

https://github.com/user-attachments/assets/b59c5011-58e4-44da-87a5-f71d24c98f84

Identitas Pembuat
Nama: Muhammad Irfan Rifai
No:21
Kelas:XI RPL2
Sekolah: SMK Negeri 1 Bantul
Jurusan: Rekayasa Perangkat Lunak (RPL)





 

