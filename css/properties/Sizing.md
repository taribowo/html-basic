# width & height

[Referensi tipe data \<length> pada CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/length)

Properti `width` dan `height`, sesuai artinya, mengatur ukuran dari suatu elemen HTML, `width` mengatur lebar (horizontal) dan `height` mengatur tinggi (vertikal). Nilai keduanya direpresentasikan menggunakan bilangan riil non-negatif dengan satuan tertentu. Penulisan nilai dari atribut `width` dan `height` adalah dengan angka dan langsung diikuti satuannya tanpa spasi. Beberapa satuan yang biasa digunakan adalah

1. `px`  
   Merepresentasikan ukuran lebar dan/atau tinggi dalam satuan pixel dalam layar. Penulisan bilangan tanpa satuan akan secara otomatis diinterpretasikan sebagai pixel
   ```html
   <div style="width: 150px; height: 100;"></div>
   <!-- elemen <div> di atas akan memiliki ukuran lebar 150 pixel dan tinggi 100 pixel -->
   ```
2. `%`  
   Merepresentasikan ukuran lebar dan/atau tinggi dalam persentase ukuran, relatif terhadap lebar dan/atau tinggi yang tersedia pada elemen _parent_
   ```html
   <div id="parent" style="width: 150px; height: 100px;">
     <div id="child" style="width: 50%; height: 25%"></div>
   </div>
   <!-- div #children akan memiliki ukuran lebar 50% dari lebar div #parent, yaitu 50% * 150px = 75px -->
   <!-- div #children akan memiliki ukuran tinggi 25% dari tinggi div #parent, yaitu 25% * 100px = 25px -->
   ```
3. `vw` & `vh`  
   Merepresentasikan ukuran lebar dan/atau dalam persentase ukuran, relatif terhadap lebar dan/atau tinggi _containing block_ awal dari _viewport_. _Viewport_ dalam konteks _web browser_ sendiri adalah keseluruhan bagian dari _web browser_ yang menampilkan halaman _web_, tidak termasuk _address bar_, daftar _tab_, dan _scroll bar_. `vw` merepresentasikan lebar (`width`) viewport, sementara `vh` merepresentasikan tinggi (`height`) viewport
   ```html
   <div style="width: 0.5vh; height: 0.25vw;"></div>
   <!-- elemen <div> di atas akan memiliki ukuran lebar 0.5 * tinggi viewport dan tinggi 0.25 * lebar viewport -->
   ```
4. `rem`  
   Merepresentasikan ukuran lebar dan/atau dalam persentase ukuran, relatif terhadap `font-size` dari elemen _root_, biasanya `<html>`. Jika tidak diubah, nilai _default_ di kebanyakan _browser_ modern adalah `16px`
   ```html
   <div style="width: 20rem; height: 10rem;"></div>
   <!-- dengan asumsi nilai font-size pada <html> tidak diubah, elemen <div> di atas akan memiliki ukuran lebar 20 * 16px = 320 pixel dan tinggi 10 * 16px = 160 pixel -->
   ```
5. `em`  
   Merepresentasikan ukuran lebar dan/atau dalam persentase ukuran, relatif terhadap `font-size` dari elemen itu sendiri
   ```html
   <div style="font-size: 20px; width: 20em; height: 10em;"></div>
   <!-- elemen <div> di atas akan memiliki ukuran lebar 20 * 20px = 400 pixel dan tinggi 10 * 20px = 200 pixel -->
   ```
