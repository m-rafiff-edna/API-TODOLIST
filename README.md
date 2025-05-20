# Flutter To-Do List App

Aplikasi To-Do List sederhana menggunakan Flutter yang terhubung ke backend Laravel melalui REST API.

## Fitur

- Menampilkan daftar tugas (to-do) dari backend.
- Menambah tugas baru dengan judul, prioritas, dan tanggal deadline.
- Mengedit tugas yang sudah ada.
- Menghapus tugas.
- Menandai tugas sebagai selesai/belum selesai.
- Fitur pencarian tugas berdasarkan judul.
- Tampilan prioritas tugas dengan warna berbeda (high, medium, low).
- Menampilkan tanggal pembuatan, update, dan deadline tugas.

## Struktur Kode Utama

- **Task**: Model data tugas.
- **TodoListPage**: Halaman utama yang menampilkan daftar tugas dan fitur CRUD.
- **fetchTasks**: Mengambil data tugas dari API.
- **addTask**: Menambah tugas baru ke backend.
- **editTask**: Mengedit data tugas di backend.
- **deleteTask**: Menghapus tugas dari backend.
- **updateTaskStatus**: Mengubah status selesai/belum selesai tugas.
- **showAddDialog / showEditDialog**: Dialog untuk menambah/mengedit tugas.
- **getFilteredTasks**: Filter dan urutkan tugas berdasarkan pencarian dan deadline.

## Cara Menjalankan

1. Pastikan backend Laravel berjalan di `http://127.0.0.1:8000` dan endpoint API sudah sesuai.
2. Jalankan perintah berikut di folder Flutter:
   ```sh
   flutter pub get
   flutter run
   ```
3. Pastikan gambar `images/download.png` tersedia untuk logo aplikasi.

## Koneksi API

Aplikasi ini menggunakan endpoint berikut:
- `GET /api/tasks` – Ambil semua tugas
- `POST /api/tasks` – Tambah tugas baru
- `PUT /api/tasks/{id}` – Edit tugas
- `DELETE /api/tasks/{id}` – Hapus tugas

Pastikan backend Laravel sudah menyediakan endpoint di atas.

---

**Catatan:**  
Kode utama aplikasi dapat dilihat di file [`lib/main.dart`](lib/main.dart).
