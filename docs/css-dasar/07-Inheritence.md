---
title : 07 - Inheritance
---

# Inheritance (Pewarisan)

Inheritance merupakan salah satu konsep dalam CSS yang dimana sebuah parent mewariskan properti yang ia miliki pada
child atau anaknya. Contoh :

```html
<body>
<nav>Ini Navigasi</nav>
<h1>Web Development Series</h1>
<p>Kata kakek-ku kuku kaki kakak-ku kaku kaku</p>
</body>
```

```css
body {
    color: red;
    font-size: 16px;
    font-family: sans-serif;

    border: 10px solid #00a4db;
}
```

Saat kita jalankan, bisa dilihat bahwa beberapa properti seperti `color`, `font-size`, dan `font-family` berlaku juga
pada elemen lainya, sedangkan properti `border` tidak, inilah yang disebut dengan pewarisan.

Kita bisa menimpa properti yang telah didefiniskan sebelumnya pada parent dengan cara **menimpa-nya**. Contoh :

```css
h1 {
    color: blue;
    font-size: 32px;
    text-transform: uppercase;
}
```

Dan jika dijalankan kembali, warna dari teks h1 yang awalnya berwarna merah berubah menjadi biru.