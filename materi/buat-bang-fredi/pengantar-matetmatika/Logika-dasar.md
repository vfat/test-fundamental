Baik! Berikut adalah versi **yang lebih sederhana dan mudah dipahami** dari **Modul 1: Logika Dasar**, ditujukan untuk siswa pemula (awam), misalnya pelajar SMA awal atau mahasiswa tahun pertama yang belum akrab dengan matematika formal.

---

# 📘 Modul 1: Logika Dasar

---

## 🎯 Tujuan Modul

Setelah mempelajari modul ini, kamu akan bisa:

* Menjelaskan apa itu logika dalam matematika.
* Membedakan mana yang disebut pernyataan logika.
* Memahami apa itu benar dan salah dalam logika.
* Menggunakan tanda-tanda logika seperti “dan”, “atau”, “jika… maka…”.
* Membuat dan membaca tabel kebenaran.
* Mengenali bentuk argumen logis sederhana.

---

## 📌 1.1 Apa itu Logika?

**Logika** adalah cara berpikir secara benar dan masuk akal. Dalam matematika, logika dipakai untuk menyusun kalimat, membuat kesimpulan, dan membuktikan sesuatu.

Contoh kehidupan sehari-hari:

> Kalau hujan, maka saya membawa payung.

Kalimat itu punya aturan: ada syarat (hujan) dan ada akibat (bawa payung). Itulah logika.

---

## 🗣️ 1.2 Pernyataan Logika

**Pernyataan logika** adalah kalimat yang bisa dinilai **benar** (B) atau **salah** (S), tapi tidak bisa keduanya sekaligus.

| Kalimat                           | Pernyataan logika? | Alasan                             |
| --------------------------------- | ------------------ | ---------------------------------- |
| 3 adalah bilangan ganjil          | ✅ Ya               | Bisa dicek benar atau salah        |
| Tolong tutup pintunya!            | ❌ Tidak            | Itu perintah, bukan pernyataan     |
| Jakarta adalah ibu kota Indonesia | ✅ Ya               | Nilai kebenarannya bisa ditentukan |

---

## 🔢 1.3 Tanda-tanda Logika

| Simbol | Nama        | Artinya                   | Contoh                                              |
| ------ | ----------- | ------------------------- | --------------------------------------------------- |
| ¬P     | Negasi      | "Bukan P"                 | Jika P = "Hari cerah", maka ¬P = "Hari tidak cerah" |
| P ∧ Q  | Dan         | Kedua pernyataan benar    | "Hari cerah **dan** saya senang"                    |
| P ∨ Q  | Atau        | Salah satu benar          | "Saya belajar **atau** saya bermain"                |
| P → Q  | Implikasi   | Jika P maka Q             | "Jika saya belajar, maka saya lulus"                |
| P ↔ Q  | Biimplikasi | P dan Q saling tergantung | "Saya datang **jika dan hanya jika** kamu datang"   |

---

## ✅ 1.4 Tabel Kebenaran

Tabel ini menunjukkan semua kemungkinan benar (B) atau salah (S) dari dua pernyataan.

Contoh:
**P** = Saya belajar
**Q** = Saya lulus

| P | Q | P ∧ Q | P ∨ Q | P → Q | P ↔ Q |
| - | - | ----- | ----- | ----- | ----- |
| B | B | B     | B     | B     | B     |
| B | S | S     | B     | **S** | S     |
| S | B | S     | B     | B     | S     |
| S | S | S     | S     | B     | B     |

📝 Catatan:

* **P → Q (Jika P maka Q)** hanya salah kalau P benar tapi Q salah.

---

## 🔄 1.5 Bentuk-Bentuk Implikasi

Kalimat:

> Jika saya belajar (P), maka saya lulus (Q).

Dari situ kita bisa buat:

| Nama         | Bentuk  | Arti                                |
| ------------ | ------- | ----------------------------------- |
| Implikasi    | P → Q   | Jika belajar maka lulus             |
| Konvers      | Q → P   | Jika lulus maka belajar             |
| Invers       | ¬P → ¬Q | Jika tidak belajar maka tidak lulus |
| Kontraposisi | ¬Q → ¬P | Jika tidak lulus maka tidak belajar |

Dari keempat bentuk ini, **implikasi dan kontraposisi** punya arti yang setara.

---

## ⚖️ 1.6 Aturan-aturan Logika

Kita bisa menyederhanakan pernyataan logika pakai aturan ini:

* **Negasi Ganda:** ¬(¬P) = P
* **De Morgan:**

  * ¬(P ∧ Q) = ¬P ∨ ¬Q
  * ¬(P ∨ Q) = ¬P ∧ ¬Q
* **Distribusi:**

  * P ∧ (Q ∨ R) = (P ∧ Q) ∨ (P ∧ R)

Contoh:

> ¬(Saya belajar dan saya bermain) = Saya tidak belajar atau saya tidak bermain

---

## 🧠 1.7 Argumen dan Kesimpulan

Contoh argumen:

1. Jika saya rajin (P), maka saya pintar (Q)
2. Saya rajin (P)
3. Maka saya pintar (Q) ✅

Ini disebut **Modus Ponens**:
P → Q, P → ∴ Q (Kesimpulan yang sah)

Contoh lain:

1. Jika P maka Q
2. Q tidak benar (¬Q)
3. Maka P tidak benar (¬P) ✅
   Disebut **Modus Tollens**

---

## 📝 Latihan

1. Kalimat berikut pernyataan logika atau bukan?

   * "Bulan itu indah."
   * "1 + 1 = 2"
   * "Tutup pintunya sekarang!"

2. Ubah ke bentuk simbol:

   * "Jika saya lapar maka saya makan."

3. Tentukan nilai kebenaran:

   * P = benar, Q = salah
     Hitung P ∧ Q, P ∨ Q, P → Q

4. Ubah ke bentuk konvers, invers, dan kontraposisi:

   * "Jika kamu datang, maka saya senang."

---

## 📌 Kesimpulan Modul

* Logika membantu kita berpikir benar dan sistematis.
* Kita belajar mengenali pernyataan, menggunakan simbol logika, dan membuat kesimpulan.
* Semua ini adalah dasar untuk pembuktian dan pemahaman matematika tingkat lanjut.

---

## 📎 Bonus: Ringkasan Simbol

| Simbol | Artinya                 |
| ------ | ----------------------- |
| ¬P     | Bukan P                 |
| P ∧ Q  | P dan Q                 |
| P ∨ Q  | P atau Q                |
| P → Q  | Jika P maka Q           |
| P ↔ Q  | P jika dan hanya jika Q |

---

Kalau kamu mau, saya bisa bantu:

* Membuat versi **Google Docs / PDF**
* Menambahkan **ilustrasi** atau **animasi logika**
* Membuat **kuis interaktif online**

Lanjut ke Modul 2: **Teori Himpunan**?
