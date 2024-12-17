Berikut adalah **panduan lengkap** untuk melakukan **Automation Testing API dengan Postman**. Postman adalah tools populer yang memungkinkan QA Engineer melakukan pengujian manual dan otomatis pada API.

---

# **Panduan Automation Testing API dengan Postman**

## **1. Persiapan Awal**
### **A. Install Postman**
- Download dan instal Postman dari [https://www.postman.com](https://www.postman.com).

### **B. Persiapkan API Endpoint**
- Dapatkan URL endpoint API, metode request (`GET`, `POST`, `PUT`, `DELETE`), dan parameter (body, query, header).

### **C. Buat Postman Workspace**
1. Buka Postman.
2. Buat workspace baru melalui menu **Workspaces > Create Workspace**.
3. Berikan nama workspace, lalu simpan.

---

## **2. Buat Collection untuk API**
Collection di Postman adalah grup dari request API yang dapat dikelompokkan dan dijalankan secara otomatis.

### **Langkah Membuat Collection:**
1. Klik **New** → **Collection**.
2. Berikan nama collection (contoh: *"Automation Testing API"*).
3. Klik **Create**.

---

## **3. Menambahkan Request ke Collection**
1. Klik **New** → **Request**.
2. Pilih metode request: `GET`, `POST`, dll.
3. Masukkan **URL endpoint**.
4. Tambahkan parameter (Query, Header, Body) jika diperlukan:
   - **Params**: Tambahkan parameter URL.
   - **Headers**: Tambahkan authorization dan content-type.
   - **Body**: Tambahkan payload jika menggunakan metode `POST` atau `PUT`.
5. Klik **Save** untuk menyimpan request ke dalam collection.

---

## **4. Menambahkan Script Test pada Postman**
Postman memungkinkan penulisan skrip otomatisasi menggunakan **JavaScript** di tab **Tests**.

### **Contoh Basic Script untuk Verifikasi Response**
1. Buka request yang telah dibuat.
2. Klik tab **Tests** dan tambahkan skrip berikut:

#### **1. Verifikasi Status Code:**
```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

#### **2. Verifikasi Waktu Respons:**
```javascript
pm.test("Response time is less than 1 second", function () {
    pm.expect(pm.response.responseTime).to.be.below(1000);
});
```

#### **3. Verifikasi Field dalam Body Response:**
```javascript
pm.test("Response contains expected field", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData).to.have.property("data");
    pm.expect(jsonData.data[0]).to.have.property("algochart", 0);
});
```

#### **4. Verifikasi Header Response:**
```javascript
pm.test("Content-Type is application/json", function () {
    pm.response.to.have.header("Content-Type", "application/json");
});
```

3. Klik **Save** setelah menambahkan script.

---

## **5. Menjalankan Automation Test dengan Collection Runner**
Collection Runner memungkinkan Anda menjalankan semua request dalam collection secara otomatis.

### **Langkah Menjalankan Collection Runner:**
1. Klik **Runner** di sidebar kiri bawah.
2. Pilih **Collection** yang ingin dijalankan.
3. Pilih environment (jika menggunakan variable).
4. Klik **Run Collection**.

### **Parameter di Collection Runner:**
- Iterations: Berapa kali pengujian dijalankan.
- Delay: Waktu jeda antar request (dalam ms).
- Data File: Gunakan file `JSON` atau `CSV` untuk data-driven testing.

---

## **6. Data-Driven Testing (Opsional)**
Gunakan file `JSON` atau `CSV` untuk menjalankan pengujian dengan berbagai input data.

### **Langkah Data-Driven Testing:**
1. Buat file `data.csv` dengan format:
   ```
   algochart, expected_status
   0, 200
   1, 200
   ```
2. Tambahkan skrip di tab **Tests** untuk mengambil nilai dari data:
```javascript
pm.test("Status Code sesuai ekspektasi", function () {
    const expectedStatus = pm.iterationData.get("expected_status");
    pm.response.to.have.status(parseInt(expectedStatus));
});
```
3. Saat menjalankan **Collection Runner**, unggah file `data.csv` di bagian **Data File**.

---

## **7. Melihat Hasil Test**
1. Setelah koleksi dijalankan, Postman akan menampilkan hasil:
   - Jumlah **Pass** dan **Fail**.
   - Detail log untuk setiap test case.
2. Klik pada request yang gagal untuk melihat detail error.

---

## **8. Export dan Integrasi CI/CD**
Untuk **Continuous Integration/Continuous Deployment** (CI/CD):
1. **Export Collection**:
   - Klik **Collection** → Export → Pilih format JSON.
2. Gunakan Postman CLI seperti **Newman** untuk menjalankan koleksi secara otomatis di pipeline.

### **Jalankan Koleksi Menggunakan Newman:**
- Install Newman:  
   ```bash
   npm install -g newman
   ```
- Jalankan koleksi:  
   ```bash
   newman run collection_name.json
   ```
- Tambahkan ke pipeline CI/CD (contoh: Jenkins, GitHub Actions).

---

## **9. Best Practices dalam Automation Testing API**
1. **Gunakan Variabel**:
   - Gunakan variabel lingkungan untuk URL base atau token.  
     Contoh: `{{base_url}}/brokers/`.
2. **Parameterisasi Data**:
   - Gunakan data file untuk variasi input.
3. **Pisahkan Test Case**:
   - Setiap endpoint API harus memiliki test case terpisah.
4. **Verifikasi Semua Aspek**:
   - Status code, response time, header, dan body response.

---

## **Contoh Kerangka Test Plan di Postman**
| **Item**                | **Deskripsi**                                                                                  |
|-------------------------|-----------------------------------------------------------------------------------------------|
| **Test Case Name**      | Filter Data Broker dengan Operator `eq`                                                       |
| **Tujuan Pengujian**    | Memastikan endpoint GET `/brokers/` dapat memfilter data dengan parameter `algochart = 0`.    |
| **Langkah Pengujian**   | 1. Kirim request GET `/brokers/?filter=algochart:eq:0` <br> 2. Verifikasi response.           |
| **Data Uji**            | Field: `algochart` <br> Nilai: `0`                                                            |
| **Contoh Request**      | ```GET /brokers/?filter=algochart:eq:0```                                                     |
| **Expected Response**   | - Status Code: `200 OK` <br> - Body: Hanya data dengan `algochart = 0`.                       |
| **Kriteria Keberhasilan** | - Status Code `200`. <br> - Data response valid sesuai filter. <br> - Waktu respons < 1 detik. |
| **Hasil Pengujian**     | **Pass**                                                                                     |
| **Evidence**            | Screenshot hasil Postman Runner dengan status "Passed".                                       |

---

Dengan mengikuti panduan ini, Anda dapat dengan mudah mengotomatiskan pengujian API menggunakan Postman. Jika Anda membutuhkan penjelasan tambahan atau bantuan dalam penerapan, beri tahu saya! 🚀
