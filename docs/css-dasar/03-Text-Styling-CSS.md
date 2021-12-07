---
title: 03 - Text Styling CSS
---

# Text Styling CSS

Terdapat berbagai cara untuk menghias/memformat/memanipulasi teks pada CSS.

## Text Color

Kita dapat mengatur warna teks dengan menggunakan properti `color` pada CSS.
Properti ini dapat kita isi dengan value berupa hex (`#21E440`), nama (`red`), atau nilai RGB/RGBA/HSL/HSLA (`rgb(255,0,0)`, `hsl(120, 100%, 50%)`, dan lain-lainnya) dari warna yang kita inginkan.

Contoh pengaplikasian :

```css
p {
  color: blue;
}

a {
  color: #ff0000;
}

.muted {
  color: rgb(80, 80, 80);
}
```

## Text Alignment

### Properti `text-align`

Kita dapat mengatur posisi teks apakah di kanan, tengah, kiri, atau rata kanan kiri dengan menggunakan properti `text-align`.
Terdapat 3 jenis value dari properti ini yaitu `left`, `right`, `center`, dan `justified` (rata kanan kiri).

Contoh pengaplikasian :

```css
p {
  text-align: left;
}
```

### Properti `direction` dan `unicode-bidi`

Kita dapat mengatur arah baca teks menggunakan properti `direction` dan `unicode-bidi`.

Contoh pengaplikasian :

```css
p {
  direction: rtl;
  unicode-bidi: bidi-override;
}
```

### Properti `vertical-align`

Kita dapat mengatur posisi teks secara vertikal dengan properti `vertical-align`.
Terdapat beberapa jenis value untuk properti ini :

- `baseline` : Default.
- jarak (`20px`) : Naikkan atau turunkan posisi elemen menyesuaikan jarak yang diberikan.
- persen (`40%`) : Naikkan atau turunkan posisi elemen menyesuaikan persen yang diberikan relatif ke jarak `line-height`.
- `sub` : Turunkan posisi elemen sampai pada posisi subscript.
- `super` : Naikkan posisi elemen sampai pada posisi superscript.
- `top`, `middle`, `bottom` : Atur posisi teks ke atas, tengah, atau bawah.

Contoh pengaplikasian :

```css
img.a {
  vertical-align: baseline;
}

img.b {
  vertical-align: text-top;
}

img.c {
  vertical-align: text-bottom;
}

img.d {
  vertical-align: sub;
}

img.e {
  vertical-align: super;
}
```

## Text Decoration

Kita dapat mengatur dekorasi yang ada pada teks melalui properti `text-decoration`.
Properti ini biasa digunakan untuk menghapus garis bawah pada link.

Contoh penggunaan :

```css
a {
  text-decoration: none;
}
```

## Text Transformation

Kita dapat mengatur transformasi teks dengan menggunakan properti `text-transform`.
Properti ini dapat digunakan untuk mengubah teks menjadi kapital atau huruf kecil seluruhnya, atau juga mengkapitalisasikan huruf pertama dari setiap kata.

Contoh penggunaan :

```css
p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
```

## Text Spacing

### Properti `text-indent`

Kita dapat mengatur indentasi dari suatu teks dengan menggunakan properti `text-indent` dan value yang ditentukan berupa jarak.

Contoh penggunaan :

```css
p {
  text-indent: 20px;
}
```

### Properti `line-height`

Kita dapat mengatur jarak antar baris dari suatu teks menggunakan properti `line-height` dan value yang ditentukan berupa jarak.

Contoh penggunaan :

```css
p.small {
  line-height: 0.8rem;
}

p.big {
  line-height: 1.8rem;
}
```

### Properti `letter-spacing`

Kita dapat mengatur jarak antar huruf dari suatu teks menggunakan properti `letter-spacing` dan value yang ditentukan berupa jarak.

Contoh penggunaan :

```css
p {
  letter-spacing: 5px;
}
```

### Properti `word-spacing`

Kita dapat mengatur jarak antar kata dari suatu teks menggunakan properti `word-spacing` dan value yang ditentukan berupa jarak.

Contoh penggunaan :

```css
p.satu {
  word-spacing: 10px;
}

p.dua {
  word-spacing: -2px;
}
```

### Properti `white-space`

Kita dapat mengatur bagaimana karakter spasi diberlakukan menggunakan properti `white-space`.

Contoh penggunaan :

```css
p {
  white-space: nowrap;
}
```

## Text Shadow

Kita dapat memberi dan mengatur bayangan dari suatu teks dengan menggunakan properti `text-shadow`.
Properti ini sendiri pada bentuk paling simpelnya mempunyai posisi horizontal dan vertikal bayangan.

Berikut cara menggunakan properti `text-shadow` :

### Dasar

```css
h1 {
  text-shadow: 2px 2px;
}
```

### Dengan Warna

```css
h1 {
  text-shadow: 2px 2px #6699dd;
}
```

### Dengan Warna dan Shadow Blur

```css
h1 {
  text-shadow: 2px 2px 10px #6699dd;
}
```

### Lebih Dari 1 Bayangan

```css
h1 {
  text-shadow: 2px 2px 10px #6699dd, -2px -2px 10px #9966ff;
}
```
