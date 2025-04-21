
# Task Manager API - Go (Golang)

## Deskripsi
Ini adalah aplikasi **Task Manager API** menggunakan bahasa **Go (Golang)**.  
API ini memungkinkan pengguna untuk melakukan operasi CRUD (Create, Read, Update, Delete) terhadap daftar tugas.

Data disimpan **sementara di memory** (slice).

---

## Teknologi yang Digunakan
- **Golang 1.18+**
- **Gin Web Framework** (`github.com/gin-gonic/gin`)
- **UUID Generator** (`github.com/google/uuid`)

---

## Persyaratan
- Go 1.18 atau lebih tinggi
- Git (opsional)

---

## Instalasi dan Menjalankan Project

1. **Clone repository ini**:
   ```bash
   git clone https://github.com/username/task-manager-api-go.git
   cd task-manager-api-go
   ```

2. **Inisialisasi dan install dependencies**:
   ```bash
   go mod init task-manager-api-go
   go mod tidy
   ```

3. **Jalankan aplikasi**:
   ```bash
   go run main.go
   ```

4. **Akses API**:
   - Server berjalan di: `http://localhost:8080`

---

## Struktur Project

```
task-manager-api-go/
├── controllers/
│   └── task_controller.go    # Logika endpoint API
├── models/
│   └── task.go                # Struktur data Task
├── routes/
│   └── routes.go              # Routing endpoint
├── main.go                    # Entry point server
├── go.mod                     # Modul Go
├── go.sum                     # Modul dependencies
└── README.md                  # Dokumentasi project
```

---

## API Endpoints

| Method | Endpoint | Keterangan |
|:-------|:---------|:-----------|
| POST | `/tasks` | Membuat tugas baru |
| GET | `/tasks` | Menampilkan semua tugas |
| GET | `/tasks/:id` | Menampilkan detail tugas berdasarkan ID |
| PUT | `/tasks/:id` | Memperbarui tugas berdasarkan ID |
| DELETE | `/tasks/:id` | Menghapus tugas berdasarkan ID |

---

## Contoh Request & Response

### 1. Tambah Tugas Baru (POST `/tasks`)

**Request Body:**
```json
{
  "title": "Belajar Golang",
  "description": "Mempelajari dasar REST API dengan Go"
}
```

**Response:**
```json
{
  "id": "uuid",
  "title": "Belajar Golang",
  "description": "Mempelajari dasar REST API dengan Go",
  "completed": false,
  "created_at": "timestamp",
  "updated_at": "timestamp"
}
```

---

## Error Handling

- **400 Bad Request**: Input tidak valid (contoh: title kosong)
- **404 Not Found**: ID tugas tidak ditemukan

---

## Testing

Untuk testing manual, gunakan:
- **Postman**
- **cURL**
- **Insomnia**

Contoh dengan curl:
```bash
curl -X POST http://localhost:8080/tasks \
-H "Content-Type: application/json" \
-d '{"title": "Belajar Golang", "description": "Mempelajari REST API"}'
```
