# color & background-color

[Referensi tipe data \<color> pada CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)

Sesuai namanya, kedua properti ini mengatur tentang pewarnaan suatu elemen, meskipun di aspek yang berbeda. Properti warna dalam CSS dapat direpresentasikan dalam beberapa cara. Cara yang paling sering kita gunakan adalah:

1. RGB Heksadesimal  
   [Referensi](https://developer.mozilla.org/en-US/docs/Web/CSS/hex-color)

   Metode paling dasar untuk merepresentasikan warna dalam CSS adalah menggunakan sintaks warna [heksadesimal](https://en.wikipedia.org/wiki/Hexadecimal) dalam ruang warna [sRGB](https://en.wikipedia.org/wiki/SRGB).

   Kode heksadesimal sebuah warna dapat direpresentasikan menggunakan 4 sintaks berbeda, yaitu

   - `#RGB` - Sintaks 3 Nilai
   - `#RGBA` - Sintaks 4 Nilai
   - `#RRGGBB` - Sintaks 6 Nilai
   - `#RRGGBBAA` - Sintaks 8 Nilai

   Masing-masing nilai `R`, `G`, `B`, dan `A` dapat diisi menggunakan bilangan heksadesimal (`[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, f]`) dan merepresentasikan warna yang berbeda.

   `R` merepresentasikan warna merah  
   `G` merepresentasikan warna hijau  
   `B` merepresentasikan warna biru  
   `A` merepresentasikan nlai _alpha_ (opsional. Jika tidak disertakan, diasumsikan bernilai `FF`. `00` berarti komponen bersifat 100% transparan, sementara nilai `FF` berarti komponen bersifat 0% transparan)

   Sintaks 3 nilai merupakan penyederhanaan dari sintaks 6 nilai, begitu pula sintaks 4 nilai merupakan penyederhanaan dari sintaks 8 nilai. 1 nilai pada sintaks 3 atau 4 nilai setara dengan nilai tersebut namun berulang pada sintaks 6 atau 8 nilai

   `#0f3 = #00ff33`
   `#c1ca = #cc11ccaa`

   Untuk dapat merepresentasikan warna dengan lebih detail, biasanya sintaks 6 atau 8 nilai yang digunakan, akan tetapi untuk menyederhanakan penulisan, sintaks 3 atau 4 nilai terkadang digunakan. Misalkan untuk penulisan warna putih `#ffffff` dapat dituliskan sebagai `#fff` agar lebih singkat.

   Misalkan kita ingin membuat sebuah elemen `<div>` dengan warna latar merah dan warna teks putih, kita dapat membuatnya seperti contoh berikut

   ```html
   <div style="background-color: #ff0000; color: #fff">Latar Merah Teks Putih</div>
   ```

   Beberapa website yang dapat membantu dalam menentukan kode heksadesimal warna adalah sebagai berikut

   1. [coolors](https://coolors.co/)
   2. [imagecolorpicker](https://imagecolorpicker.com/)

2. _Named Colors_  
   [Referensi](https://developer.mozilla.org/en-US/docs/Web/CSS/named-color)

   Dalam CSS, ada beberapa warna yang diasosiasikan dengan alias/_keyword_ tertentu dan bisa langsung digunakan menggunakan nama warna tersebut. Daftar lengkap warna yang memiliki nama dapat dilihat pada tautan referensi. Contoh pada poin 1 dapat kita tulis ulang menggunakan _named color_ menjadi sebagai berikut

   ```html
   <div style="background-color: red; color: white">Latar Merah Teks Putih</div>
   ```

3. Fungsi RGB
   [Referensi](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/rgb)

   Metode selanjutnya adalah menggunakan fungsi yang sudah ada dalam bahasa CSS, yaitu `rgb()`. Fungsi ini menerima 3 parameter wajib (nilai `R`, `G`, dan `B`, bernilai antara `0` sampai dengan `255`, dipisahkan oleh spasi) dan 1 parameter opsional (nilai `A`, dituliskan dengan didahului oleh simbol `/`, bernilai antara `0` sampai dengan `1`)

   Contoh penggunaan fungsi `rgb()` dalam membuat contoh pada poin sebelumnya adalah sebagai berikut

   ```html
   <div style="background-color: rgb(255 0 0 / 1); color: rgb(255 255 255)">Latar Merah Teks Putih</div>
   ```
