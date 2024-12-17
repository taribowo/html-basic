# Selector

[Bacaan Komprehensif](https://web.dev/learn/css/selectors)

Dalam memisahkan _file_ CSS dan HTML, tentunya kita membutuhkan sesuatu yang dapat menghubungkan _style_ mana yang harus diterapkan untuk elemen HTML yang mana. Hal ini dapat kita lakukan dengan menggunakan yang disebut _selector_ CSS. Ada beberapa jenis _selector_ yang bisa digunakan, namun kita akan fokus pada _selector_ yang sering digunakan, yaitu

1. _Class Selector_
2. _ID Selector_
3. _Type Selector_
4. _Attribute Selector_

Selain itu, masih ada beberapa metode kombinasi selektor untuk menarget elemen HTML dengan lebih spesifik, yang bisa dipelajari secara mandiri melalui URL berikut

1. [_Pseudo Class_](https://web.dev/learn/css/selectors#pseudo-classes_and_pseudo-elements)
2. [_Complex Selector_](https://web.dev/learn/css/selectors#complex_selectors)

## Class Selector

_Class selector_ mengasosiasikan _style_ CSS melalui atribut `class` yang ada pada hampir seluruh elemen HTML. Penulisan selektor pada _file_ CSS diawali dengan `.` diikuti dengan nama `class`.

```css
.container {
  . . .
  /*
    seluruh style pada blok ini akan diterapkan kepada seluruh elemen yang memiliki atribut class="container"
  */
}
```

```html
<div class="container"></div>
```

## ID Selector

_ID selector_ mengasosiasikan _style_ CSS melalui atribut `id` yang ada pada hampir seluruh elemen HTML. Penulisan selektor pada _file_ CSS diawali dengan `#` diikuti dengan nama `id`.

```css
#centered-box {
  . . .
  /*
    seluruh style pada blok ini akan diterapkan kepada seluruh elemen yang memiliki atribut id="centered-box"
  */
}
```

```html
<div id="centered-box"></div>
```

## Type Selector

_Type selector_ mengasosiasikan _style_ CSS melalui nama tag elemen HTML. Penulisan selektor pada _file_ CSS langsung menggunakan nama tag

```css
div {
  . . .
  /*
    seluruh style pada blok ini akan diterapkan kepada seluruh elemen <div>
  */
}
```

```html
<div></div>
```

## Attribute Selector

_Attribute selector_ mengasosiasikan _style_ CSS melalui atribut yang dapat kita tentukan sendiri. Penulisan selektor pada _file_ CSS dikurung menggunakan `[]`

```css
[data-type="test"] {
  . . .
  /*
    seluruh style pada blok ini akan diterapkan kepada seluruh elemen yang memiliki atribut data-type="test"
  */
}
```

```html
<div data-type="test"></div>
```
