# SKEMA HTML

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

Sejauh ini, skema HTML dasar kita adalah sebagai berikut
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Skema Dasar Halaman HTML</title>
  </head>
  <body>. . .</body>
</html>
```
