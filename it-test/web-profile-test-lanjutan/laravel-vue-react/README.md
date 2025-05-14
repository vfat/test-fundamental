# 🚀 Tes Web Development - Laravel + Vue.js / React.js

## 🎯 Tujuan Tes

Menilai kemampuan Anda dalam membangun aplikasi web modern dengan arsitektur **frontend-backend terpisah**, mencakup:

- RESTful API / Inertia integration
- Implementasi autentikasi user
- CRUD data dinamis (skill & project)
- Validasi input form
- Penggunaan UI framework modern
- Struktur kode yang bersih dan maintainable

---

## 📌 Deskripsi Umum

Buatlah sebuah aplikasi **Personal Portfolio Website** dengan Laravel (versi terbaru) untuk backend dan Vue.js atau React.js untuk frontend.

---

## ✅ Fitur Wajib

### 👤 Public Area (tanpa login)

1. **Tampilan Profil**:
   - Nama, foto profil, deskripsi singkat
   - Daftar **skills**
   - Daftar **projects** (minimal 2)
   - Formulir kontak (nama, email, pesan)
     - Validasi klien & server
     - Tampilkan alert jika gagal atau sukses

---

### 🔒 Admin Area (login required)

2. **Autentikasi**:
   - Register dan Login menggunakan email & password
   - Proteksi halaman admin menggunakan middleware

3. **Dashboard Admin**:
   - Tambah, ubah, hapus skill
   - Tambah, ubah, hapus project
   - Lihat daftar pesan dari form kontak

---

## 🛠️ Ketentuan Teknis

- **Backend**: Laravel versi terbaru (Laravel 11+)
  - Gunakan Laravel Breeze (Inertia.js dengan Vue atau React) **atau** jadikan Laravel sebagai API-only (`laravel new --api`)
- **Frontend**:
  - Pilih salah satu: **Vue.js** atau **React.js**
  - Boleh menggunakan framework UI seperti Tailwind CSS, Bootstrap, MUI, dll.
- Validasi wajib dilakukan di sisi klien dan server
- Responsif (mobile & desktop)
- Struktur file rapi (pisah komponen, services, dll.)
- Kode bersih dan readable

---

## 🗃️ Struktur Database

Gunakan skema ini:

### Tabel: `users`
| Kolom      | Tipe Data |
|------------|------------|
| id         | UUID       |
| name       | VARCHAR    |
| email      | VARCHAR    |
| password   | VARCHAR    |

### Tabel: `skills`
| Kolom    | Tipe Data |
|----------|-----------|
| id       | UUID      |
| user_id  | UUID      |
| name     | VARCHAR   |

### Tabel: `projects`
| Kolom      | Tipe Data |
|------------|-----------|
| id         | UUID      |
| user_id    | UUID      |
| title      | VARCHAR   |
| description| TEXT      |
| link       | TEXT      |
| image_url  | TEXT      |

### Tabel: `contact_messages`
| Kolom      | Tipe Data |
|------------|-----------|
| id         | UUID      |
| name       | VARCHAR   |
| email      | VARCHAR   |
| message    | TEXT      |
| created_at | TIMESTAMP |

---

## 🎁 Bonus Poin

- Implementasi **Dark Mode**
- Animasi scroll atau transisi halus (misal: `Framer Motion` / `Vue Transition`)
- Unit test atau e2e test (misal: `Vitest`, `Cypress`, `PHPUnit`)
- Gunakan Docker
- Upload gambar project (pakai storage Laravel + frontend preview)

---

## ⏱️ Waktu Pengerjaan

**Maksimal: 4 jam**

---

## 📤 Cara Menyerahkan

- Upload ke GitHub atau GitLab dan kirimkan link repo
- Tambahkan instruksi jelas di `README.md` untuk menjalankan backend dan frontend
- Atau kirim file `.zip` beserta file `.env.example`

---


