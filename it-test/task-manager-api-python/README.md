

## Persyaratan
- Python 3.8 atau lebih tinggi
- Pip

---

## Instalasi dan Menjalankan Project

1. **Clone repository ini**:
   ```bash
      git clone -b it-test/backend https://github.com/vfat/test-fundamental.git
      cd task-manager-api-python
   ```




# 📚 Instruksi Tes Backend Development - Python (FastAPI/Flask)

## 🎯 Tujuan Tes
Mengukur kemampuan Anda dalam:
- Membuat REST API sederhana menggunakan Python
- Menyusun struktur project backend yang rapi
- Menerapkan validasi input dan error handling
- Menulis clean code dan dokumentasi sederhana

---

## 🛠️ Deskripsi Proyek

Buatlah sebuah **Task Manager API** sederhana menggunakan **Python**.

Aplikasi ini harus memungkinkan pengguna untuk:
- Menambahkan tugas baru
- Melihat semua tugas
- Melihat detail tugas berdasarkan ID
- Memperbarui tugas
- Menghapus tugas

**Data tugas** disimpan **sementara di memory** (gunakan list atau dictionary).

---

## 🧩 Fitur yang Harus Dibuat

| Method | Endpoint        | Deskripsi |
|:-------|:----------------|:----------|
| POST   | `/tasks`         | Menambahkan tugas baru |
| GET    | `/tasks`         | Melihat semua tugas |
| GET    | `/tasks/{id}`    | Melihat detail tugas berdasarkan ID |
| PUT    | `/tasks/{id}`    | Memperbarui tugas berdasarkan ID |
| DELETE | `/tasks/{id}`    | Menghapus tugas berdasarkan ID |

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

- Gunakan **Python 3.9** atau lebih tinggi.
- Framework yang disarankan:
  - **FastAPI** (direkomendasikan) atau
  - **Flask**
- Gunakan UUID (`uuid` library bawaan) untuk ID tugas.
- Validasi: title dan description harus wajib diisi.
- Semua response dalam format **JSON**.
- HTTP Status Code sesuai (200, 201, 400, 404, dll).
- Struktur project harus rapi (pisahkan model, service, route).
- Tambahkan dokumentasi minimal di README.

---

## 🎯 Kriteria Penilaian

| Aspek | Detail | Bobot |
|:------|:-------|:-----|
| Struktur Project | Modular dan bersih | 20% |
| Implementasi CRUD | Semua endpoint berjalan | 30% |
| Validasi & Error Handling | Ada dan sesuai | 20% |
| Clean Code | Naming, komentar, pemisahan file | 15% |
| Dokumentasi API | Ada dan jelas | 15% |

**Total: 100 poin**

---

## 🎁 Bonus (Opsional)

- Membuat middleware sederhana (contoh: logging request atau error).
- Menambahkan pagination untuk `GET /tasks`.
- Menulis unit test (menggunakan pytest/unittest).
- Deploy sederhana di platform seperti Render/Heroku.

---

## 🚀 Petunjuk Submit

1. Upload project ke GitHub atau GitLab (public atau share akses).
2. Sertakan file `requirements.txt` atau `Pipfile` berisi dependencies.
3. Tambahkan README yang menjelaskan:
   - Cara install dan menjalankan project
   - Struktur project
   - Cara testing API (boleh sertakan contoh cURL atau Postman)

---

## 📦 Contoh Struktur Project (FastAPI)

```
task-manager-api/
├── app/
│   ├── main.py        # Entry point
│   ├── models.py      # Model data Task
│   ├── routes.py      # API routes
│   └── services.py    # Logika bisnis (opsional)
├── requirements.txt
└── README.md
```

