# Materi Dasar Development Web: HTML, CSS, dan JavaScript

Materi ini cocok untuk pemula yang ingin belajar membuat website dari nol menggunakan tiga teknologi utama: **HTML**, **CSS**, dan **JavaScript**.

---

## 1. Pengantar Web Development

- Apa itu website?
- Bagaimana website bekerja? (Client & Server, Browser)
- Tiga pilar utama front-end: HTML, CSS, JavaScript

---

## 2. HTML (HyperText Markup Language)

### a. Pengertian HTML

- Bahasa markup untuk membuat struktur halaman web.

### b. Struktur Dasar HTML

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Judul Halaman</title>
  </head>
  <body>
    <!-- Konten di sini -->
  </body>
</html>
```

### c. Elemen & Tag HTML Penting

- Heading: `<h1>` sampai `<h6>`
- Paragraf: `<p>`
- Link: `<a href="url">Teks</a>`
- Gambar: `<img src="gambar.jpg" alt="Deskripsi">`
- List: `<ul>`, `<ol>`, `<li>`
- Table: `<table>`, `<tr>`, `<td>`, `<th>`
- Form: `<form>`, `<input>`, `<button>`, `<textarea>`, dsb
- Div & Span: `<div>`, `<span>`

### d. Atribut HTML

- Contoh: `src`, `href`, `alt`, `id`, `class`, `style`

### e. Semantic HTML

- `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`

---

## 3. CSS (Cascading Style Sheets)

### a. Pengertian CSS

- Bahasa untuk mengatur tampilan (style) halaman web.

### b. Cara Menyisipkan CSS

- Inline: `<p style="color:red;">Teks</p>`
- Internal: `<style>p { color: red; }</style>`
- Eksternal: `<link rel="stylesheet" href="style.css">`

### c. Selektor CSS

- Tag: `p { ... }`
- Class: `.namaKelas { ... }`
- ID: `#namaId { ... }`
- Kombinasi & Pseudo-class: `a:hover`, `div > p`, dsb

### d. Properti CSS Dasar

- Warna: `color`, `background-color`
- Teks: `font-size`, `font-family`, `font-weight`, `text-align`
- Box Model: `width`, `height`, `margin`, `padding`, `border`
- Layout: `display`, `position`, `float`, `flex`, `grid`
- Gambar: `background-image`, `background-size`
- Transisi & Animasi sederhana

### e. Responsive Design

- Media Query:  
  ```css
  @media (max-width: 600px) {
    body { background: yellow; }
  }
  ```
- Mobile-first

---

## 4. JavaScript

### a. Pengertian JavaScript

- Bahasa pemrograman untuk menambahkan interaktivitas pada website.

### b. Cara Menyisipkan JavaScript

- Inline: `<button onclick="alert('Hello')">Klik</button>`
- Internal: `<script>console.log('Hello');</script>`
- Eksternal: `<script src="script.js"></script>`

### c. Dasar-dasar JavaScript

- Variabel: `let`, `const`, `var`
- Tipe data: String, Number, Boolean, Array, Object
- Operator: `+`, `-`, `*`, `/`, `==`, `===`, `&&`, `||`, dsb
- Kondisi: `if`, `else`, `switch`
- Perulangan: `for`, `while`, `do...while`
- Fungsi: `function namaFungsi() { ... }`, arrow function
- Event: `onclick`, `onchange`, `onmouseover`, dsb

### d. Manipulasi DOM

- Mengambil elemen: `document.getElementById('id')`, `document.querySelector('.class')`
- Mengubah konten: `element.innerHTML = "teks baru"`
- Mengubah style: `element.style.color = "red"`
- Menambah/menghapus elemen: `appendChild`, `removeChild`

### e. Contoh Interaksi Sederhana

```html
<button onclick="ubahTeks()">Klik aku!</button>
<p id="teks">Ini paragraf asli.</p>
<script>
function ubahTeks() {
  document.getElementById("teks").innerHTML = "Teks sudah berubah!";
}
</script>
```

---

## 5. Studi Kasus Mini: Membuat Web Sederhana

- Struktur HTML: Header, Konten, Footer
- Styling dengan CSS: Warna, Layout, Responsive
- Interaktif dengan JavaScript: Tombol, Validasi Form

---

## 6. Tools Pendukung

- Code Editor: VSCode, Sublime Text
- Browser: Chrome, Firefox
- Sumber belajar: MDN Web Docs, freeCodeCamp, w3schools

---

## 7. Tips & Best Practice

- Selalu gunakan semantic HTML
- Pisahkan file HTML, CSS, & JS
- Gunakan class untuk styling, hindari styling langsung di HTML
- Cek tampilan di berbagai perangkat (responsive)
- Selalu tes interaktivitas di browser

---

## 8. Referensi

- [MDN Web Docs](https://developer.mozilla.org/)
- [W3Schools](https://www.w3schools.com/)
- [freeCodeCamp](https://www.freecodecamp.org/)

---

**Selamat belajar!**
