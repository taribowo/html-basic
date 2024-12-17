# Teks
[Bacaan Komprehensif 1 (\<h1>, \<h2>, \<h3>, \<h4>, \<h5>, \<h6>)](https://web.dev/learn/html/headings-and-sections#headings_h1-h6)  
[Bacaan Komprehensif 2 (\<p>)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/p)  
[Bacaan Komprehensif 3 (\<span>)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/span)  

Ada banyak cara untuk merepresentasikan teks pada suatu halaman HTML. Kali ini kita hanya akan membahas 3 saja, yaitu _heading_, paragraf, dan teks _inline_

## Heading
Sesuai namanya, _heading_ mengindikasikan bahwa sebuah teks merupakan judul atau subjudul akan sekelompok elemen dan/atau teks lainnya. Pada dasarnya, standar HTML mempunyai 6 jenis/ukuran _heading_, dari \<h1> s.d. \<h6>, dengan ukuran yang berbeda-beda. \<h1> merupakan yang terbesar, hingga \<h6> yang terkecil.  

FYI, beberapa _library/framework_ CSS seperti [TailwindCSS](https://tailwindcss.com/) menghilangkan _default styling_ dari tag-tag dasar HTML sehingga tidak ada perbedaan antara masing-masing _heading_ ini
```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

## Paragraf
Direpresentasikan melalui tag \<p>, sesuai namanya ia merepresentasikan sebuah paragraf atau kumpulan teks. Secara _default, browser_ akan memisahkan konten dari dua atau lebih tag \<p> selayaknya paragraf dalam artikel
```html
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque et tempus arcu. Vivamus fermentum enim vitae mattis rhoncus. Pellentesque sit amet consectetur ex. Duis eget
  malesuada nulla, non ultricies magna. Proin est enim, interdum imperdiet vulputate vitae, interdum at nisl. Sed aliquam tincidunt sapien sed lobortis. Duis a neque volutpat,
  sagittis augue eu, tristique nisi. Sed tristique vitae nulla a feugiat. Curabitur ipsum libero, dictum id lacus vel, efficitur ultricies erat. Mauris semper elit id massa
  luctus, at rutrum leo elementum. Proin et augue placerat, vestibulum libero a, vulputate enim.
</p>
<p>Paragraf 2</p>
```

## Teks _Inline_
Direpresentasikan melalui tag \<span>, biasanya berfungsi untuk membedakan _styling_ sekelompok teks dari kelompok teks lainnya di dalam suatu kelompok teks yang lebih besar
```html
<p>
  Pada Hari Minggu ku turut Ayah ke kota. <span class="some-class">Naik delman istimewa ku duduk di muka.</span> Di samping Pak Kusir yang sedang bekerja.
</p>
```
