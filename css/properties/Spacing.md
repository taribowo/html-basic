# margin & padding

Properti `margin` mengatur penjarakan suatu elemen HTML dengan elemen lainnya. Sementara itu `padding` mengatur penjarakan elemen _child_ terhadap batas-batas elemen _parent_-nya. Kedua properti ini juga direpresentasikan dengan tipe data [\<length>](https://developer.mozilla.org/en-US/docs/Web/CSS/length)

1. `margin`
   ```html
   <div style="margin-bottom: 10px">TES 1</div>
   <!-- akan ada jarak vertikal sejauh 10 pixel dari teks "TES 1" ke teks "TES 2" -->
   <div>TES 2</div>
   ```
2. Padding
   ```html
   <div>TES 1</div>
   <div style="padding-left: 10px; border: 1px solid black">TES 2</div>
   <!-- teks "TES 2" akan berjarak 10 pixel dari tepi border-nya -->
   ```
