

## Persyaratan
- Go 1.18 atau lebih tinggi
- Git (opsional)

---

## Instalasi dan Menjalankan Project

1. **Clone repository ini**:
   ```bash
   git clone -b it-test/backend https://github.com/vfat/test-fundamental.git
   cd task-manager-api-go
   ```


# 📚 Instruksi Tes Backend Development - Go (Golang)

## 🎯 Tujuan Tes
Mengukur kemampuan Anda dalam:
- Membuat REST API sederhana menggunakan Go
- Menyusun struktur project backend yang rapi
- Menerapkan validasi input dan error handling
- Menulis clean code dan dokumentasi sederhana

---

## 🛠️ Deskripsi Proyek

Buatlah sebuah **Task Manager API** sederhana menggunakan **Golang**.

Aplikasi ini harus memungkinkan pengguna untuk:
- Menambahkan tugas baru
- Melihat semua tugas
- Melihat detail tugas berdasarkan ID
- Memperbarui tugas
- Menghapus tugas

**Data tugas** disimpan **sementara di memory** (gunakan slice atau map).

---

## 🧩 Fitur yang Harus Dibuat

| Method | Endpoint        | Deskripsi |
|:-------|:----------------|:----------|
| POST   | `/tasks`         | Menambahkan tugas baru |
| GET    | `/tasks`         | Melihat semua tugas |
| GET    | `/tasks/:id`     | Melihat detail tugas berdasarkan ID |
| PUT    | `/tasks/:id`     | Memperbarui tugas berdasarkan ID |
| DELETE | `/tasks/:id`     | Menghapus tugas berdasarkan ID |

---

## 📦 Struktur Data Tugas (Task)

```json
{
  "id": "uuid",
  "title": "Judul Tugas",
  "description": "Deskripsi Tugas",
  "completed": false,
  "created_at": "timestamp",
  "updated_at": "timestamp"
}
```

---

## 📌 Persyaratan Teknis

- Gunakan **Go 1.18** atau lebih tinggi.
- Gunakan **Gin Web Framework** (`github.com/gin-gonic/gin`) atau **net/http** bawaan.
- Gunakan UUID untuk ID tugas (`github.com/google/uuid`).
- Validasi wajib: **title** dan **description** harus diisi.
- Response harus dalam format **JSON**.
- Berikan HTTP Status Code yang sesuai untuk setiap response.
- Struktur project harus rapi (contoh: pisahkan controller, model, route).
- Tambahkan minimal dokumentasi endpoint dalam README.

---

## 🎯 Kriteria Penilaian

| Aspek | Detail | Bobot |
|:------|:-------|:-----|
| Struktur Project | Modular dan rapi | 20% |
| Implementasi CRUD | Semua endpoint berjalan | 30% |
| Validasi & Error Handling | Ada dan sesuai | 20% |
| Clean Code | Kode bersih, mudah dibaca | 15% |
| Dokumentasi API | Jelas dan lengkap | 15% |

**Total: 100 poin**

---

## 🎁 Bonus (Opsional)

- Membuat middleware sederhana (contoh: logging request).
- Menambahkan pagination untuk `GET /tasks`.
- Membuat Dockerfile untuk containerization.
- Menulis unit testing sederhana.

---




