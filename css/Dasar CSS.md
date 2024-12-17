# Dasar-dasar CSS

CSS (_Cascading Style Sheets_) adalah baris kode/_file_ yang berfungsi untuk memberikan bentuk, warna, ukuran, jarak, orientasi, dll kepada elemen-elemen HTML  
Ada 2 cara utama untuk memberikan _style_ kepada elemen HTML, yaitu:

1. _Inline_
2. _File_

## Inline Styling

Metode ini menggunakan atribut `style` yang ada pada hampir semua elemen HTML. Baris kode CSS dituliskan langsung pada masing-masing elemen HTML yang dibuat, oleh karena itu, metode ini disebut _inline styling_

```html
<div style="width: 100px; height: 100px; background-color: red; color: white">Sayur Lodeh + Tempe Goreng</div>
```

## File CSS

Metode ini mengumpulkan seluruh baris kode CSS pada _file-file_ terpisah untuk kemudian di-_load_ sesuai kebutuhan di halaman-halaman terpisah

#### **style.css**

```css
.container {
  display: flex;
  width: 500px;
  height: 500px;
  background-color: red;
  justify-content: center;
  align-items: center;
}

#centered-box {
  display: flex;
  width: 300px;
  height: 300px;
  background-color: cornflowerblue;
}
```

#### **index.html**

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Contoh CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <div id="centered-box"></div>
    </div>
  </body>
</html>
```
