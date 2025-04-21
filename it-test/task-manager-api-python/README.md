
# Task Manager API - Python FastAPI

## Deskripsi
Ini adalah aplikasi **Task Manager API** menggunakan **FastAPI**.  
API ini memungkinkan pengguna untuk mengelola daftar tugas melalui operasi CRUD (Create, Read, Update, Delete).

Semua data tugas disimpan **sementara di memory** (dictionary).

---

## Teknologi yang Digunakan
- **Python 3.8+**
- **FastAPI**
- **Uvicorn** (ASGI server)
- **Pydantic** (Data validation)

---

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





---

## Struktur Project

```
task-manager-api-fastapi/
├── app/
│   ├── main.py          # Entry point aplikasi
│   ├── models.py        # Schema tugas menggunakan Pydantic
│   ├── routes.py        # API endpoint dan routing
│   └── services.py      # Logika manipulasi data
├── run.py               # Alternatif entry point
├── requirements.txt     # Daftar dependencies
└── README.md            # Dokumentasi project
```

---

## API Endpoints

| Method | Endpoint        | Keterangan                  |
|:-------|:-----------------|:----------------------------|
| POST   | `/tasks`          | Membuat tugas baru           |
| GET    | `/tasks`          | Melihat semua tugas          |
| GET    | `/tasks/{task_id}`| Melihat tugas berdasarkan ID |
| PUT    | `/tasks/{task_id}`| Memperbarui tugas berdasarkan ID |
| DELETE | `/tasks/{task_id}`| Menghapus tugas berdasarkan ID |

---

## Contoh Request & Response

### 1. Tambah Tugas Baru (POST `/tasks`)

**Request:**
```json
{
  "title": "Belajar FastAPI",
  "description": "Pelajari cara membuat REST API dengan FastAPI"
}
```

**Response:**
```json
{
  "id": "uuid",
  "title": "Belajar FastAPI",
  "description": "Pelajari cara membuat REST API dengan FastAPI",
  "completed": false,
  "created_at": "timestamp",
  "updated_at": "timestamp"
}
```

---

## Error Handling

- **404 Not Found**: Jika ID tugas tidak ditemukan
- **400 Bad Request**: Jika input tidak valid (misal: title kosong)

---

## Testing (Opsional)

Untuk testing manual, Anda bisa menggunakan:
- **Postman**
- **cURL**
- **Swagger UI**

Contoh curl:
```bash
curl -X POST http://localhost:8000/tasks \
-H "Content-Type: application/json" \
-d '{"title": "Belajar FastAPI", "description": "Membuat REST API"}'
```

---
