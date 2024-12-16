# SKEMA HTML
[Bacaan Komprehensif](https://web.dev/learn/html/document-structure)

Berikut adalah skema dasar dari sebuah halaman HTML

```html
<!DOCTYPE html>
<html>
  <head>. . .</head>
  <body>. . .</body>
</html>
```
## \<head>
Berisi metadata dari halaman web  
Yang dianggap sebagai metadata esensial yang harus ada di dalam \<head> biasanya adalah
1. Charset
```html
<meta charset="utf-8" />
```
Tag ini berfungsi untuk memberitahu browser _encoding_ karakter yang digunakan di keseluruhan dokumen HTML sehingga browser dapat me-_render_ karakter-karakter yang ada  

2. Title
```html
<title>Judul Halaman HTML</title>
```
Tag ini berfungsi untuk memberi _title_ pada halaman HTML yang dibuat. _Title_ yang dibuat akan muncul sebagai nama tab di mayoritas browser masa kini

3. Viewport
```html
<meta name="viewport" content="width=device-width" />
```
Tag ini berfungsi untuk memberi kapasitas _responsiveness_ kepada halaman HTML agar browser dapat me-_render_ elemen-elemen pada halaman dengan baik, sesuai dengan layar _device_ yang digunakan

Untuk pelajaran dasar HTML, kita tidak terlalu memperlukan informasi viewport. Tag-tag lainnya pun biasanya akan di-_generate_ secara otomatis nantinya saat kita mulai belajar react jika kita menggunakan tools seperti [Vite](https://vite.dev/)

Selain itu, tag yang biasanya akan kita tambahkan di \<head> adalah \<link>, yang berguna untuk me-_load_ _file-file_ CSS
```html
<link rel="stylesheet" href="style.css" />
```

Sejauh ini, skema HTML dasar kita adalah sebagai berikut
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Dasar-dasar HTML</title>

    <!-- <link rel="stylesheet" href="style.css" /> -->
    <!-- Contoh comment HTML --> 
  </head>
  <body>. . .</body>
</html>
```

## \<body>
Seluruh konten dari halaman web yang kita buat akan ada di dalam tag ini. Isi dari tag ini dapat berupa text mentah maupun elemen HTML lainnya. Selain itu, biasanya \<script> akan diletakkan pada akhir \<body> agar _file-file_ Javascript di-_load_ setelah seluruh elemen di halaman ter-_render_

### \<script>
Tag untuk me-_load_ kode ataupun _file_ Javascript, untuk memberikan interaktivitas pada elemen-elemen HTML di halaman web
```html
<script type="text/javascript">
  console.log("Hello, World!")
</script>
<script type="text/javascript" src="main.js" />
```

Dengan menambahkan konten \<body> dan \<script>, _file_ HTML dasar kita menjadi sebagai berikut
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Dasar-dasar HTML</title>

    <!-- <link rel="stylesheet" href="style.css" /> -->
    <!-- Contoh comment HTML --> 
  </head>
  <body>
    Hello, World!

    <script type="text/javascript">
      console.log("Hello, World!")
    </script>
    <!-- <script type="text/javascript" src="main.js" /> -->
  </body>
</html>
```
