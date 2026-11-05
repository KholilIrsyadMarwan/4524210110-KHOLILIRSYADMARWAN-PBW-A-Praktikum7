📘 Laporan Praktikum Pertemuan Ke - 7

🧑‍🎓 Kholil Irsyad Marwan - 4524210110

📚 Book Management System (AuthBook - Multi Role & Category)

Aplikasi manajemen buku, penulis, dan kategori berbasis web dengan multi-role access (Admin, Staff, User) yang dibangun menggunakan Laravel 11 dan Filament v3 Admin Panel untuk Praktikum 7 Pemrograman Berbasis Web.

📋 Daftar Isi

🚀 Instalasi & Penggunaan

📌 Soal & Jawaban Tugas 2

🎯 Tentang Aplikasi

🎯 Tujuan Praktikum

✨ Fitur Utama

🛠️ Tech Stack

🗄️ Struktur Database

📸 Hasil Screenshot Tampilan Aplikasi

🚀 Instalasi & Penggunaan

1. Clone Repository

Buka terminal dan jalankan perintah clone untuk mengunduh repositori:

git clone https://github.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7.git
cd 4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/authbook


2. Install PHP Dependencies

Instal seluruh pustaka PHP yang dibutuhkan (termasuk Filament v3):

composer install


3. Setup Environment (.env)

Salin file .env.example menjadi .env lalu generate application key:

cp .env.example .env
php artisan key:generate


Catatan Konfigurasi Database (SQLite):

Pastikan di dalam file .env variabel database sudah terkonfigurasi ke SQLite:

DB_CONNECTION=sqlite


4. Setup Database & Seeding Data Dummy

Jalankan migrasi database untuk membuat tabel categories, authors, books, dan users, sekaligus mengisi data dummy dan role default:

php artisan migrate:fresh --seed


5. Membuat Account User / Admin Filament

Buat akun pengguna untuk masing-masing role agar bisa menguji hak akses pada Filament Admin Panel:

php artisan make:filament-user


Input data akun:

Admin Role: admin@example.com | Password: password

Staff Role: staff@example.com | Password: password

User Role: user@example.com | Password: password

6. Jalankan Local Development Server

Jalankan server bawaan Laravel:

php artisan serve


📌 Soal & Jawaban Tugas 2

Tugas 2: Implementasi Multi-Role & Advanced Filament (Nilai: 60)

Implementasikan pengembangannya dengan menyusun manajemen Kategori, otorisasi 3 Hak Akses (Admin, Staff, User) menggunakan Laravel Policy, serta pembuktian screenshot untuk setiap role.

💡 Jawaban Bukti Implementasi (Screenshot):
A. Hak Akses Role Admin (Akses Penuh / Full Control)
Dashboard Admin

#### A. Hak Akses Role Admin (Full Control)

1. **Dashboard Admin**  
   ![Dashboard Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/dashbooard_admin.jpeg)

2. **Daftar Buku Admin (Books List)**  
   ![List Books Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/books_list_admin.jpeg)

3. **Detail Informasi Buku (View Book Admin)**  
   ![View Book Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/view_books_admin.jpeg)

4. **Form Edit Buku (Edit Book Admin)**  
   ![Edit Book Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/edit_books_admin.jpeg)

5. **Hapus Data Buku (Delete Book Admin)**  
   ![Delete Book Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/delete_books_admin.jpeg)

6. **Kelola Data Kategori (Category List Admin)**  
   ![Category List Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/category_admin.jpeg)

7. **Form Tambah Kategori (Add Category Admin)**  
   ![Add Category Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/add_category.jpeg)

8. **Form Edit Kategori (Edit Category Admin)**  
   ![Edit Category Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/edit_category_admin.jpeg)

9. **Hapus Data Kategori (Delete Category Admin)**  
   ![Delete Category Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/delete_category_admin.jpeg)

10. **Kelola Data Penulis (Author List Admin)**  
    ![Author List Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/author_admin.jpeg)

11. **Form Tambah Penulis (Add Author Admin)**  
    ![Add Author Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/add_author_admin.jpeg)

12. **Detail Informasi Penulis (View Author Admin)**  
    ![View Author Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/view_author_admin.jpeg)

13. **Form Edit Penulis (Edit Author Admin)**  
    ![Edit Author Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/edit_author_admin.jpeg)

14. **Hapus Data Penulis (Delete Author Admin)**  
    ![Delete Author Admin](https://raw.githubusercontent.com/KholilIrsyadMarwan/4524210110-KHOLILIRSYADMARWAN-PBW-A-Praktikum7/main/screenshot/admin/delete_author_admin.jpeg)

B. Hak Akses Role Staff (Create, Read, Update / Non-Delete)
Dashboard Staff

🔗 Link Gambar: dashbooard_staff.jpeg

Daftar Buku Staff (Books List)

🔗 Link Gambar: books_list_staff.jpeg

Form Tambah Buku (Create Book Staff)

🔗 Link Gambar: create_books_staff.jpeg

Daftar Kategori Staff (Category List)

🔗 Link Gambar: category_staff.jpeg

Form Tambah Kategori (Create Category Staff)

🔗 Link Gambar: create_category_staff.jpeg

Form Edit Kategori (Edit Category Staff)

🔗 Link Gambar: edit_category_staff.jpeg

Daftar Penulis Staff (Author List)

🔗 Link Gambar: author_staff.jpeg

Form Tambah Penulis (Add Author Staff)

🔗 Link Gambar: add_author_staff.jpeg

Detail Penulis (View Author Staff)

🔗 Link Gambar: view_author_staff.jpeg

Pencarian Penulis (Search Author Staff)

🔗 Link Gambar: search_author_staff.jpeg

C. Hak Akses Role User (Read Only)
Daftar Buku User (Books List - Read Only)

🔗 Link Gambar: books_list_user.jpeg

Detail Informasi Buku (View Book User)

🔗 Link Gambar: view_books.jpeg

Daftar Kategori User (Category List - Read Only)

🔗 Link Gambar: category_user.jpeg

Daftar Penulis User (Author List - Read Only)

🔗 Link Gambar: author_user.jpeg

Detail Informasi Penulis (View Author User)

🔗 Link Gambar: view_author_user.jpeg

🎯 Tentang Aplikasi

AuthBook versi lanjutan ini dikembangkan sebagai sistem manajemen pustaka digital yang mendukung Multi-Role Access Control dan pengelolaan entitas Kategori Buku. Aplikasi dibangun menggunakan Laravel 11 dan Filament v3, memungkinkan pengaturan otorisasi bertingkat antara Administrator (Admin), Staff, dan Reguler User.

🎯 Tujuan Praktikum

Memahami pengelolaan Multi-Role User pada Filament v3 Admin Panel.

Mengimplementasikan skema database relasional lanjutan (Category HasMany Book, Author HasMany Book).

Menyiapkan pengisian data otomatis (Data Seeding) untuk entitas Kategori, Penulis, Buku, dan Pengguna berdasarkan Role.

Menerapkan pengaturan izin hak akses terpusat menggunakan Laravel Policy untuk mengamankan tindakan Create, Read, Update, dan Delete (CRUD).

✨ Fitur Utama

✅ Multi-Role Authentication & Authorization - Hak akses terbagi menjadi Admin (Akses Penuh), Staff (Create, Read, Update), dan User (Read Only).

✅ Manajemen Category (Kategori) - Fitur pengelolaan kategori buku relasional.

✅ Manajemen Author (Penulis) - Pengelolaan data penulis buku lengkap dengan relasi buku.

✅ Manajemen Book (Buku) - Katalog buku interaktif dilengkapi relasi Kategori, Penulis, ISBN, Cover, Tahun, dan Status.

✅ Search & Filter Table - Fitur pencarian instan dan filter interaktif pada setiap panel tabel.

✅ Policy-Based Control - Keamanan data diatur ketat via Laravel Authorization Policy.

🛠️ Tech Stack

Backend

Laravel 11.x - PHP Framework

PHP ^8.2 - Programming Language

SQLite - Database Storage

Eloquent ORM - Database Management

Admin Panel & Frontend

Filament v3 - Admin Panel Framework

Tailwind CSS - UI Styling Framework

🗄️ Struktur Database

categories: id, name, slug, timestamps

authors: id, name, timestamps

books: id, isbn, title, category_id, author_id, publisher, year, cover, status, timestamps

users: id, name, email, password, role (Admin/Staff/User), timestamps
