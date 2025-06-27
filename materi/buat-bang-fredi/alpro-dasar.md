# Materi Dasar Algoritma Pemrograman

Materi ini dirancang untuk pemula yang ingin memahami konsep algoritma dan dasar-dasar pemrograman.

---

## 1. Pengertian Algoritma

- **Algoritma** adalah urutan langkah logis, sistematis, dan terstruktur untuk menyelesaikan suatu masalah.
- Algoritma digunakan untuk memecahkan masalah, baik dalam kehidupan sehari-hari maupun dalam dunia pemrograman.
- Contoh algoritma dalam kehidupan sehari-hari: cara membuat mie instan, proses login ke aplikasi, dsb.

---

## 2. Karakteristik Algoritma yang Baik

1. **Jelas dan Tidak Ambigu**: Setiap langkah harus jelas dan hanya memiliki satu interpretasi.
2. **Pasti Berakhir (Finiteness)**: Algoritma harus memiliki akhir, tidak berjalan selamanya.
3. **Efisien (Efficiency)**: Algoritma harus hemat waktu dan sumber daya.
4. **Input dan Output Terdefinisi**: Algoritma memiliki input yang jelas dan menghasilkan output.
5. **Setiap Langkah Dapat Dikerjakan (Effectiveness)**: Setiap instruksi dapat dilakukan dengan sumber daya yang tersedia.

---

## 3. Representasi Algoritma

- **Deskripsi Narasi**: Menulis langkah-langkah secara narasi/kalimat.
- **Flowchart (Diagram Alur)**: Representasi grafis dari langkah-langkah algoritma dengan simbol standar.
- **Pseudocode (Kode Semu)**: Menulis algoritma menyerupai kode, tetapi tidak terikat aturan bahasa pemrograman tertentu.

### Contoh Pseudocode:
```
Input: dua angka, a dan b
Proses: jumlahkan a dan b
Output: hasil penjumlahan
```

### Contoh Flowchart:
- Start → Input a,b → c = a+b → Output c → End

---

## 4. Dasar Pemrograman

### a. Variabel dan Tipe Data

- **Variabel**: Tempat menyimpan data/nilai.
- **Tipe Data**:
  - Integer (bilangan bulat): `int`
  - Float/Double (pecahan): `float`, `double`
  - String (teks): `string`
  - Boolean (benar/salah): `bool`

**Contoh deklarasi:**
```python
# Python
umur = 18           # integer
tinggi = 1.75       # float
nama = "Andi"       # string
lulus = True        # boolean
```

### b. Operator

- **Aritmatika**: `+`, `-`, `*`, `/`, `%`
- **Relasi/Perbandingan**: `==`, `!=`, `<`, `>`, `<=`, `>=`
- **Logika**: `and`, `or`, `not`

---

## 5. Struktur Kontrol

### a. Percabangan (Kondisi)

- Menentukan keputusan berdasarkan kondisi tertentu.
- Bentuk umum: `if`, `if-else`, `if-elif-else`, `switch-case` (tergantung bahasa).

**Contoh:**
```python
nilai = 80
if nilai >= 75:
    print("Lulus")
else:
    print("Tidak Lulus")
```

### b. Perulangan (Looping)

- Mengulang instruksi beberapa kali.
- Tipe utama: `for`, `while`, `do-while` (tergantung bahasa).

**Contoh:**
```python
for i in range(1, 6):
    print(i)  # Akan mencetak 1 hingga 5

# While
jumlah = 5
while jumlah > 0:
    print(jumlah)
    jumlah -= 1
```

---

## 6. Fungsi dan Prosedur

- **Fungsi**: blok kode yang menerima parameter, memproses, dan mengembalikan nilai.
- **Prosedur**: mirip fungsi, tapi tidak mengembalikan nilai (tergantung istilah bahasa pemrograman).

**Contoh Fungsi:**
```python
def tambah(a, b):
    return a + b

hasil = tambah(3, 4)  # hasil = 7
```

**Contoh Prosedur:**
```python
def cetak_halo():
    print("Halo dunia!")
```

---

## 7. Contoh Algoritma Dasar

### a. Penjumlahan Dua Angka
```
1. Input angka a
2. Input angka b
3. jumlah = a + b
4. Output jumlah
```

### b. Mencari Nilai Terbesar dari Dua Angka
```
1. Input angka a
2. Input angka b
3. Jika a > b, maka terbesar = a
   Jika tidak, terbesar = b
4. Output terbesar
```

### c. Menentukan Bilangan Ganjil/Genap
```
1. Input angka n
2. Jika n % 2 == 0, maka output "Genap"
   Jika tidak, output "Ganjil"
```

### d. Menghitung Faktorial
```
1. Input angka n
2. faktorial = 1
3. Untuk i dari 1 sampai n:
      faktorial = faktorial * i
4. Output faktorial
```

### e. Menghitung Rata-rata
```
1. Input jumlah data n
2. total = 0
3. Untuk i dari 1 sampai n:
      Input data
      total = total + data
4. rata = total / n
5. Output rata
```

---

## 8. Studi Kasus Sederhana

### 1. Algoritma Menentukan Kelulusan Siswa
```
1. Input nilai ujian
2. Jika nilai >= 75, output "LULUS"
   Jika tidak, output "TIDAK LULUS"
```

### 2. Algoritma Menghitung Luas Segitiga
```
1. Input alas
2. Input tinggi
3. luas = 0.5 * alas * tinggi
4. Output luas
```

### 3. Algoritma Menampilkan Deret Bilangan 1 hingga N
```
1. Input angka n
2. Untuk i dari 1 sampai n:
      Output i
```

---

## 9. Latihan Soal

1. Buatlah algoritma untuk mencari bilangan terbesar dari tiga angka.
2. Buatlah flowchart untuk menentukan bilangan ganjil/genap.
3. Tulis pseudocode untuk menghitung rata-rata tiga nilai ujian.
4. Buat program sederhana untuk menentukan apakah suatu tahun adalah tahun kabisat.

---

## 10. Tips Belajar Algoritma

- Pahami masalah sebelum menulis kode.
- Buat solusi secara bertahap (step by step).
- Latihan membuat algoritma tanpa komputer (paper coding).
- Pelajari contoh dan latihan dari berbagai sumber.
- Diskusikan solusi dengan teman atau mentor.

---

## 11. Referensi

- [Visualgo.net](https://visualgo.net/)
- [Programiz: Algoritma Pemrograman](https://www.programiz.com/article/algorithm)
- Buku: Dasar-Dasar Algoritma dan Pemrograman, Rinaldi Munir
- [GeeksforGeeks - Algorithms](https://www.geeksforgeeks.org/fundamentals-of-algorithms/)

---

**Selamat belajar! Jangan ragu untuk mencoba membuat dan menguji algoritma sendiri.**
