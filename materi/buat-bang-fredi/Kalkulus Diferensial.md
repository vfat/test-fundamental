# Materi Lengkap Kalkulus Diferensial

Materi ini mencakup konsep, rumus, dan contoh penting dalam kalkulus diferensial yang sangat berguna untuk siswa SMA, mahasiswa, ataupun siapa saja yang ingin memahami dasar-dasar kalkulus.

---

## 1. Pengantar Kalkulus Diferensial

- **Kalkulus diferensial** mempelajari tentang perubahan (rate of change), kemiringan kurva, dan turunan suatu fungsi.
- Aplikasi: fisika, teknik, ekonomi, biologi, dsb.

---

## 2. Fungsi dan Limit

### a. Fungsi

- Fungsi: suatu aturan yang menghubungkan setiap elemen di domain ke tepat satu elemen di kodomain.
- Notasi: \( f(x) \) atau \( y = f(x) \)
- Contoh: \( f(x) = 2x + 1 \)

### b. Limit

- **Limit**: Nilai yang didekati oleh suatu fungsi saat variabel mendekati nilai tertentu.
- Notasi: \( \lim_{x \to a} f(x) \)
- Contoh:
  \[
  \lim_{x \to 2} (3x + 1) = 3(2) + 1 = 7
  \]
- Aturan limit:
  - Limit penjumlahan: \( \lim_{x \to a} [f(x) + g(x)] = \lim_{x \to a} f(x) + \lim_{x \to a} g(x) \)
  - Limit hasil kali, hasil bagi, dan sebagainya.

---

## 3. Konsep Turunan (Derivatif)

### a. Pengertian Turunan

- Turunan dari fungsi \( f(x) \) di titik \( x = a \) adalah laju perubahan \( f(x) \) terhadap \( x \) di sekitar \( a \).
- Definisi formal:
  \[
  f'(a) = \lim_{h \to 0} \frac{f(a + h) - f(a)}{h}
  \]

### b. Notasi Turunan

- \( f'(x) \), \( \frac{dy}{dx} \), \( y' \)

---

## 4. Aturan Dasar Turunan

### a. Aturan Dasar

- Turunan konstanta: \( (c)' = 0 \)
- Turunan \( x \): \( (x)' = 1 \)
- Turunan \( x^n \): \( (x^n)' = n x^{n-1} \)
- Turunan penjumlahan: \( (f(x) + g(x))' = f'(x) + g'(x) \)
- Turunan selisih: \( (f(x) - g(x))' = f'(x) - g'(x) \)
- Turunan hasil kali: \( (f(x)g(x))' = f'(x)g(x) + f(x)g'(x) \)
- Turunan hasil bagi: \( \left(\frac{f(x)}{g(x)}\right)' = \frac{f'(x)g(x) - f(x)g'(x)}{[g(x)]^2} \)
- Aturan rantai (chain rule): \( (f(g(x)))' = f'(g(x)) \cdot g'(x) \)

### b. Turunan Fungsi Aljabar

- Contoh: \( f(x) = 3x^2 + 2x + 1 \Rightarrow f'(x) = 6x + 2 \)

### c. Turunan Fungsi Trigonometri

- \( (\sin x)' = \cos x \)
- \( (\cos x)' = -\sin x \)
- \( (\tan x)' = \sec^2 x \)
- \( (\cot x)' = -\csc^2 x \)
- \( (\sec x)' = \sec x \tan x \)
- \( (\csc x)' = -\csc x \cot x \)

### d. Turunan Fungsi Eksponensial dan Logaritma

- \( (e^x)' = e^x \)
- \( (a^x)' = a^x \ln a \)
- \( (\ln x)' = \frac{1}{x} \)
- \( (\log_a x)' = \frac{1}{x \ln a} \)

---

## 5. Turunan Tingkat Tinggi

- Turunan kedua: \( f''(x) = \frac{d^2y}{dx^2} \)
- Turunan ketiga, dst.

---

## 6. Aplikasi Turunan

### a. Gradien dan Garis Singgung

- Gradien garis singgung di titik \( x = a \) adalah \( f'(a) \)
- Persamaan garis singgung di titik \( (a, f(a)) \):
  \[
  y - f(a) = f'(a)(x - a)
  \]

### b. Menentukan Titik Stasioner

- Titik di mana \( f'(x) = 0 \)
- Untuk menentukan maksimum/minimum lokal

### c. Uji Maksimum/Minimum

- Pakai turunan kedua:  
  Jika \( f''(x) > 0 \) → minimum lokal  
  Jika \( f''(x) < 0 \) → maksimum lokal

### d. Masalah Optimasi

- Menentukan nilai maksimum/minimum suatu fungsi dalam konteks masalah nyata (misal: luas maksimum, biaya minimum, dsb.)

### e. Kecepatan dan Percepatan (Fisika)

- Jika \( s(t) \) adalah posisi terhadap waktu \( t \), maka:
  - Kecepatan: \( v(t) = s'(t) \)
  - Percepatan: \( a(t) = v'(t) = s''(t) \)

---

## 7. Contoh Soal dan Pembahasan

### Contoh 1: Turunan Polinomial

Hitung turunan dari \( f(x) = 5x^3 - 2x^2 + 4x - 7 \)

**Jawab:**
\[
f'(x) = 15x^2 - 4x + 4
\]

---

### Contoh 2: Turunan Fungsi Trigonometri

Hitung turunan dari \( y = 2\sin x + 3\cos x \)

**Jawab:**
\[
y' = 2\cos x - 3\sin x
\]

---

### Contoh 3: Garis Singgung Kurva

Tentukan persamaan garis singgung kurva \( y = x^2 - 3x + 2 \) di titik \( x = 1 \).

**Jawab:**
- \( y' = 2x - 3 \)
- Pada \( x = 1 \), \( y' = 2(1) - 3 = -1 \)
- Titik: \( (1, 1^2 - 3(1) + 2) = (1, 0) \)
- Persamaan: \( y - 0 = -1(x - 1) \Rightarrow y = -x + 1 \)

---

### Contoh 4: Titik Stasioner

Tentukan titik stasioner dari \( f(x) = x^3 - 3x^2 + 2 \).

**Jawab:**
- \( f'(x) = 3x^2 - 6x \)
- \( 3x^2 - 6x = 0 \rightarrow x(x-2) = 0 \rightarrow x = 0 \) atau \( x = 2 \)
- Titik stasioner: \( (0,2) \) dan \( (2, -2) \)

---

### Contoh 5: Optimasi

Sebuah persegi panjang memiliki keliling 20 cm. Tentukan dimensi agar luas maksimum.

**Jawab:**
- Keliling: \( 2x + 2y = 20 \rightarrow x + y = 10 \rightarrow y = 10 - x \)
- Luas: \( L = x \cdot y = x(10-x) = 10x - x^2 \)
- Maksimum saat \( L' = 10 - 2x = 0 \rightarrow x = 5 \), maka \( y = 5 \)
- Jadi, bentuk maksimum adalah persegi \( 5 \times 5 \)

---

## 8. Latihan Soal

1. Hitung turunan dari \( f(x) = 4x^4 - 3x^3 + 2x - 8 \)
2. Hitung turunan dari \( y = \sin x \cdot \cos x \)
3. Tentukan persamaan garis singgung dari \( y = x^3 \) di \( x = 2 \)
4. Sebuah kotak tanpa tutup akan dibuat dari selembar karton ukuran \( 30 \times 30 \) cm dengan memotong persegi di keempat sudutnya. Tentukan ukuran potongan agar volume maksimum!
5. Jika \( s(t) = 2t^3 - 5t^2 + 4t \), tentukan kecepatan dan percepatan pada \( t = 2 \).

---

## 9. Referensi

- Purcell & Varberg, Kalkulus
- James Stewart, Calculus
- [Khan Academy - Differential Calculus](https://www.khanacademy.org/math/differential-calculus)
- [Materi Kalkulus di Zenius](https://zenius.net/subject/kalkulus)
- [Materi di Ruangguru](https://www.ruangguru.com/)

---

**Selamat belajar dan jangan lupa berlatih soal!**
