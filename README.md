

 Penjelasan Struktur Kode

1. Deklarasi Dokumen

   ```html
   <!DOCTYPE html>
   <html>
   ```

   Menandakan bahwa dokumen ini adalah *HTML5*.

2. *Bagian `<head>`*

   ```html
   <head>
       <title>Tag HTML Dasar</title>
       <meta charset="UTF-8">
   </head>
   ```

   * `<title>` : Menentukan judul tab browser.
   * `<meta charset="UTF-8">` : Supaya teks mendukung karakter Unicode (huruf, simbol, dll).

3. *Bagian `<body>`*

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

   * *Identitas Mahasiswa*

     ```html
     <h1>Belajar Dasar HTML</h1>
     <p> Nama: Syalsha Putri Ichwani</p>
     <p> NIM: 312410209</p>
     <p> Kelas: TI.24.A2</p>
     ```

     Menggunakan heading `<h1>` untuk judul utama, lalu `<p>` untuk paragraf identitas.

   * *Paragraf dengan format teks*

     ```html
     <p> 
         Kami sedang belajar <mark>HTML dasar</mark>, pada mata kuliah 
         <b>Pemrograman Web</b> di Prodi <i>Teknik Informatika</i> 
         <a href="https://www.pelitabangsa.ac.id">Universitas Pelita Bangsa</a>. 
         ...
     </p>
     ```

     Menampilkan teks dengan format:

     * `<mark>` : memberi highlight.
     * `<b>` : cetak tebal.
     * `<i>` : cetak miring.
     * `<a>` : hyperlink.

   * *Subjudul dan Paragraf*

     ```html
     <h2>Paragraf pada HTML</h2>
     <p>Ini merupakan sebuah paragraf ...</p>
     ```

      `<h2>` untuk subjudul, `<p>` untuk isi paragraf.

   * *Subjudul + Gambar*

     ```html
     <h3>UNIVERSITAS PELITA BANGSA </h3>
     <img src="Logo-Universitas-Pelita-Bangsa.png" width="300" alt="Logo Universitas Pelita Bangsa.png" title="Logo Universitas Pelita Bangsa">
     

     `<img>` menampilkan gambar logo, dengan atribut:

     * `src` : lokasi file gambar.
     * `width` : ukuran lebar gambar (300px).
     * `alt` : teks alternatif jika gambar tidak muncul.
     * `title` : teks yang tampil saat mouse diarahkan ke gambar.


 *Kesimpulan:*

* File HTML ini sudah sesuai untuk praktikum dasar.
* Struktur `<head>` dan `<body>` rapi.
* Sudah menggunakan tag teks, link, paragraf, heading, dan gambar.

---

