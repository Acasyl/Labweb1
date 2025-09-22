

## Penjelasan Struktur Kode

---

###  Penjelasan Struktur Kode

1. **Deklarasi Dokumen**

   ```html
   <!DOCTYPE html>
   <html>
   ```

   → Menandakan bahwa dokumen ini adalah **HTML5**.

2. **Bagian `<head>`**

   ```html
   <head>
       <title>Tag HTML Dasar</title>
       <meta charset="UTF-8">
   </head>
   ```

   * `<title>` : Menentukan judul tab browser.
   * `<meta charset="UTF-8">` : Supaya teks mendukung karakter Unicode (huruf, simbol, dll).

3. **Bagian `<body>`**

   * **Navigasi**

     ```html
     <nav> 
         <a href="lab1_tag_dasar.html">Dasar HTML</a> 
         <a href="lab1_halaman2.html">Halaman 2</a> 
         <a href="http://www.google.com">Halaman Web Eksternal Google</a> 
     </nav> 
     <hr>
     ```

      Membuat menu navigasi dengan link ke halaman internal dan eksternal, lalu dipisahkan dengan garis `<hr>`.

   * **Identitas Mahasiswa**

     ```html
     <h1>Belajar Dasar HTML</h1>
     <p> Nama: Syalsha Putri Ichwani</p>
     <p> NIM: 312410209</p>
     <p> Kelas: TI.24.A2</p>
     ```

      Menggunakan heading `<h1>` untuk judul utama, lalu `<p>` untuk paragraf identitas.

   * **Paragraf dengan format teks**

     ```html
     <p> 
         Kami sedang belajar <mark>HTML dasar</mark>, pada mata kuliah 
         <b>Pemrograman Web</b> di Prodi <i>Teknik Informatika</i> 
         <a href="https://www.pelitabangsa.ac.id">Universitas Pelita Bangsa</a>. 
         ...
     </p>
     ```

      Menampilkan teks dengan format:

     * `<mark>` → memberi highlight.
     * `<b>` → cetak tebal.
     * `<i>` → cetak miring.
     * `<a>` → hyperlink.

   * **Subjudul dan Paragraf**

     ```html
     <h2>Paragraf pada HTML</h2>
     <p>Ini merupakan sebuah paragraf ...</p>
     ```

      `<h2>` untuk subjudul, `<p>` untuk isi paragraf.

   * **Subjudul + Gambar**

     ```html
     <h3>UNIVERSITAS PELITA BANGSA </h3>
     <img src="Logo-Universitas-Pelita-Bangsa.png" width="300" alt="Logo Universitas Pelita Bangsa.png" title="Logo Universitas Pelita Bangsa">
     ```

      `<img>` menampilkan gambar logo, dengan atribut:

     * `src` → lokasi file gambar.
     * `width` → ukuran lebar gambar (300px).
     * `alt` → teks alternatif jika gambar tidak muncul.
     * `title` → teks yang tampil saat mouse diarahkan ke gambar.



---

Mau aku bikinkan versi yang lebih menarik (misalnya ditambahkan warna background dan styling sederhana dengan CSS), atau tetap fokus pada **HTML murni** dulu?


---




## Jawaban Pertanyaan

### 1. Lakukan perubahan pada kode sesuai dengan keinginan anda, amati perubahannya. Adakah error ketika terjadi kesalahan penulisan tag?
Jawab :

Jika ada kesalahan penulisan tag HTML (misalnya `<p>` ditulis `<pp>`), browser tidak akan menampilkan error secara langsung, tetapi elemen tidak akan berfungsi sebagaimana mestinya.  
* Contoh: `<pp>Ini teks</pp>` hanya ditampilkan sebagai teks biasa, bukan paragraf.  
* HTML bersifat toleran (forgiving), jadi tidak muncul pesan error, tetapi hasil tampilan bisa tidak sesuai harapan.

---

### 2. Apa perbedaan dari tag `<p>` dengan tag `<br>`?
Jawab :

- `<p>` digunakan untuk membuat paragraf baru. Saat digunakan, otomatis memberi jarak (spasi) antar paragraf.  
- `<br>` digunakan untuk pindah baris di dalam paragraf tanpa memberi jarak tambahan.

**Contoh:**
```html
<p>Ini paragraf pertama.</p>
<p>Ini paragraf kedua.</p>
```
Hasil: ada jarak antar paragraf.

```html
Ini baris pertama.<br>
Ini baris kedua.
```
Hasil: hanya pindah baris, tanpa jarak tambahan.

---

### 3. Apa perbedaan atribut `title` dan `alt` pada tag `<img>`?
Jawab : alt = teks alternatif, muncul jika gambar gagal dimuat. Juga penting untuk aksesibilitas (screen reader).
title = teks yang muncul ketika kursor diarahkan ke gambar (tooltip).

<img src="Logo-Universitas-Pelita-Bangsa.png" width="300" alt="Logo Universitas Pelita Bangsa.png" title="Logo Universitas Pelita Bangsa">
Jika file Logo.png tidak ada, akan tampil teks Logo Universitas Pelita Bangsa. jika gambar berhasil dimuat, lalu diarahkan mouse, muncul tooltip Logo Universitas Pelita Bangsa.

### 4. Untuk mengatur ukuran gambar, digunakan atribut `width` dan `height`. Agar tampilan gambar proporsional sebaiknya kedua atribut tersebut diisi semua atau tidak?
Jawab :

Tidak harus diisi semua.

* Jika hanya salah satu atribut diisi (misalnya `width`), maka browser otomatis menyesuaikan yang lain agar proporsional.
* Jika keduanya diisi dengan nilai yang tidak sesuai rasio asli gambar, maka gambar bisa tampak gepeng atau melebar.

Jadi sebaiknya cukup isi salah satu (biasanya `width`) agar gambar tetap proporsional.

---
### 5. Pada link tambahkan atribut `target` dengan nilai bervariasi (`_blank`, `_self`, `_top`, `_parent`). Apa yang terjadi pada masing-masing nilai atribut tersebut?
Jawab :
Ini ngatur cara link dibuka:

* `_blank ` → buka di tab/jendela baru.

* `_self ` → buka di tab yang sama (default).

* `_top ` → kalau ada frame/iframe, link langsung buka di jendela penuh (paling luar).

* `_parent ` → buka link di frame induknya. Kalau nggak ada frame, sama aja kayak _self.

Yang paling sering dipakai biasanya  `_blank ` biar linknya kebuka di tab baru.


