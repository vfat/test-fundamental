# 🚀 Tes Web Development - Laravel (Backend + Frontend)

## 🎯 Tujuan Tes

Menilai kemampuan Anda dalam membangun aplikasi web sederhana dengan Laravel, mencakup:

- Struktur backend dan frontend yang rapi
- Penerapan autentikasi (login & register)
- Penggunaan database sesuai skema
- Penerapan validasi form
- Penerapan UI responsif dan interaktif

---

## 📌 Deskripsi Umum

Buatlah sebuah aplikasi **Personal Portfolio Website** dengan fitur-fitur berikut:

### ✅ Fitur Utama

1. **Menampilkan Profil Pribadi**:
   - Nama, foto, dan deskripsi singkat
   - Daftar **skills**
   - Daftar **projects** (minimal 2 item)

2. **Formulir Kontak**:
   - Input nama, email, dan pesan
   - Validasi sisi klien & server (semua field wajib, email valid)
   - Simpan ke database

3. **User Authentication**:
   - Register & Login (gunakan Laravel authentication)
   - Hanya user login yang bisa mengakses halaman admin untuk:
     - Menambahkan/mengubah **skill**
     - Menambahkan/mengubah **project**
     - Melihat pesan dari form kontak

---

## 🧱 Ketentuan Teknis

- Gunakan **Laravel versi terbaru** (Laravel 11.x)
- Gunakan **MySQL / PostgreSQL** untuk database
- Gunakan Blade (boleh pakai Inertia/Vue jika mahir)
- Gunakan Laravel Breeze/Fortify untuk autentikasi (opsional: Jetstream)
- Form kontak harus aman dan tervalidasi
- Boleh gunakan Bootstrap atau Tailwind CSS
- Halaman harus **responsive** (mobile-friendly)
- Struktur folder harus rapi
- Kode harus bersih dan mudah dibaca

---

## 🗃️ Struktur Database yang Digunakan

### Tabel: `users`
| Kolom      | Tipe Data |
|------------|------------|
| id         | INT       |
| name       | VARCHAR    |
| email      | VARCHAR    |
| password   | VARCHAR    |
| created_at | TIMESTAMP  |

### Tabel: `skills`
| Kolom    | Tipe Data |
|----------|-----------|
| id       | INT      |
| user_id  | INT      |
| name     | VARCHAR   |

### Tabel: `projects`
| Kolom      | Tipe Data |
|------------|-----------|
| id         | INT      |
| user_id    | INT      |
| title      | VARCHAR   |
| description| TEXT      |
| link       | TEXT      |
| image_url  | TEXT      |

### Tabel: `contact_messages`
| Kolom      | Tipe Data |
|------------|-----------|
| id         | INT      |
| name       | VARCHAR   |
| email      | VARCHAR   |
| message    | TEXT      |
| created_at | TIMESTAMP |

---

## ✨ Bonus Poin

- Dark mode toggle
- Animasi scroll atau transisi komponen
- Dashboard admin dengan UI terpisah
- Unit test atau feature test
- Dockerize project

---

## ⏱️ Waktu Pengerjaan

Maksimal: **4 jam**

---

## 📤 Cara Menyerahkan

- Upload ke GitHub dan kirimkan link repo
- Pastikan repo public atau berikan akses
- Tambahkan instruksi singkat di README untuk menjalankan proyek
- Atau kirim dalam bentuk `.zip`

---

