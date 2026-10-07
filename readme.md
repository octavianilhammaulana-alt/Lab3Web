# Praktikum 3: CSS Dasar - Lab3Web

Praktikum mata kuliah **Pemrograman Web** memahami konsep dasar CSS, aturan penulisan, selector, serta penerapan CSS (Internal, Eksternal, dan Inline) pada dokumen HTML.

## Identitas Mahasiswa
Nama : Octavian Ilham Maulana
NIM : 312510275
Kelas : I251A

## 1. Langkah-Langkah Praktikum & Implementasi

### Langkah 1: Membuat Dokumen HTML Dasar 
Membuat struktur dasar dokumen HTML dengan menyertakan navigasi, elemen header, serta pembungkus dengan ID dan Class selector.

<img src="Screenshoot/code 1.png">  
<img src="Screenshoot/hasil 1.png">  


### Langkah 2: Mendeklarasikan CSS Internal
Menambahkan tag `<style>` pada bagian `<head>` dokumen untuk mengatur gaya dasar seperti font, padding, border, dan warna teks pada elemen `header` dan `h1`.

<img src="Screenshoot/code 2.png">
<img src="Screenshoot/hasil 2.png">


### Langkah 3: Menambahkan Inline CSS
Menambahkan deklarasi inline CSS langsung pada tag paragraf `<p>` untuk mengubah gaya pada baris tertentu secara spesifik.

<img src="Screenshoot/code 3.png">  
<img src="Screenshoot/hasil 3.png">  


### Langkah 4: Membuat CSS Eksternal 
Membuat file CSS terpisah untuk mengatur tata letak navigasi, warna latar belakang, serta efek hover pada menu. File eksternal dihubungkan menggunakan tag `<link>`.

<img src="Screenshoot/code 4.png">  
<img src="Screenshoot/code 4 ke 2.png">  
<img src="Screenshoot/hasil 4.png">  


### Langkah 5: Menambahkan CSS Selector (ID dan Class Selector)
Menggunakan ID Selector (`#intro`, `#intro h1`) dan Class Selector (`.button`) pada file `style_eksternal.css` untuk memberikan gaya spesifik pada elemen kontainer utama dan tombol tautan.

<img src="Screenshoot/code 5.png">  
<img src="Screenshoot/hasil 5.png">  

## 3. Pertanyaan dan Tugas

1. **Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS.**
   *Experiment memindahkan letak text **Hello World** menjadi berada di tengah halaman, menambahkan efek hover pada tag `a` yang memiliki class `.button`
      <img src="Screenshoot/code 6.png">    
      <img src="Screenshoot/hasil 6.png">  

2. **Apa perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}`? Berikan penjelasannya!**
   * *Jawaban:* 
     * `h1 {...}` adalah **Element Selector** yang akanmenerapkan aturan gaya ke **seluruh** tag `h1` di dalam dokumen HTML.
     * `#intro h1 {...}` adalah **Descendant / Combined Selector** yang hanya akan menerapkan aturan gaya pada tag `h1` yang berada **di dalam** elemen yang memiliki ID `intro`. Selector ini memiliki tingkat spesifisitas yang lebih tinggi dibandingkan element selector biasa.

3. **Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!**
   * *Jawaban:* Yang akan ditampilkan dan diprioritaskan adalah **Inline CSS**, kemudian **Internal/Eksternal CSS**. Aturan umum dalam CSS menempatkan *Inline Style* pada prioritas tertinggi karena ditulis langsung pada elemen tersebut. Contoh : 
   
      <img src="Screenshoot/code 7.png">  
      <img src="Screenshoot/code 7 ke 2.png">  
      <img src="Screenshoot/hasil 7.png">  


4. **Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! (`<p id="deklarasi-id" class="deklarasi-class">`)**
   * *Jawaban:* Deklarasi dari **ID Selector** akan lebih diprioritaskan dibandingkan **Class Selector**. Hal ini dikarenakan ID memiliki tingkat spesifisitas (specificity weight) yang jauh lebih tinggi daripada Class dalam hierarki CSS. Contoh :  
   <img src="Screenshoot/code 8.png">  
   <img src="Screenshoot/code 8 ke 2.png">  
   <img src="Screenshoot/hasil 8.png">