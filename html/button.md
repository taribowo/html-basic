# Button
[Bacaan Komprehensif](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button)

Direpresentasikan oleh tag \<button>, sesuai namanya ia adalah elemen yang di-_render_ sebagai tombol untuk _user_ dapat berinteraksi dengan halaman _web_ yang kita buat.  
Interaktivitas dari elemen ini akan bergantung pada _script_ Javascript yang kita buat

Atribut yang sering digunakan dalam elemen button adalah sebagai berikut

## type
atribut yang menandakan perilaku dari tombol yang dibuat.  
_By default_, jika atribut tidak dituliskan, _browser_ akan mengasumsikan nilai `type="button`. Selain itu, nilai atribut yang sering digunakan adalah `type="submit"` yang dapat berfungsi untuk men-_submit_ \<form> yang membungkus tombol tersebut
```html
<button type="button" onclick="alert('Hello, World!')">Click Me!</button>

<form onsubmit="">
  <button type="submit">Submit Me!</button>
</form>
```

## onclick
Dapat dilihat pada contoh sebelumnya, atribut ini berisikan baris javascript yang akan dipanggil ketika _user_ menekan tombol 
