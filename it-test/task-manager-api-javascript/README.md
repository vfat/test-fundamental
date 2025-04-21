# Task Manager API - Node.js + Express.js

## Deskripsi
Ini adalah aplikasi **Task Manager API** yang dibuat menggunakan **Node.js** dan **Express.js**. Aplikasi ini memungkinkan pengguna untuk mengelola tugas (task) dengan menyediakan endpoint untuk membuat, membaca, memperbarui, dan menghapus tugas.

## Fitur
- Menambahkan tugas baru
- Melihat daftar semua tugas
- Melihat tugas berdasarkan ID
- Memperbarui tugas berdasarkan ID
- Menghapus tugas berdasarkan ID

## Teknologi yang Digunakan
- **Node.js**
- **Express.js**
- **UUID** (untuk ID unik)
- **Postman** atau **reast api client lain** untuk pengujian API

## Persyaratan
- **Node.js** v14 atau lebih tinggi
- **npm** (atau **yarn**) untuk mengelola dependencies

## Instalasi

1. Clone repositori ini:
   ```bash
   git clone -b it-test/backend https://github.com/vfat/test-fundamental.git
   cd task-manager-api-javascript
   ```

## API Endpoints

### 1. **POST** `/tasks`
Menambahkan tugas baru.

**Request Body:**
```json
{
  "title": "Tugas 1",
  "description": "Deskripsi tugas 1"
}
```

**Response:**
```json
{
  "id": "uuid",
  "title": "Tugas 1",
  "description": "Deskripsi tugas 1",
  "completed": false,
  "createdAt": "timestamp",
  "updatedAt": "timestamp"
}
```

### 2. **GET** `/tasks`
Melihat daftar semua tugas.

**Response:**
```json
[
  {
    "id": "uuid",
    "title": "Tugas 1",
    "description": "Deskripsi tugas 1",
    "completed": false,
    "createdAt": "timestamp",
    "updatedAt": "timestamp"
  }
]
```

### 3. **GET** `/tasks/:id`
Melihat detail tugas berdasarkan ID.

**Response:**
```json
{
  "id": "uuid",
  "title": "Tugas 1",
  "description": "Deskripsi tugas 1",
  "completed": false,
  "createdAt": "timestamp",
  "updatedAt": "timestamp"
}
```

### 4. **PUT** `/tasks/:id`
Memperbarui tugas berdasarkan ID.

**Request Body:**
```json
{
  "title": "Tugas 1 Updated",
  "description": "Deskripsi tugas 1 yang diperbarui",
  "completed": true
}
```

**Response:**
```json
{
  "id": "uuid",
  "title": "Tugas 1 Updated",
  "description": "Deskripsi tugas 1 yang diperbarui",
  "completed": true,
  "createdAt": "timestamp",
  "updatedAt": "timestamp"
}
```

### 5. **DELETE** `/tasks/:id`
Menghapus tugas berdasarkan ID.

**Response:**
```json
{
  "message": "Task with ID {id} deleted successfully."
}
```

## Error Handling
- Jika ID tidak ditemukan, server akan mengembalikan status **404 Not Found**.
- Jika input tidak valid, server akan mengembalikan status **400 Bad Request**.

## Cara Pengujian
Gunakan **Postman** atau **curl** untuk menguji endpoint yang tersedia.

### Contoh Curl:
- **Menambahkan Tugas Baru:**
  ```bash
  curl -X POST http://localhost:3000/tasks \
    -H "Content-Type: application/json" \
    -d '{"title": "Tugas 1", "description": "Deskripsi tugas 1"}'
  ```

- **Melihat Semua Tugas:**
  ```bash
  curl http://localhost:3000/tasks
  ```

## Struktur Folder
```
task-manager-api/
├── controllers/
│   └── tasksController.js        # Menangani logika untuk setiap endpoint
├── routes/
│   └── tasksRoutes.js           # Menangani routing untuk API
├── models/
│   └── taskModel.js             # Menyimpan data tugas di memory
├── server.js                    # File utama untuk memulai server
├── package.json                 # Dependencies dan skrip
└── README.md                    # Dokumentasi API
```
