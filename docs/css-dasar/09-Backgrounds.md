---
title: 09 - Backgrounds
---

# Backgrounds

Properti `background` pada CSS digunakan untuk mengatur background dan efek background untuk elemen.

## Background Color

Properti `background-color` digunakan untuk mengatur warna background pada suatu elemen.
Jenis value dapat menggunakan value yang properti `color` izinkan.

Contoh implementasi :

```css
body {
  background-color: lightblue;
}
```

## Opacity

Properti `opacity` digunakan untuk mengatur opasitas suatu elemen.

Contoh implementasi :

```css
div {
  background-color: green;
  opacity: 0.3;
}
```

## Background Image

Properti `background-image` digunakan untuk mengatur gambar background suatu elemen.

Contoh implementasi :

```css
body {
  background-image: url("paper.png");
}
```

## Background Repeat

Properti `background-repeat` digunakan untuk mengulang gambar secara horizontal, vertikal, maupun keduanya.

Contoh implementasi :

```css
body {
  background-image: url("gradient_bg.png");
}
```

## Background Position

Properti `background-position` digunakan untuk mengatur posisi gambar background.

Contoh implementasi :

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```

## Background Attachment

Properti `background-attachment` digunakan untuk mengatur apakah gambar background harus mengikuti scroll atau tetap diam.

Contoh implementasi :

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
```

## Shorthand

Properti `background` dapat digunakan sebagai shorthand untuk mengatur background halaman.

Jadi, selain mengimplementasikan background seperti berikut :

```css
body {
  background-color: #ffffff;
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
}
```

Kita dapat melakukannya seperti ini :

```css
body {
  background: #ffffff url("img_tree.png") no-repeat right top;
}
```

Harus diingat bahwa aturan shorthand sebagai berikut :

`background-color` - `background-image` - `background-repeat` - `background-attachment` - `background-position`
